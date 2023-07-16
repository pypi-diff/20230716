# Comparing `tmp/i8-terminal-0.2.97.tar.gz` & `tmp/i8-terminal-0.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8-terminal-0.2.97.tar", last modified: Sun Jul  9 08:43:01 2023, max compression
+gzip compressed data, was "i8-terminal-0.2.98.tar", last modified: Sun Jul 16 16:30:14 2023, max compression
```

## Comparing `i8-terminal-0.2.97.tar` & `i8-terminal-0.2.98.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:01.001280 i8-terminal-0.2.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-09 08:43:01.001280 i8-terminal-0.2.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.981280 i8-terminal-0.2.97/i8_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.981280 i8-terminal-0.2.97/i8_terminal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.981280 i8-terminal-0.2.97/i8_terminal/api/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/api/earnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/app/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/app/plot_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-07-09 08:41:47.000000 i8-terminal-0.2.97/i8_terminal/assets/i8t_chart_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/assets/i8t_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/assets/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/assets/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/commands/company/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/company/company_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/company/company_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/company/compnay_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/commands/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/earnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_recent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_upcoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.985280 i8-terminal-0.2.97/i8_terminal/commands/financials/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/financials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/financials/financials_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/financials/financials_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/financials/financials_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/financials/financials_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/market/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/market/market_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_describe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/news/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/news/news_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/notebook/notebook_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/price/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/price/price_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/price/price_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/price/price_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/screen/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/screen/screen_gainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/screen/screen_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/screen/screen_losers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/screen/screen_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.989280 i8-terminal-0.2.97/i8_terminal/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/user/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/user/user_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/user/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.993280 i8-terminal-0.2.97/i8_terminal/commands/watchlist/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.993280 i8-terminal-0.2.97/i8_terminal/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/i8_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.993280 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 08:43:00.000000 i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.993280 i8-terminal-0.2.97/i8_terminal/service_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/service_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/service_result/column_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/service_result/columns_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/service_result/earning_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/service_result/service_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:00.997280 i8-terminal-0.2.97/i8_terminal/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/services/earnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:43:01.001280 i8-terminal-0.2.97/i8_terminal/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/auto_complete_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/chart_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/fin_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/fin_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/fin_statement_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/i8_auto_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/i8_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/indicator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/market_indice_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/metric_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/metric_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/metric_view_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/output_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/period_type_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/price_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/screening_condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/screening_operator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/screening_value_field_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/sort_order_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/ticker_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/user_watchlist_tickers_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/types/user_watchlists_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/utils_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/i8_terminal/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 08:43:01.001280 i8-terminal-0.2.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-09 08:41:48.000000 i8-terminal-0.2.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/api/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/api/earnings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/app/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/app/plot_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/assets/i8t_chart_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/assets/i8t_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/assets/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/assets/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/commands/company/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/company/company_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/company/company_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/company/compnay_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/commands/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/earnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_upcoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/commands/financials/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/financials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/financials/financials_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/financials/financials_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/financials/financials_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/financials/financials_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.097253 i8-terminal-0.2.98/i8_terminal/commands/market/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/market/market_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/news/news_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/notebook/notebook_launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/price/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/price/price_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/price/price_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/price/price_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/screen/screen_gainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/screen/screen_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/screen/screen_losers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/screen/screen_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/user/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/user/user_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/user/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/commands/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.101253 i8-terminal-0.2.98/i8_terminal/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/i8_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 16:30:14.000000 i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/i8_terminal/service_result/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/service_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/service_result/column_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/service_result/columns_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/service_result/earning_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/service_result/service_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/i8_terminal/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/services/earnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/i8_terminal/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/auto_complete_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/chart_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/fin_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/fin_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/fin_statement_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/i8_auto_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/i8_completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/indicator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/market_indice_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/metric_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/metric_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/metric_view_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/output_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/period_type_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/price_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/screening_condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/screening_operator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/screening_value_field_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/sort_order_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/ticker_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/user_watchlist_tickers_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/types/user_watchlists_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/utils_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/i8_terminal/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:30:14.105253 i8-terminal-0.2.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-16 16:29:16.000000 i8-terminal-0.2.98/setup.py
```

### Comparing `i8-terminal-0.2.97/LICENSE` & `i8-terminal-0.2.98/LICENSE`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/PKG-INFO` & `i8-terminal-0.2.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.97
+Version: 0.2.98
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.97/README.md` & `i8-terminal-0.2.98/README.md`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/app/layout.py` & `i8-terminal-0.2.98/i8_terminal/app/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/app/plot_server.py` & `i8-terminal-0.2.98/i8_terminal/app/plot_server.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/assets/favicon.ico` & `i8-terminal-0.2.98/i8_terminal/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/assets/i8t_chart_logo.png` & `i8-terminal-0.2.98/i8_terminal/assets/i8t_chart_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/assets/i8t_logo.png` & `i8-terminal-0.2.98/i8_terminal/assets/i8t_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/assets/loading.gif` & `i8-terminal-0.2.98/i8_terminal/assets/loading.gif`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/assets/styles.css` & `i8-terminal-0.2.98/i8_terminal/assets/styles.css`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/company/company_compare.py` & `i8-terminal-0.2.98/i8_terminal/commands/company/company_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/company/company_search.py` & `i8-terminal-0.2.98/i8_terminal/commands/company/company_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/company/compnay_details.py` & `i8-terminal-0.2.98/i8_terminal/commands/company/compnay_details.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_list.py` & `i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_plot.py` & `i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_recent.py` & `i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_recent.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/earnings/earnings_upcoming.py` & `i8-terminal-0.2.98/i8_terminal/commands/earnings/earnings_upcoming.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/financials/financials_compare.py` & `i8-terminal-0.2.98/i8_terminal/commands/financials/financials_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/financials/financials_coverage.py` & `i8-terminal-0.2.98/i8_terminal/commands/financials/financials_coverage.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/financials/financials_list.py` & `i8-terminal-0.2.98/i8_terminal/commands/financials/financials_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/financials/financials_plot.py` & `i8-terminal-0.2.98/i8_terminal/commands/financials/financials_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/market/market_summary.py` & `i8-terminal-0.2.98/i8_terminal/commands/market/market_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_current.py` & `i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_current.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     Examples:
 
     `i8 metrics current --metrics total_revenue.q,net_income.fy,close.d,total_revenue --tickers AMD,INTC,QCOM`
     """  # noqa: E501
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = get_current_metrics_df(tickers, metrics.replace(".p", ""))
-    if df is None:
+    if df is None or df.empty:
         console.print("No data found for metrics with selected tickers", style="yellow")
         return
     for m in [*set(metric.split(".")[0] for metric in set(metrics.split(","))) - set(df["metric_name"])]:
         console.print(f"\nNo data found for metric {m} with selected tickers", style="yellow")
     columns_justify: Dict[str, Any] = {}
     if export_path:
         if export_path.split(".")[-1] == "html":
```

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_describe.py` & `i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_describe.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_historical.py` & `i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_historical.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/metrics/metrics_search.py` & `i8-terminal-0.2.98/i8_terminal/commands/metrics/metrics_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/news/news_list.py` & `i8-terminal-0.2.98/i8_terminal/commands/news/news_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/notebook/notebook_launch.py` & `i8-terminal-0.2.98/i8_terminal/commands/notebook/notebook_launch.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/price/price_compare.py` & `i8-terminal-0.2.98/i8_terminal/commands/price/price_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/price/price_list.py` & `i8-terminal-0.2.98/i8_terminal/commands/price/price_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/price/price_plot.py` & `i8-terminal-0.2.98/i8_terminal/commands/price/price_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/screen/screen_gainers.py` & `i8-terminal-0.2.98/i8_terminal/commands/screen/screen_gainers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/screen/screen_losers.py` & `i8-terminal-0.2.98/i8_terminal/commands/screen/screen_losers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/screen/screen_search.py` & `i8-terminal-0.2.98/i8_terminal/commands/screen/screen_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/user/user_login.py` & `i8-terminal-0.2.98/i8_terminal/commands/user/user_login.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/user/webserver.py` & `i8-terminal-0.2.98/i8_terminal/commands/user/webserver.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_add.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_add.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_create.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_create.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_export.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_export.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_financials.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_list.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_metrics.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_rm.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_rm.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/commands/watchlist/watchlist_summary.py` & `i8-terminal-0.2.98/i8_terminal/commands/watchlist/watchlist_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/cli.py` & `i8-terminal-0.2.98/i8_terminal/common/cli.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/financials.py` & `i8-terminal-0.2.98/i8_terminal/common/financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/formatting.py` & `i8-terminal-0.2.98/i8_terminal/common/formatting.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/layout.py` & `i8-terminal-0.2.98/i8_terminal/common/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/metrics.py` & `i8-terminal-0.2.98/i8_terminal/common/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     return period_start_date[period]
 
 
 def get_current_metrics_df(tickers: str, metricsList: str) -> Optional[pd.DataFrame]:
     stocks_peers = get_stocks_df()[["ticker", "peers"]].set_index("ticker").to_dict()["peers"]
     tickers_list = []
     for tk in tickers.split(","):
-        if "PEERS" in tk and stocks_peers.get(tk.split(".")[0]):
+        if "peers" in tk and stocks_peers.get(tk.split(".")[0]):
             ticker_name = tk.split(".")[0]
             tickers_list.append(ticker_name)
             tickers_list.extend(literal_eval(stocks_peers.get(ticker_name)))
         else:
             tickers_list.append(tk)
     metrics = investor8_sdk.MetricsApi().get_current_metrics(
         symbols=",".join(tickers_list),
@@ -136,14 +136,16 @@
     if metrics.data is None:
         return None
     metrics_data_df = pd.DataFrame([m.to_dict() for m in metrics.data])
     metrics_data_df.rename(columns={"metric": "metric_name", "symbol": "Ticker"}, inplace=True)
     metrics_metadata_df = pd.DataFrame([m.to_dict() for m in metrics.metadata])
     df = pd.merge(metrics_data_df, metrics_metadata_df, on="metric_name")
     df[["data_format", "display_format"]] = df[["data_format", "display_format"]].replace("string", "str")
+    df["value"].replace("None", np.nan, inplace=True)
+    df.dropna(subset=["value"], axis=0, inplace=True)
     return df
 
 
 def prepare_current_metrics_formatted_df(df: DataFrame, target: str, include_period: bool = False) -> DataFrame:
     formatted_df = format_metrics_df(df, target)
     if include_period:
         formatted_df.rename(columns={"period": "Period"}, inplace=True)
```

### Comparing `i8-terminal-0.2.97/i8_terminal/common/price.py` & `i8-terminal-0.2.98/i8_terminal/common/price.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/screen.py` & `i8-terminal-0.2.98/i8_terminal/common/screen.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/common/stock_info.py` & `i8-terminal-0.2.98/i8_terminal/common/stock_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 
 from i8_terminal.common.utils import is_cached_file_expired
 from i8_terminal.config import SETTINGS_FOLDER
 
 
 def sort_stocks(df: pd.DataFrame, include_peers: bool = False) -> pd.DataFrame:
     df["default_rank"] = 11
-    default_rank = (
-        {
+    if not include_peers:
+        default_rank = {
             "A": 1,
             "AAL": 2,
             "AAP": 3,
             "AAPL": 4,
             "AABV": 5,
             "ABC": 6,
             "ABMD": 7,
             "ABT": 8,
             "ACN": 9,
             "ADBE": 10,
         }
-        if not include_peers
-        else {
+    else:
+        default_rank = {
             "A": 1,
             "A.peers": 2,
             "AAL": 3,
             "AAL.peers": 4,
             "AAP": 5,
             "AAP.peers": 6,
             "AAPL": 7,
             "AAPL.peers": 8,
             "AABV": 9,
             "AABV.peers": 10,
         }
-    )
     df["default_rank"] = df["ticker"].apply(lambda x: default_rank.get(x, 11))
     df = df.sort_values("default_rank").reset_index(drop=True)
     return df[["ticker", "name", "peers"]]
 
 
 def get_stocks_df() -> pd.DataFrame:
     companies_path = f"{SETTINGS_FOLDER}/companies.csv"
@@ -57,15 +56,16 @@
 
 
 def get_stocks(include_peers: bool) -> List[Tuple[str, str]]:
     columns_list = ["ticker", "name"]
     df = get_stocks_df().replace("", np.nan)
     if include_peers:
         df_peers = df[~df["peers"].isna()].copy()
-        df_peers.loc[:, "ticker"] = df_peers["ticker"].apply(lambda x: x + ".PEERS")
+        df_peers.loc[:, "ticker"] = df_peers["ticker"].apply(lambda x: x + ".peers")
+        df_peers.loc[:, "name"] = df_peers["name"].apply(lambda x: "Peers of " + x)
         df = sort_stocks(pd.concat([df, df_peers]), include_peers)
     return list(df[columns_list].to_records(index=False))
 
 
 def validate_ticker(ctx: click.Context, param: str, value: str) -> Optional[str]:
     if not ctx.resilient_parsing:
         if value and len(value.replace(" ", "").split(",")) > 1:
@@ -76,15 +76,15 @@
             ctx.exit()
     return value
 
 
 def validate_tickers(ctx: click.Context, param: str, value: str) -> Optional[str]:
     tickers = {d[0] for d in get_stocks(True)}
     if not ctx.resilient_parsing:
-        invalid_tickers = [*set(value.replace(" ", "").upper().split(",")) - tickers] if value else []
+        invalid_tickers = [*set(value.replace(" ", "").split(",")) - tickers] if value else []
         if value and invalid_tickers:
             msg = "are not valid ticker names." if len(invalid_tickers) > 1 else "is not a valid ticker name."
             click.echo(
                 click.style(
                     f"`{', '.join(invalid_tickers)}` {msg}",
                     fg="yellow",
                 )
```

### Comparing `i8-terminal-0.2.97/i8_terminal/common/utils.py` & `i8-terminal-0.2.98/i8_terminal/common/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import enum
 import os
 from difflib import SequenceMatcher
 from io import StringIO
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
 import arrow
+import click
 import pandas as pd
+from prompt_toolkit.document import Document
 from rich.console import Console
 
 from i8_terminal.config import APP_SETTINGS
+from i8_terminal.types.command_parser import CompleterContext
 
 T = TypeVar("T")
 
 
 class PlotType(enum.Enum):
     CHART = "chart"
     TABLE = "table"
@@ -122,7 +125,24 @@
         return wrapper
 
     return decorate
 
 
 def concat_and(items: List[str]) -> str:
     return " and ".join(", ".join(items).rsplit(", ", 1))
+
+
+def get_matched_params(ctx: CompleterContext, command: click.Command, document: Document) -> List[click.Option]:
+    if not document.is_cursor_at_the_end:
+        command_string = document.current_line
+        cursor_position = document.cursor_position
+        options_positions = [
+            (o, cursor_position - command_string.find(o))
+            for c in command.params
+            for o in ctx.used_options
+            if cursor_position - command_string.find(o) > 0
+        ]
+        matched = min(options_positions, key=lambda option_position: option_position[1])  # type: ignore
+        matched_params = [p for p in command.params if isinstance(p, click.Option) and matched[0] in p.opts]
+    else:
+        matched_params = [p for p in command.params if isinstance(p, click.Option) and ctx.last_option in p.opts]
+    return matched_params
```

### Comparing `i8-terminal-0.2.97/i8_terminal/config.py` & `i8-terminal-0.2.98/i8_terminal/config.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/config.yml` & `i8-terminal-0.2.98/i8_terminal/config.yml`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/PKG-INFO` & `i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.97
+Version: 0.2.98
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.97/i8_terminal/i8_terminal.egg-info/SOURCES.txt` & `i8-terminal-0.2.98/i8_terminal/i8_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/main.py` & `i8-terminal-0.2.98/i8_terminal/main.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/service_result/column_info.py` & `i8-terminal-0.2.98/i8_terminal/service_result/column_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/service_result/columns_context.py` & `i8-terminal-0.2.98/i8_terminal/service_result/columns_context.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/service_result/earning_list_result.py` & `i8-terminal-0.2.98/i8_terminal/service_result/earning_list_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/service_result/service_result.py` & `i8-terminal-0.2.98/i8_terminal/service_result/service_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/services/earnings.py` & `i8-terminal-0.2.98/i8_terminal/services/earnings.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/auto_complete_choice.py` & `i8-terminal-0.2.98/i8_terminal/types/auto_complete_choice.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/chart_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/chart_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/command_parser.py` & `i8-terminal-0.2.98/i8_terminal/types/command_parser.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/condition_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/fin_identifier_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/fin_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/fin_period_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/fin_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/fin_statement_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/fin_statement_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/i8_auto_suggest.py` & `i8-terminal-0.2.98/i8_terminal/types/i8_auto_suggest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import click
 from click import Group
 from click.decorators import F
 from prompt_toolkit.auto_suggest import AutoSuggest, Suggestion
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.document import Document
 
+from i8_terminal.common.utils import get_matched_params
 from i8_terminal.types.command_parser import CommandParser
 from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType
 from i8_terminal.types.metric_identifier_param_type import MetricIdentifierParamType
 
 
 class I8AutoSuggest(AutoSuggest):
     """
@@ -24,15 +25,15 @@
         ctx = CommandParser(self.cli).parse(document)
         if not ctx:
             return None
 
         command = ctx.click_ctx.command
 
         if ctx.last_option:
-            matched_params = [p for p in command.params if isinstance(p, click.Option) and ctx.last_option in p.opts]
+            matched_params = get_matched_params(ctx, command, document)
             if len(matched_params) > 0:
                 matched_param = matched_params[0]
                 if type(matched_param.type) is click.types.DateTime:
                     return Suggestion("YYYY-MM-DD"[len(ctx.incomplete) :])  # noqa: E203
                 elif type(matched_param.type) is FinancialsIdentifierParamType:
                     parts_num = 3
                     parts = ctx.incomplete.split(",")
```

### Comparing `i8-terminal-0.2.97/i8_terminal/types/i8_completer.py` & `i8-terminal-0.2.98/i8_terminal/types/i8_completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import click
 from click import Group
 from click.decorators import F
 from click_repl import ClickCompleter, text_type
 from prompt_toolkit.completion import CompleteEvent, Completion
 from prompt_toolkit.document import Document
 
+from i8_terminal.common.utils import get_matched_params
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 from i8_terminal.types.chart_param_type import ChartParamType
 from i8_terminal.types.command_parser import CommandParser
 from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType
 from i8_terminal.types.fin_period_param_type import FinancialsPeriodParamType
 from i8_terminal.types.fin_statement_param_type import FinancialStatementParamType
 from i8_terminal.types.indicator_param_type import IndicatorParamType
@@ -41,15 +42,15 @@
 
         command = ctx.click_ctx.command
 
         choices = []
         filter_choices = True
 
         if ctx.last_option:
-            matched_params = [p for p in command.params if isinstance(p, click.Option) and ctx.last_option in p.opts]
+            matched_params = get_matched_params(ctx, command, document)
             if len(matched_params) > 0:
                 matched_param = matched_params[0]
                 if type(matched_param.type) is click.types.Choice:
                     for c in matched_param.type.choices:
                         choices.append(Completion(text_type(c), -len(ctx.incomplete)))
 
                 elif type(matched_param.type) in [
@@ -77,15 +78,15 @@
                         incomplete = ctx.incomplete
                     else:
                         parts = ctx.incomplete.split(",")
                         incomplete = parts[-1] if len(parts) > 0 else " "
                     for (ticker, name) in matched_param.type.get_suggestions(  # type: ignore
                         incomplete if incomplete else " ", True, include_peers
                     ):
-                        choices.append(Completion(text_type(ticker.upper()), -len(incomplete), display_meta=name))
+                        choices.append(Completion(text_type(ticker), -len(incomplete), display_meta=name))
                 elif type(matched_param.type) in [MetricParamType, IndicatorParamType]:
                     filter_choices = False
                     parts = ctx.incomplete.split(",")
                     incomplete = parts[-1] if len(parts) > 0 else " "
                     for (metric, name) in matched_param.type.get_suggestions(  # type: ignore
                         incomplete if incomplete else " ", True
                     ):
```

### Comparing `i8-terminal-0.2.97/i8_terminal/types/indicator_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/indicator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/market_indice_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/market_indice_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/metric_identifier_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/metric_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/metric_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/metric_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/metric_view_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/metric_view_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/output_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/output_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/period_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/period_type_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/period_type_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/price_period_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/price_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/screening_condition_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/screening_condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/screening_operator_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/screening_operator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/screening_value_field_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/screening_value_field_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/sort_order_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/sort_order_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/ticker_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/ticker_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/user_watchlist_tickers_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/user_watchlist_tickers_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/types/user_watchlists_param_type.py` & `i8-terminal-0.2.98/i8_terminal/types/user_watchlists_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/i8_terminal/utils_setup.py` & `i8-terminal-0.2.98/i8_terminal/utils_setup.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.97/setup.py` & `i8-terminal-0.2.98/setup.py`

 * *Files identical despite different names*

