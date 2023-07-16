# Comparing `tmp/redis-5.0.0rc1.tar.gz` & `tmp/redis-5.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.0.0rc1.tar", last modified: Tue Jun 27 18:40:37 2023, max compression
+gzip compressed data, was "redis-5.0.0rc2.tar", last modified: Sun Jul 16 12:13:24 2023, max compression
```

## Comparing `redis-5.0.0rc1.tar` & `redis-5.0.0rc2.tar`

### file list

```diff
@@ -1,158 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.150637 redis-5.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 18:40:17.000000 redis-5.0.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:40:17.000000 redis-5.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 18:40:17.000000 redis-5.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-27 18:40:37.150637 redis-5.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-27 18:40:17.000000 redis-5.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.118637 redis-5.0.0rc1/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55541 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61437 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    52680 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    84080 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    90814 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   217539 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.130637 redis-5.0.0rc1/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    48046 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/ocsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.130637 redis-5.0.0rc1/redis/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.118637 redis-5.0.0rc1/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:40:37.150637 redis-5.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-27 18:40:17.000000 redis-5.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.138637 redis-5.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/asynctests
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/synctests
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.142637 redis-5.0.0rc1/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   113908 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34543 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    35100 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38167 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    57127 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.142637 redis-5.0.0rc1/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   119547 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   177287 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30431 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.146637 redis-5.0.0rc1/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    47244 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    43246 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    80154 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    33464 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.146637 redis-5.0.0rc1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.562458 redis-5.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 12:13:07.000000 redis-5.0.0rc2/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 12:13:07.000000 redis-5.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-16 12:13:07.000000 redis-5.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-16 12:13:24.562458 redis-5.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-16 12:13:07.000000 redis-5.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis/_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27882 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/_parsers/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55900 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62460 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51346 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55427 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92237 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31125 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219147 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.550458 redis-5.0.0rc2/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.550458 redis-5.0.0rc2/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.550458 redis-5.0.0rc2/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36125 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.550458 redis-5.0.0rc2/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48911 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-16 12:13:07.000000 redis-5.0.0rc2/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.546458 redis-5.0.0rc2/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-16 12:13:24.000000 redis-5.0.0rc2/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-16 12:13:24.000000 redis-5.0.0rc2/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:13:24.000000 redis-5.0.0rc2/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-16 12:13:24.000000 redis-5.0.0rc2/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 12:13:24.000000 redis-5.0.0rc2/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:13:24.562458 redis-5.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-16 12:13:07.000000 redis-5.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.554458 redis-5.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/ssl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.558458 redis-5.0.0rc2/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118006 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127626 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_cwe_404.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36682 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38377 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57127 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.558458 redis-5.0.0rc2/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125393 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182063 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30760 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.558458 redis-5.0.0rc2/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48732 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43249 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80154 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33464 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:13:24.558458 redis-5.0.0rc2/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-07-16 12:13:07.000000 redis-5.0.0rc2/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.0.0rc1/LICENSE` & `redis-5.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/PKG-INFO` & `redis-5.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0rc1/README.md` & `redis-5.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/__init__.py` & `redis-5.0.0rc2/redis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     AuthenticationError,
     AuthenticationWrongNumberOfArgsError,
     BusyLoadingError,
     ChildDeadlockedError,
     ConnectionError,
     DataError,
     InvalidResponse,
+    OutOfMemoryError,
     PubSubError,
     ReadOnlyError,
     RedisError,
     ResponseError,
     TimeoutError,
     WatchError,
 )
@@ -69,14 +70,15 @@
     "ConnectionError",
     "ConnectionPool",
     "CredentialProvider",
     "DataError",
     "from_url",
     "default_backoff",
     "InvalidResponse",
+    "OutOfMemoryError",
     "PubSubError",
     "ReadOnlyError",
     "Redis",
     "RedisCluster",
     "RedisError",
     "ResponseError",
     "Sentinel",
```

### Comparing `redis-5.0.0rc1/redis/asyncio/__init__.py` & `redis-5.0.0rc2/redis/asyncio/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AuthenticationError,
     AuthenticationWrongNumberOfArgsError,
     BusyLoadingError,
     ChildDeadlockedError,
     ConnectionError,
     DataError,
     InvalidResponse,
+    OutOfMemoryError,
     PubSubError,
     ReadOnlyError,
     RedisError,
     ResponseError,
     TimeoutError,
     WatchError,
 )
@@ -41,14 +42,15 @@
     "ConnectionError",
     "ConnectionPool",
     "DataError",
     "from_url",
     "default_backoff",
     "InvalidResponse",
     "PubSubError",
+    "OutOfMemoryError",
     "ReadOnlyError",
     "Redis",
     "RedisCluster",
     "RedisError",
     "ResponseError",
     "Sentinel",
     "SentinelConnectionPool",
```

### Comparing `redis-5.0.0rc1/redis/asyncio/client.py` & `redis-5.0.0rc2/redis/asyncio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,33 @@
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
+from redis._parsers.helpers import (
+    _RedisCallbacks,
+    _RedisCallbacksRESP2,
+    _RedisCallbacksRESP3,
+    bool_ok,
+)
 from redis.asyncio.connection import (
     Connection,
     ConnectionPool,
     SSLConnection,
     UnixDomainSocketConnection,
 )
 from redis.asyncio.lock import Lock
 from redis.asyncio.retry import Retry
 from redis.client import (
     EMPTY_RESPONSE,
     NEVER_DECODE,
     AbstractRedis,
     CaseInsensitiveDict,
-    bool_ok,
 )
 from redis.commands import (
     AsyncCoreCommands,
     AsyncRedisModuleCommands,
     AsyncSentinelCommands,
     list_or_args,
 )
@@ -135,16 +140,20 @@
         or "Yes"/"No". Values that cannot be properly cast cause a
         ``ValueError`` to be raised. Once parsed, the querystring arguments
         and keyword arguments are passed to the ``ConnectionPool``'s
         class initializer. In the case of conflicting arguments, querystring
         arguments always win.
 
         """
+        single_connection_client = kwargs.pop("single_connection_client", False)
         connection_pool = ConnectionPool.from_url(url, **kwargs)
-        return cls(connection_pool=connection_pool)
+        return cls(
+            connection_pool=connection_pool,
+            single_connection_client=single_connection_client,
+        )
 
     def __init__(
         self,
         *,
         host: str = "localhost",
         port: int = 6379,
         db: Union[str, int] = 0,
@@ -249,20 +258,20 @@
                         }
                     )
             connection_pool = ConnectionPool(**kwargs)
         self.connection_pool = connection_pool
         self.single_connection_client = single_connection_client
         self.connection: Optional[Connection] = None
 
-        self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
+        self.response_callbacks = CaseInsensitiveDict(_RedisCallbacks)
 
         if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+            self.response_callbacks.update(_RedisCallbacksRESP3)
         else:
-            self.response_callbacks.update(self.__class__.RESP2_RESPONSE_CALLBACKS)
+            self.response_callbacks.update(_RedisCallbacksRESP2)
 
         # If using a single connection client, we need to lock creation-of and use-of
         # the client in order to avoid race conditions such as using asyncio.gather
         # on a set of redis commands
         self._single_conn_lock = asyncio.Lock()
 
     def __repr__(self):
@@ -458,15 +467,15 @@
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
     _DEL_MESSAGE = "Unclosed Redis client"
 
     def __del__(self, _warnings: Any = warnings) -> None:
-        if self.connection is not None:
+        if hasattr(self, "connection") and (self.connection is not None):
             _warnings.warn(
                 f"Unclosed client session {self!r}", ResourceWarning, source=self
             )
             context = {"client": self, "message": self._DEL_MESSAGE}
             asyncio.get_running_loop().call_exception_handler(context)
 
     async def close(self, close_connection_pool: Optional[bool] = None) -> None:
@@ -709,14 +718,19 @@
                 self.connection = None
             self.channels = {}
             self.pending_unsubscribe_channels = set()
             self.patterns = {}
             self.pending_unsubscribe_patterns = set()
 
     def close(self) -> Awaitable[NoReturn]:
+        # In case a connection property does not yet exist
+        # (due to a crash earlier in the Redis() constructor), return
+        # immediately as there is nothing to clean-up.
+        if not hasattr(self, "connection"):
+            return
         return self.reset()
 
     async def on_connect(self, connection: Connection):
         """Re-subscribe to any channels and patterns previously subscribed to"""
         # NOTE: for python3, we can't pass bytestrings as keyword arguments
         # so we need to decode channel/pattern names back to unicode strings
         # before passing them to [p]subscribe.
@@ -802,15 +816,19 @@
         await self.check_health()
 
         if not conn.is_connected:
             await conn.connect()
 
         read_timeout = None if block else timeout
         response = await self._execute(
-            conn, conn.read_response, timeout=read_timeout, push_request=True
+            conn,
+            conn.read_response,
+            timeout=read_timeout,
+            disconnect_on_error=False,
+            push_request=True,
         )
 
         if conn.health_check_interval and response in self.health_check_response:
             # ignore the health check message as user might not expect it
             return None
         return response
 
@@ -1400,24 +1418,18 @@
             conn = await self.connection_pool.get_connection("MULTI", self.shard_hint)
             # assign to self.connection so reset() releases the connection
             # back to the pool after we're done
             self.connection = conn
         conn = cast(Connection, conn)
 
         try:
-            return await asyncio.shield(
-                conn.retry.call_with_retry(
-                    lambda: execute(conn, stack, raise_on_error),
-                    lambda error: self._disconnect_raise_reset(conn, error),
-                )
+            return await conn.retry.call_with_retry(
+                lambda: execute(conn, stack, raise_on_error),
+                lambda error: self._disconnect_raise_reset(conn, error),
             )
-        except asyncio.CancelledError:
-            # not supposed to be possible, yet here we are
-            await conn.disconnect(nowait=True)
-            raise
         finally:
             await self.reset()
 
     async def discard(self):
         """Flushes all previously queued commands
         See: https://redis.io/commands/DISCARD
         """
```

### Comparing `redis-5.0.0rc1/redis/asyncio/cluster.py` & `redis-5.0.0rc2/redis/asyncio/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import asyncio
 import collections
 import random
 import socket
 import warnings
 from typing import (
     Any,
+    Callable,
     Deque,
     Dict,
     Generator,
     List,
     Mapping,
     Optional,
+    Tuple,
     Type,
     TypeVar,
     Union,
 )
 
+from redis._parsers import AsyncCommandsParser, Encoder
+from redis._parsers.helpers import (
+    _RedisCallbacks,
+    _RedisCallbacksRESP2,
+    _RedisCallbacksRESP3,
+)
 from redis.asyncio.client import ResponseCallbackT
 from redis.asyncio.connection import Connection, DefaultParser, SSLConnection, parse_url
 from redis.asyncio.lock import Lock
 from redis.asyncio.retry import Retry
 from redis.backoff import default_backoff
 from redis.client import EMPTY_RESPONSE, NEVER_DECODE, AbstractRedis
 from redis.cluster import (
@@ -49,15 +57,14 @@
     MovedError,
     RedisClusterException,
     ResponseError,
     SlotNotCoveredError,
     TimeoutError,
     TryAgainError,
 )
-from redis.parsers import AsyncCommandsParser, Encoder
 from redis.typing import AnyKeyT, EncodableT, KeyT
 from redis.utils import dict_merge, safe_str, str_if_bytes
 
 TargetNodesT = TypeVar(
     "TargetNodesT", str, "ClusterNode", List["ClusterNode"], Dict[Any, "ClusterNode"]
 )
 
@@ -137,14 +144,20 @@
           default_backoff in backoff.py). To change it, pass a custom Retry object
           using the "retry" keyword.
     :param max_connections:
         | Maximum number of connections per node. If there are no free connections & the
           maximum number of connections are already created, a
           :class:`~.MaxConnectionsError` is raised. This error may be retried as defined
           by :attr:`connection_error_retry_attempts`
+    :param address_remap:
+        | An optional callable which, when provided with an internal network
+          address of a node, e.g. a `(host, port)` tuple, will return the address
+          where the node is reachable.  This can be used to map the addresses at
+          which the nodes _think_ they are, to addresses at which a client may
+          reach them, such as when they sit behind a proxy.
 
     | Rest of the arguments will be passed to the
       :class:`~redis.asyncio.connection.Connection` instances when created
 
     :raises RedisClusterException:
         if any arguments are invalid or unknown. Eg:
 
@@ -231,24 +244,25 @@
         # Connection related kwargs
         health_check_interval: float = 0,
         socket_connect_timeout: Optional[float] = None,
         socket_keepalive: bool = False,
         socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
         socket_timeout: Optional[float] = None,
         retry: Optional["Retry"] = None,
-        retry_on_error: Optional[List[Exception]] = None,
+        retry_on_error: Optional[List[Type[Exception]]] = None,
         # SSL related kwargs
         ssl: bool = False,
         ssl_ca_certs: Optional[str] = None,
         ssl_ca_data: Optional[str] = None,
         ssl_cert_reqs: str = "required",
         ssl_certfile: Optional[str] = None,
         ssl_check_hostname: bool = False,
         ssl_keyfile: Optional[str] = None,
         protocol: Optional[int] = 2,
+        address_remap: Optional[Callable[[str, int], Tuple[str, int]]] = None,
     ) -> None:
         if db:
             raise RedisClusterException(
                 "Argument 'db' must be 0 or None in cluster mode"
             )
 
         if path:
@@ -314,34 +328,39 @@
             )
             if not retry_on_error:
                 # Default errors for retrying
                 retry_on_error = [ConnectionError, TimeoutError]
             self.retry.update_supported_errors(retry_on_error)
             kwargs.update({"retry": self.retry})
 
-        kwargs["response_callbacks"] = self.__class__.RESPONSE_CALLBACKS.copy()
+        kwargs["response_callbacks"] = _RedisCallbacks.copy()
         if kwargs.get("protocol") in ["3", 3]:
-            kwargs["response_callbacks"].update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+            kwargs["response_callbacks"].update(_RedisCallbacksRESP3)
         else:
-            kwargs["response_callbacks"].update(self.__class__.RESP2_RESPONSE_CALLBACKS)
+            kwargs["response_callbacks"].update(_RedisCallbacksRESP2)
         self.connection_kwargs = kwargs
 
         if startup_nodes:
             passed_nodes = []
             for node in startup_nodes:
                 passed_nodes.append(
                     ClusterNode(node.host, node.port, **self.connection_kwargs)
                 )
             startup_nodes = passed_nodes
         else:
             startup_nodes = []
         if host and port:
             startup_nodes.append(ClusterNode(host, port, **self.connection_kwargs))
 
-        self.nodes_manager = NodesManager(startup_nodes, require_full_coverage, kwargs)
+        self.nodes_manager = NodesManager(
+            startup_nodes,
+            require_full_coverage,
+            kwargs,
+            address_remap=address_remap,
+        )
         self.encoder = Encoder(encoding, encoding_errors, decode_responses)
         self.read_from_replicas = read_from_replicas
         self.reinitialize_steps = reinitialize_steps
         self.cluster_error_retry_attempts = cluster_error_retry_attempts
         self.connection_error_retry_attempts = connection_error_retry_attempts
         self.reinitialize_counter = 0
         self.commands_parser = AsyncCommandsParser()
@@ -998,26 +1017,18 @@
         # Acquire connection
         connection = self.acquire_connection()
 
         # Execute command
         await connection.send_packed_command(connection.pack_command(*args), False)
 
         # Read response
-        return await asyncio.shield(
-            self._parse_and_release(connection, args[0], **kwargs)
-        )
-
-    async def _parse_and_release(self, connection, *args, **kwargs):
         try:
-            return await self.parse_response(connection, *args, **kwargs)
-        except asyncio.CancelledError:
-            # should not be possible
-            await connection.disconnect(nowait=True)
-            raise
+            return await self.parse_response(connection, args[0], **kwargs)
         finally:
+            # Release connection
             self._free.append(connection)
 
     async def execute_pipeline(self, commands: List["PipelineCommand"]) -> bool:
         # Acquire connection
         connection = self.acquire_connection()
 
         # Execute command
@@ -1048,25 +1059,28 @@
         "connection_kwargs",
         "default_node",
         "nodes_cache",
         "read_load_balancer",
         "require_full_coverage",
         "slots_cache",
         "startup_nodes",
+        "address_remap",
     )
 
     def __init__(
         self,
         startup_nodes: List["ClusterNode"],
         require_full_coverage: bool,
         connection_kwargs: Dict[str, Any],
+        address_remap: Optional[Callable[[str, int], Tuple[str, int]]] = None,
     ) -> None:
         self.startup_nodes = {node.name: node for node in startup_nodes}
         self.require_full_coverage = require_full_coverage
         self.connection_kwargs = connection_kwargs
+        self.address_remap = address_remap
 
         self.default_node: "ClusterNode" = None
         self.nodes_cache: Dict[str, "ClusterNode"] = {}
         self.slots_cache: Dict[int, List["ClusterNode"]] = {}
         self.read_load_balancer = LoadBalancer()
         self._moved_exception: MovedError = None
 
@@ -1217,14 +1231,15 @@
                 for i in range(2, len(slot)):
                     slot[i] = [str_if_bytes(val) for val in slot[i]]
                 primary_node = slot[2]
                 host = primary_node[0]
                 if host == "":
                     host = startup_node.host
                 port = int(primary_node[1])
+                host, port = self.remap_host_port(host, port)
 
                 target_node = tmp_nodes_cache.get(get_node_name(host, port))
                 if not target_node:
                     target_node = ClusterNode(
                         host, port, PRIMARY, **self.connection_kwargs
                     )
                 # add this node to the nodes cache
@@ -1235,14 +1250,15 @@
                         tmp_slots[i] = []
                         tmp_slots[i].append(target_node)
                         replica_nodes = [slot[j] for j in range(3, len(slot))]
 
                         for replica_node in replica_nodes:
                             host = replica_node[0]
                             port = replica_node[1]
+                            host, port = self.remap_host_port(host, port)
 
                             target_replica_node = tmp_nodes_cache.get(
                                 get_node_name(host, port)
                             )
                             if not target_replica_node:
                                 target_replica_node = ClusterNode(
                                     host, port, REPLICA, **self.connection_kwargs
@@ -1308,14 +1324,24 @@
         await asyncio.gather(
             *(
                 asyncio.create_task(node.disconnect())
                 for node in getattr(self, attr).values()
             )
         )
 
+    def remap_host_port(self, host: str, port: int) -> Tuple[str, int]:
+        """
+        Remap the host and port returned from the cluster to a different
+        internal value.  Useful if the client is not connecting directly
+        to the cluster.
+        """
+        if self.address_remap:
+            return self.address_remap((host, port))
+        return host, port
+
 
 class ClusterPipeline(AbstractRedis, AbstractRedisCluster, AsyncRedisClusterCommands):
     """
     Create a new ClusterPipeline object.
 
     Usage::
```

### Comparing `redis-5.0.0rc1/redis/asyncio/connection.py` & `redis-5.0.0rc2/redis/asyncio/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import inspect
 import os
 import socket
 import ssl
 import sys
 import threading
 import weakref
+from abc import abstractmethod
 from itertools import chain
 from types import MappingProxyType
 from typing import (
     Any,
     Callable,
     Iterable,
     List,
@@ -21,15 +22,17 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from urllib.parse import ParseResult, parse_qs, unquote, urlparse
 
-if sys.version_info.major >= 3 and sys.version_info.minor >= 11:
+# the functionality is available in 3.11.x but has a major issue before
+# 3.11.3. See https://github.com/redis/redis-py/issues/2633
+if sys.version_info >= (3, 11, 3):
     from asyncio import timeout as async_timeout
 else:
     from async_timeout import timeout as async_timeout
 
 from redis.asyncio.retry import Retry
 from redis.backoff import NoBackoff
 from redis.compat import Protocol, TypedDict
@@ -44,15 +47,15 @@
     RedisError,
     ResponseError,
     TimeoutError,
 )
 from redis.typing import EncodableT
 from redis.utils import HIREDIS_AVAILABLE, str_if_bytes
 
-from ..parsers import (
+from .._parsers import (
     BaseParser,
     Encoder,
     _AsyncHiredisParser,
     _AsyncRESP2Parser,
     _AsyncRESP3Parser,
 )
 
@@ -74,43 +77,38 @@
 if HIREDIS_AVAILABLE:
     DefaultParser = _AsyncHiredisParser
 else:
     DefaultParser = _AsyncRESP2Parser
 
 
 class ConnectCallbackProtocol(Protocol):
-    def __call__(self, connection: "Connection"):
+    def __call__(self, connection: "AbstractConnection"):
         ...
 
 
 class AsyncConnectCallbackProtocol(Protocol):
-    async def __call__(self, connection: "Connection"):
+    async def __call__(self, connection: "AbstractConnection"):
         ...
 
 
 ConnectCallbackT = Union[ConnectCallbackProtocol, AsyncConnectCallbackProtocol]
 
 
-class Connection:
-    """Manages TCP communication to and from a Redis server"""
+class AbstractConnection:
+    """Manages communication to and from a Redis server"""
 
     __slots__ = (
         "pid",
-        "host",
-        "port",
         "db",
         "username",
         "client_name",
         "credential_provider",
         "password",
         "socket_timeout",
         "socket_connect_timeout",
-        "socket_keepalive",
-        "socket_keepalive_options",
-        "socket_type",
         "redis_connect_func",
         "retry_on_timeout",
         "retry_on_error",
         "health_check_interval",
         "next_health_check",
         "last_active_at",
         "encoder",
@@ -125,23 +123,18 @@
         "_socket_read_size",
         "__dict__",
     )
 
     def __init__(
         self,
         *,
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
         db: Union[str, int] = 0,
         password: Optional[str] = None,
         socket_timeout: Optional[float] = None,
         socket_connect_timeout: Optional[float] = None,
-        socket_keepalive: bool = False,
-        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
-        socket_type: int = 0,
         retry_on_timeout: bool = False,
         retry_on_error: Union[list, _Sentinel] = SENTINEL,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: Type[BaseParser] = DefaultParser,
         socket_read_size: int = 65536,
@@ -158,26 +151,23 @@
             raise DataError(
                 "'username' and 'password' cannot be passed along with 'credential_"
                 "provider'. Please provide only one of the following arguments: \n"
                 "1. 'password' and (optional) 'username'\n"
                 "2. 'credential_provider'"
             )
         self.pid = os.getpid()
-        self.host = host
-        self.port = int(port)
         self.db = db
         self.client_name = client_name
         self.credential_provider = credential_provider
         self.password = password
         self.username = username
         self.socket_timeout = socket_timeout
-        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
-        self.socket_keepalive = socket_keepalive
-        self.socket_keepalive_options = socket_keepalive_options or {}
-        self.socket_type = socket_type
+        if socket_connect_timeout is None:
+            socket_connect_timeout = socket_timeout
+        self.socket_connect_timeout = socket_connect_timeout
         self.retry_on_timeout = retry_on_timeout
         if retry_on_error is SENTINEL:
             retry_on_error = []
         if retry_on_timeout:
             retry_on_error.append(TimeoutError)
             retry_on_error.append(socket.timeout)
             retry_on_error.append(asyncio.TimeoutError)
@@ -190,15 +180,14 @@
                 self.retry = copy.deepcopy(retry)
             # Update the retry's supported errors with the specified errors
             self.retry.update_supported_errors(retry_on_error)
         else:
             self.retry = Retry(NoBackoff(), 0)
         self.health_check_interval = health_check_interval
         self.next_health_check: float = -1
-        self.ssl_context: Optional[RedisSSLContext] = None
         self.encoder = encoder_class(encoding, encoding_errors, decode_responses)
         self.redis_connect_func = redis_connect_func
         self._reader: Optional[asyncio.StreamReader] = None
         self._writer: Optional[asyncio.StreamWriter] = None
         self._socket_read_size = socket_read_size
         self.set_parser(parser_class)
         self._connect_callbacks: List[weakref.WeakMethod[ConnectCallbackT]] = []
@@ -214,31 +203,17 @@
                 raise ConnectionError("protocol must be either 2 or 3")
             self.protocol = protocol
 
     def __repr__(self):
         repr_args = ",".join((f"{k}={v}" for k, v in self.repr_pieces()))
         return f"{self.__class__.__name__}<{repr_args}>"
 
+    @abstractmethod
     def repr_pieces(self):
-        pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
-        if self.client_name:
-            pieces.append(("client_name", self.client_name))
-        return pieces
-
-    def __del__(self):
-        try:
-            if self.is_connected:
-                loop = asyncio.get_running_loop()
-                coro = self.disconnect()
-                if loop.is_running():
-                    loop.create_task(coro)
-                else:
-                    loop.run_until_complete(coro)
-        except Exception:
-            pass
+        pass
 
     @property
     def is_connected(self):
         return self._reader is not None and self._writer is not None
 
     def register_connect_callback(self, callback):
         self._connect_callbacks.append(weakref.WeakMethod(callback))
@@ -289,59 +264,25 @@
         # is for pubsub channel/pattern resubscription
         for ref in self._connect_callbacks:
             callback = ref()
             task = callback(self)
             if task and inspect.isawaitable(task):
                 await task
 
+    @abstractmethod
     async def _connect(self):
-        """Create a TCP socket connection"""
-        async with async_timeout(self.socket_connect_timeout):
-            reader, writer = await asyncio.open_connection(
-                host=self.host,
-                port=self.port,
-                ssl=self.ssl_context.get() if self.ssl_context else None,
-            )
-        self._reader = reader
-        self._writer = writer
-        sock = writer.transport.get_extra_info("socket")
-        if sock:
-            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-            try:
-                # TCP_KEEPALIVE
-                if self.socket_keepalive:
-                    sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-                    for k, v in self.socket_keepalive_options.items():
-                        sock.setsockopt(socket.SOL_TCP, k, v)
-
-            except (OSError, TypeError):
-                # `socket_keepalive_options` might contain invalid options
-                # causing an error. Do not leave the connection open.
-                writer.close()
-                raise
+        pass
 
-    def _error_message(self, exception):
-        # args for socket.error can either be (errno, "message")
-        # or just "message"
-        if not exception.args:
-            # asyncio has a bug where on Connection reset by peer, the
-            # exception is not instanciated, so args is empty. This is the
-            # workaround.
-            # See: https://github.com/redis/redis-py/issues/2237
-            # See: https://github.com/python/cpython/issues/94061
-            return (
-                f"Error connecting to {self.host}:{self.port}. Connection reset by peer"
-            )
-        elif len(exception.args) == 1:
-            return f"Error connecting to {self.host}:{self.port}. {exception.args[0]}."
-        else:
-            return (
-                f"Error {exception.args[0]} connecting to {self.host}:{self.port}. "
-                f"{exception.args[0]}."
-            )
+    @abstractmethod
+    def _host_error(self) -> str:
+        pass
+
+    @abstractmethod
+    def _error_message(self, exception: BaseException) -> str:
+        pass
 
     async def on_connect(self) -> None:
         """Initialize the connection, authenticate and select a database"""
         self._parser.on_connect(self)
         parser = self._parser
 
         auth_args = None
@@ -487,15 +428,19 @@
                 err_no, errmsg = "UNKNOWN", e.args[0]
             else:
                 err_no = e.args[0]
                 errmsg = e.args[1]
             raise ConnectionError(
                 f"Error {err_no} while writing to socket. {errmsg}."
             ) from e
-        except Exception:
+        except BaseException:
+            # BaseExceptions can be raised when a socket send operation is not
+            # finished, e.g. due to a timeout.  Ideally, a caller could then re-try
+            # to send un-sent data. However, the send_packed_command() API
+            # does not support it so there is no point in keeping the connection open.
             await self.disconnect(nowait=True)
             raise
 
     async def send_command(self, *args: Any, **kwargs: Any) -> None:
         """Pack and send a command to the Redis server"""
         await self.send_packed_command(
             self.pack_command(*args), check_health=kwargs.get("check_health", True)
@@ -503,26 +448,28 @@
 
     async def can_read_destructive(self):
         """Poll the socket to see if there's data that can be read."""
         try:
             return await self._parser.can_read_destructive()
         except OSError as e:
             await self.disconnect(nowait=True)
-            raise ConnectionError(
-                f"Error while reading from {self.host}:{self.port}: {e.args}"
-            )
+            host_error = self._host_error()
+            raise ConnectionError(f"Error while reading from {host_error}: {e.args}")
 
     async def read_response(
         self,
         disable_decoding: bool = False,
         timeout: Optional[float] = None,
+        *,
+        disconnect_on_error: bool = True,
         push_request: Optional[bool] = False,
     ):
         """Read the response from a previously sent command"""
         read_timeout = timeout if timeout is not None else self.socket_timeout
+        host_error = self._host_error()
         try:
             if (
                 read_timeout is not None
                 and self.protocol in ["3", 3]
                 and not HIREDIS_AVAILABLE
             ):
                 async with async_timeout(read_timeout):
@@ -540,30 +487,30 @@
                 )
             else:
                 response = await self._parser.read_response(
                     disable_decoding=disable_decoding
                 )
         except asyncio.TimeoutError:
             if timeout is not None:
-                # user requested timeout, return None
+                # user requested timeout, return None. Operation can be retried
                 return None
             # it was a self.socket_timeout error.
-            await self.disconnect(nowait=True)
-            raise TimeoutError(f"Timeout reading from {self.host}:{self.port}")
+            if disconnect_on_error:
+                await self.disconnect(nowait=True)
+            raise TimeoutError(f"Timeout reading from {host_error}")
         except OSError as e:
-            await self.disconnect(nowait=True)
-            raise ConnectionError(
-                f"Error while reading from {self.host}:{self.port} : {e.args}"
-            )
-        except asyncio.CancelledError:
-            # need this check for 3.7, where CancelledError
-            # is subclass of Exception, not BaseException
-            raise
-        except Exception:
-            await self.disconnect(nowait=True)
+            if disconnect_on_error:
+                await self.disconnect(nowait=True)
+            raise ConnectionError(f"Error while reading from {host_error} : {e.args}")
+        except BaseException:
+            # Also by default close in case of BaseException.  A lot of code
+            # relies on this behaviour when doing Command/Response pairs.
+            # See #1128.
+            if disconnect_on_error:
+                await self.disconnect(nowait=True)
             raise
 
         if self.health_check_interval:
             next_time = asyncio.get_running_loop().time() + self.health_check_interval
             self.next_health_check = next_time
 
         if isinstance(response, ResponseError):
@@ -643,34 +590,122 @@
                     buffer_length += chunklen
 
         if pieces:
             output.append(SYM_EMPTY.join(pieces))
         return output
 
 
+class Connection(AbstractConnection):
+    "Manages TCP communication to and from a Redis server"
+
+    def __init__(
+        self,
+        *,
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        **kwargs,
+    ):
+        self.host = host
+        self.port = int(port)
+        self.socket_keepalive = socket_keepalive
+        self.socket_keepalive_options = socket_keepalive_options or {}
+        self.socket_type = socket_type
+        super().__init__(**kwargs)
+
+    def repr_pieces(self):
+        pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
+        if self.client_name:
+            pieces.append(("client_name", self.client_name))
+        return pieces
+
+    def _connection_arguments(self) -> Mapping:
+        return {"host": self.host, "port": self.port}
+
+    async def _connect(self):
+        """Create a TCP socket connection"""
+        async with async_timeout(self.socket_connect_timeout):
+            reader, writer = await asyncio.open_connection(
+                **self._connection_arguments()
+            )
+        self._reader = reader
+        self._writer = writer
+        sock = writer.transport.get_extra_info("socket")
+        if sock:
+            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            try:
+                # TCP_KEEPALIVE
+                if self.socket_keepalive:
+                    sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+                    for k, v in self.socket_keepalive_options.items():
+                        sock.setsockopt(socket.SOL_TCP, k, v)
+
+            except (OSError, TypeError):
+                # `socket_keepalive_options` might contain invalid options
+                # causing an error. Do not leave the connection open.
+                writer.close()
+                raise
+
+    def _host_error(self) -> str:
+        return f"{self.host}:{self.port}"
+
+    def _error_message(self, exception: BaseException) -> str:
+        # args for socket.error can either be (errno, "message")
+        # or just "message"
+
+        host_error = self._host_error()
+
+        if not exception.args:
+            # asyncio has a bug where on Connection reset by peer, the
+            # exception is not instanciated, so args is empty. This is the
+            # workaround.
+            # See: https://github.com/redis/redis-py/issues/2237
+            # See: https://github.com/python/cpython/issues/94061
+            return f"Error connecting to {host_error}. Connection reset by peer"
+        elif len(exception.args) == 1:
+            return f"Error connecting to {host_error}. {exception.args[0]}."
+        else:
+            return (
+                f"Error {exception.args[0]} connecting to {host_error}. "
+                f"{exception.args[0]}."
+            )
+
+
 class SSLConnection(Connection):
+    """Manages SSL connections to and from the Redis server(s).
+    This class extends the Connection class, adding SSL functionality, and making
+    use of ssl.SSLContext (https://docs.python.org/3/library/ssl.html#ssl.SSLContext)
+    """
+
     def __init__(
         self,
         ssl_keyfile: Optional[str] = None,
         ssl_certfile: Optional[str] = None,
         ssl_cert_reqs: str = "required",
         ssl_ca_certs: Optional[str] = None,
         ssl_ca_data: Optional[str] = None,
         ssl_check_hostname: bool = False,
         **kwargs,
     ):
-        super().__init__(**kwargs)
         self.ssl_context: RedisSSLContext = RedisSSLContext(
             keyfile=ssl_keyfile,
             certfile=ssl_certfile,
             cert_reqs=ssl_cert_reqs,
             ca_certs=ssl_ca_certs,
             ca_data=ssl_ca_data,
             check_hostname=ssl_check_hostname,
         )
+        super().__init__(**kwargs)
+
+    def _connection_arguments(self) -> Mapping:
+        kwargs = super()._connection_arguments()
+        kwargs["ssl"] = self.ssl_context.get()
+        return kwargs
 
     @property
     def keyfile(self):
         return self.ssl_context.keyfile
 
     @property
     def certfile(self):
@@ -742,108 +777,49 @@
                 context.load_cert_chain(certfile=self.certfile, keyfile=self.keyfile)
             if self.ca_certs or self.ca_data:
                 context.load_verify_locations(cafile=self.ca_certs, cadata=self.ca_data)
             self.context = context
         return self.context
 
 
-class UnixDomainSocketConnection(Connection):  # lgtm [py/missing-call-to-init]
-    def __init__(
-        self,
-        *,
-        path: str = "",
-        db: Union[str, int] = 0,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        retry_on_timeout: bool = False,
-        retry_on_error: Union[list, _Sentinel] = SENTINEL,
-        parser_class: Type[BaseParser] = DefaultParser,
-        socket_read_size: int = 65536,
-        health_check_interval: float = 0.0,
-        client_name: str = None,
-        retry: Optional[Retry] = None,
-        redis_connect_func=None,
-        credential_provider: Optional[CredentialProvider] = None,
-    ):
-        """
-        Initialize a new UnixDomainSocketConnection.
-        To specify a retry policy, first set `retry_on_timeout` to `True`
-        then set `retry` to a valid `Retry` object
-        """
-        if (username or password) and credential_provider is not None:
-            raise DataError(
-                "'username' and 'password' cannot be passed along with 'credential_"
-                "provider'. Please provide only one of the following arguments: \n"
-                "1. 'password' and (optional) 'username'\n"
-                "2. 'credential_provider'"
-            )
-        self.pid = os.getpid()
+class UnixDomainSocketConnection(AbstractConnection):
+    "Manages UDS communication to and from a Redis server"
+
+    def __init__(self, *, path: str = "", **kwargs):
         self.path = path
-        self.db = db
-        self.client_name = client_name
-        self.credential_provider = credential_provider
-        self.password = password
-        self.username = username
-        self.socket_timeout = socket_timeout
-        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
-        self.retry_on_timeout = retry_on_timeout
-        if retry_on_error is SENTINEL:
-            retry_on_error = []
-        if retry_on_timeout:
-            retry_on_error.append(TimeoutError)
-        self.retry_on_error = retry_on_error
-        if retry_on_error:
-            if retry is None:
-                self.retry = Retry(NoBackoff(), 1)
-            else:
-                # deep-copy the Retry object as it is mutable
-                self.retry = copy.deepcopy(retry)
-            # Update the retry's supported errors with the specified errors
-            self.retry.update_supported_errors(retry_on_error)
-        else:
-            self.retry = Retry(NoBackoff(), 0)
-        self.health_check_interval = health_check_interval
-        self.next_health_check = -1
-        self.redis_connect_func = redis_connect_func
-        self.encoder = Encoder(encoding, encoding_errors, decode_responses)
-        self._sock = None
-        self._reader = None
-        self._writer = None
-        self._socket_read_size = socket_read_size
-        self.set_parser(parser_class)
-        self._connect_callbacks = []
-        self._buffer_cutoff = 6000
+        super().__init__(**kwargs)
 
     def repr_pieces(self) -> Iterable[Tuple[str, Union[str, int]]]:
         pieces = [("path", self.path), ("db", self.db)]
         if self.client_name:
             pieces.append(("client_name", self.client_name))
         return pieces
 
     async def _connect(self):
         async with async_timeout(self.socket_connect_timeout):
             reader, writer = await asyncio.open_unix_connection(path=self.path)
         self._reader = reader
         self._writer = writer
         await self.on_connect()
 
-    def _error_message(self, exception):
+    def _host_error(self) -> str:
+        return self.path
+
+    def _error_message(self, exception: BaseException) -> str:
         # args for socket.error can either be (errno, "message")
         # or just "message"
+        host_error = self._host_error()
         if len(exception.args) == 1:
-            return f"Error connecting to unix socket: {self.path}. {exception.args[0]}."
+            return (
+                f"Error connecting to unix socket: {host_error}. {exception.args[0]}."
+            )
         else:
             return (
                 f"Error {exception.args[0]} connecting to unix socket: "
-                f"{self.path}. {exception.args[1]}."
+                f"{host_error}. {exception.args[1]}."
             )
 
 
 FALSE_STRINGS = ("0", "F", "FALSE", "N", "NO")
 
 
 def to_bool(value) -> Optional[bool]:
@@ -867,15 +843,15 @@
     }
 )
 
 
 class ConnectKwargs(TypedDict, total=False):
     username: str
     password: str
-    connection_class: Type[Connection]
+    connection_class: Type[AbstractConnection]
     host: str
     port: int
     db: int
     path: str
 
 
 def parse_url(url: str) -> ConnectKwargs:
@@ -989,15 +965,15 @@
         """
         url_options = parse_url(url)
         kwargs.update(url_options)
         return cls(**kwargs)
 
     def __init__(
         self,
-        connection_class: Type[Connection] = Connection,
+        connection_class: Type[AbstractConnection] = Connection,
         max_connections: Optional[int] = None,
         **connection_kwargs,
     ):
         max_connections = max_connections or 2**31
         if not isinstance(max_connections, int) or max_connections < 0:
             raise ValueError('"max_connections" must be a positive integer')
 
@@ -1012,16 +988,16 @@
         # to acquire the lock will reset the data structures and lock
         # object of this pool. subsequent threads acquiring this lock
         # will notice the first thread already did the work and simply
         # release the lock.
         self._fork_lock = threading.Lock()
         self._lock = asyncio.Lock()
         self._created_connections: int
-        self._available_connections: List[Connection]
-        self._in_use_connections: Set[Connection]
+        self._available_connections: List[AbstractConnection]
+        self._in_use_connections: Set[AbstractConnection]
         self.reset()  # lgtm [py/init-calls-subclass]
         self.encoder_class = self.connection_kwargs.get("encoder_class", Encoder)
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}"
             f"<{self.connection_class(**self.connection_kwargs)!r}>"
@@ -1136,15 +1112,15 @@
     def make_connection(self):
         """Create a new connection"""
         if self._created_connections >= self.max_connections:
             raise ConnectionError("Too many connections")
         self._created_connections += 1
         return self.connection_class(**self.connection_kwargs)
 
-    async def release(self, connection: Connection):
+    async def release(self, connection: AbstractConnection):
         """Releases the connection back to the pool"""
         self._checkpid()
         async with self._lock:
             try:
                 self._in_use_connections.remove(connection)
             except KeyError:
                 # Gracefully fail when a connection is returned to this pool
@@ -1157,29 +1133,29 @@
                 # pool doesn't own this connection. do not add it back
                 # to the pool and decrement the count so that another
                 # connection can take its place if needed
                 self._created_connections -= 1
                 await connection.disconnect()
                 return
 
-    def owns_connection(self, connection: Connection):
+    def owns_connection(self, connection: AbstractConnection):
         return connection.pid == self.pid
 
     async def disconnect(self, inuse_connections: bool = True):
         """
         Disconnects connections in the pool
 
         If ``inuse_connections`` is True, disconnect connections that are
         current in use, potentially by other tasks. Otherwise only disconnect
         connections that are idle in the pool.
         """
         self._checkpid()
         async with self._lock:
             if inuse_connections:
-                connections: Iterable[Connection] = chain(
+                connections: Iterable[AbstractConnection] = chain(
                     self._available_connections, self._in_use_connections
                 )
             else:
                 connections = self._available_connections
             resp = await asyncio.gather(
                 *(connection.disconnect() for connection in connections),
                 return_exceptions=True,
@@ -1229,22 +1205,22 @@
         >>> pool = BlockingConnectionPool(timeout=5)
     """
 
     def __init__(
         self,
         max_connections: int = 50,
         timeout: Optional[int] = 20,
-        connection_class: Type[Connection] = Connection,
+        connection_class: Type[AbstractConnection] = Connection,
         queue_class: Type[asyncio.Queue] = asyncio.LifoQueue,
         **connection_kwargs,
     ):
 
         self.queue_class = queue_class
         self.timeout = timeout
-        self._connections: List[Connection]
+        self._connections: List[AbstractConnection]
         super().__init__(
             connection_class=connection_class,
             max_connections=max_connections,
             **connection_kwargs,
         )
 
     def reset(self):
@@ -1326,15 +1302,15 @@
         except BaseException:
             # release the connection back to the pool so that we don't leak it
             await self.release(connection)
             raise
 
         return connection
 
-    async def release(self, connection: Connection):
+    async def release(self, connection: AbstractConnection):
         """Releases the connection back to the pool."""
         # Make sure we haven't changed process.
         self._checkpid()
         if not self.owns_connection(connection):
             # pool doesn't own this connection. do not add it back
             # to the pool. instead add a None value which is a placeholder
             # that will cause the pool to recreate the connection if
```

### Comparing `redis-5.0.0rc1/redis/asyncio/lock.py` & `redis-5.0.0rc2/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/asyncio/retry.py` & `redis-5.0.0rc2/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/asyncio/sentinel.py` & `redis-5.0.0rc2/redis/asyncio/sentinel.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,22 @@
             lambda error: asyncio.sleep(0),
         )
 
     async def read_response(
         self,
         disable_decoding: bool = False,
         timeout: Optional[float] = None,
+        *,
+        disconnect_on_error: Optional[float] = True,
     ):
         try:
             return await super().read_response(
                 disable_decoding=disable_decoding,
                 timeout=timeout,
+                disconnect_on_error=disconnect_on_error,
             )
         except ReadOnlyError:
             if self.connection_pool.is_master:
                 # When talking to a master, a ReadOnlyError when likely
                 # indicates that the previous master that we're still connected
                 # to has been demoted to a slave and there's a new master.
                 # calling disconnect will force the connection to re-query
@@ -216,21 +219,21 @@
                node at random, rather than across the entire sentinel cluster.
         """
         once = bool(kwargs.get("once", False))
         if "once" in kwargs.keys():
             kwargs.pop("once")
 
         if once:
+            await random.choice(self.sentinels).execute_command(*args, **kwargs)
+        else:
             tasks = [
                 asyncio.Task(sentinel.execute_command(*args, **kwargs))
                 for sentinel in self.sentinels
             ]
             await asyncio.gather(*tasks)
-        else:
-            await random.choice(self.sentinels).execute_command(*args, **kwargs)
         return True
 
     def __repr__(self):
         sentinel_addresses = []
         for sentinel in self.sentinels:
             sentinel_addresses.append(
                 f"{sentinel.connection_pool.connection_kwargs['host']}:"
@@ -250,28 +253,34 @@
         """
         Asks sentinel servers for the Redis master's address corresponding
         to the service labeled ``service_name``.
 
         Returns a pair (address, port) or raises MasterNotFoundError if no
         master is found.
         """
+        collected_errors = list()
         for sentinel_no, sentinel in enumerate(self.sentinels):
             try:
                 masters = await sentinel.sentinel_masters()
-            except (ConnectionError, TimeoutError):
+            except (ConnectionError, TimeoutError) as e:
+                collected_errors.append(f"{sentinel} - {e!r}")
                 continue
             state = masters.get(service_name)
             if state and self.check_master_state(state, service_name):
                 # Put this sentinel at the top of the list
                 self.sentinels[0], self.sentinels[sentinel_no] = (
                     sentinel,
                     self.sentinels[0],
                 )
                 return state["ip"], state["port"]
-        raise MasterNotFoundError(f"No master found for {service_name!r}")
+
+        error_info = ""
+        if len(collected_errors) > 0:
+            error_info = f" : {', '.join(collected_errors)}"
+        raise MasterNotFoundError(f"No master found for {service_name!r}{error_info}")
 
     def filter_slaves(
         self, slaves: Iterable[Mapping]
     ) -> Sequence[Tuple[EncodableT, EncodableT]]:
         """Remove slaves that are in an ODOWN or SDOWN state"""
         slaves_alive = []
         for slave in slaves:
```

### Comparing `redis-5.0.0rc1/redis/asyncio/utils.py` & `redis-5.0.0rc2/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/backoff.py` & `redis-5.0.0rc2/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/client.py` & `redis-5.0.0rc2/redis/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import copy
-import datetime
 import re
 import threading
 import time
 import warnings
 from itertools import chain
 from typing import Optional
 
+from redis._parsers.helpers import (
+    _RedisCallbacks,
+    _RedisCallbacksRESP2,
+    _RedisCallbacksRESP3,
+    bool_ok,
+)
 from redis.commands import (
     CoreCommands,
     RedisModuleCommands,
     SentinelCommands,
     list_or_args,
 )
 from redis.connection import ConnectionPool, SSLConnection, UnixDomainSocketConnection
 from redis.credentials import CredentialProvider
 from redis.exceptions import (
     ConnectionError,
     ExecAbortError,
-    ModuleError,
     PubSubError,
     RedisError,
     ResponseError,
     TimeoutError,
     WatchError,
 )
 from redis.lock import Lock
@@ -32,29 +36,14 @@
 SYM_EMPTY = b""
 EMPTY_RESPONSE = "EMPTY_RESPONSE"
 
 # some responses (ie. dump) are binary, and just meant to never be decoded
 NEVER_DECODE = "NEVER_DECODE"
 
 
-def timestamp_to_datetime(response):
-    "Converts a unix timestamp to a Python datetime object"
-    if not response:
-        return None
-    try:
-        response = int(response)
-    except ValueError:
-        return None
-    return datetime.datetime.fromtimestamp(response)
-
-
-def string_keys_to_dict(key_string, callback):
-    return dict.fromkeys(key_string.split(), callback)
-
-
 class CaseInsensitiveDict(dict):
     "Case insensitive dict implementation. Assumes string keys only."
 
     def __init__(self, data):
         for k, v in data.items():
             self[k.upper()] = v
 
@@ -74,856 +63,19 @@
         super().__setitem__(k.upper(), v)
 
     def update(self, data):
         data = CaseInsensitiveDict(data)
         super().update(data)
 
 
-def parse_debug_object(response):
-    "Parse the results of Redis's DEBUG OBJECT command into a Python dict"
-    # The 'type' of the object is the first item in the response, but isn't
-    # prefixed with a name
-    response = str_if_bytes(response)
-    response = "type:" + response
-    response = dict(kv.split(":") for kv in response.split())
-
-    # parse some expected int values from the string response
-    # note: this cmd isn't spec'd so these may not appear in all redis versions
-    int_fields = ("refcount", "serializedlength", "lru", "lru_seconds_idle")
-    for field in int_fields:
-        if field in response:
-            response[field] = int(response[field])
-
-    return response
-
-
-def parse_object(response, infotype):
-    """Parse the results of an OBJECT command"""
-    if infotype in ("idletime", "refcount"):
-        return int_or_none(response)
-    return response
-
-
-def parse_info(response):
-    """Parse the result of Redis's INFO command into a Python dict"""
-    info = {}
-    response = str_if_bytes(response)
-
-    def get_value(value):
-        if "," not in value or "=" not in value:
-            try:
-                if "." in value:
-                    return float(value)
-                else:
-                    return int(value)
-            except ValueError:
-                return value
-        else:
-            sub_dict = {}
-            for item in value.split(","):
-                k, v = item.rsplit("=", 1)
-                sub_dict[k] = get_value(v)
-            return sub_dict
-
-    for line in response.splitlines():
-        if line and not line.startswith("#"):
-            if line.find(":") != -1:
-                # Split, the info fields keys and values.
-                # Note that the value may contain ':'. but the 'host:'
-                # pseudo-command is the only case where the key contains ':'
-                key, value = line.split(":", 1)
-                if key == "cmdstat_host":
-                    key, value = line.rsplit(":", 1)
-
-                if key == "module":
-                    # Hardcode a list for key 'modules' since there could be
-                    # multiple lines that started with 'module'
-                    info.setdefault("modules", []).append(get_value(value))
-                else:
-                    info[key] = get_value(value)
-            else:
-                # if the line isn't splittable, append it to the "__raw__" key
-                info.setdefault("__raw__", []).append(line)
-
-    return info
-
-
-def parse_memory_stats(response, **kwargs):
-    """Parse the results of MEMORY STATS"""
-    stats = pairs_to_dict(response, decode_keys=True, decode_string_values=True)
-    for key, value in stats.items():
-        if key.startswith("db."):
-            stats[key] = pairs_to_dict(
-                value, decode_keys=True, decode_string_values=True
-            )
-    return stats
-
-
-SENTINEL_STATE_TYPES = {
-    "can-failover-its-master": int,
-    "config-epoch": int,
-    "down-after-milliseconds": int,
-    "failover-timeout": int,
-    "info-refresh": int,
-    "last-hello-message": int,
-    "last-ok-ping-reply": int,
-    "last-ping-reply": int,
-    "last-ping-sent": int,
-    "master-link-down-time": int,
-    "master-port": int,
-    "num-other-sentinels": int,
-    "num-slaves": int,
-    "o-down-time": int,
-    "pending-commands": int,
-    "parallel-syncs": int,
-    "port": int,
-    "quorum": int,
-    "role-reported-time": int,
-    "s-down-time": int,
-    "slave-priority": int,
-    "slave-repl-offset": int,
-    "voted-leader-epoch": int,
-}
-
-
-def parse_sentinel_state(item):
-    result = pairs_to_dict_typed(item, SENTINEL_STATE_TYPES)
-    flags = set(result["flags"].split(","))
-    for name, flag in (
-        ("is_master", "master"),
-        ("is_slave", "slave"),
-        ("is_sdown", "s_down"),
-        ("is_odown", "o_down"),
-        ("is_sentinel", "sentinel"),
-        ("is_disconnected", "disconnected"),
-        ("is_master_down", "master_down"),
-    ):
-        result[name] = flag in flags
-    return result
-
-
-def parse_sentinel_master(response):
-    return parse_sentinel_state(map(str_if_bytes, response))
-
-
-def parse_sentinel_masters(response):
-    result = {}
-    for item in response:
-        state = parse_sentinel_state(map(str_if_bytes, item))
-        result[state["name"]] = state
-    return result
-
-
-def parse_sentinel_slaves_and_sentinels(response):
-    return [parse_sentinel_state(map(str_if_bytes, item)) for item in response]
-
-
-def parse_sentinel_get_master(response):
-    return response and (response[0], int(response[1])) or None
-
-
-def pairs_to_dict(response, decode_keys=False, decode_string_values=False):
-    """Create a dict given a list of key/value pairs"""
-    if response is None:
-        return {}
-    if decode_keys or decode_string_values:
-        # the iter form is faster, but I don't know how to make that work
-        # with a str_if_bytes() map
-        keys = response[::2]
-        if decode_keys:
-            keys = map(str_if_bytes, keys)
-        values = response[1::2]
-        if decode_string_values:
-            values = map(str_if_bytes, values)
-        return dict(zip(keys, values))
-    else:
-        it = iter(response)
-        return dict(zip(it, it))
-
-
-def pairs_to_dict_typed(response, type_info):
-    it = iter(response)
-    result = {}
-    for key, value in zip(it, it):
-        if key in type_info:
-            try:
-                value = type_info[key](value)
-            except Exception:
-                # if for some reason the value can't be coerced, just use
-                # the string value
-                pass
-        result[key] = value
-    return result
-
-
-def zset_score_pairs(response, **options):
-    """
-    If ``withscores`` is specified in the options, return the response as
-    a list of (value, score) pairs
-    """
-    if not response or not options.get("withscores"):
-        return response
-    score_cast_func = options.get("score_cast_func", float)
-    it = iter(response)
-    return list(zip(it, map(score_cast_func, it)))
-
-
-def sort_return_tuples(response, **options):
-    """
-    If ``groups`` is specified, return the response as a list of
-    n-element tuples with n being the value found in options['groups']
-    """
-    if not response or not options.get("groups"):
-        return response
-    n = options["groups"]
-    return list(zip(*[response[i::n] for i in range(n)]))
-
-
-def int_or_none(response):
-    if response is None:
-        return None
-    return int(response)
-
-
-def parse_stream_list(response):
-    if response is None:
-        return None
-    data = []
-    for r in response:
-        if r is not None:
-            data.append((r[0], pairs_to_dict(r[1])))
-        else:
-            data.append((None, None))
-    return data
-
-
-def pairs_to_dict_with_str_keys(response):
-    return pairs_to_dict(response, decode_keys=True)
-
-
-def parse_list_of_dicts(response):
-    return list(map(pairs_to_dict_with_str_keys, response))
-
-
-def parse_xclaim(response, **options):
-    if options.get("parse_justid", False):
-        return response
-    return parse_stream_list(response)
-
-
-def parse_xautoclaim(response, **options):
-    if options.get("parse_justid", False):
-        return response[1]
-    response[1] = parse_stream_list(response[1])
-    return response
-
-
-def parse_xinfo_stream(response, **options):
-    if isinstance(response, list):
-        data = pairs_to_dict(response, decode_keys=True)
-    else:
-        data = {str_if_bytes(k): v for k, v in response.items()}
-    if not options.get("full", False):
-        first = data["first-entry"]
-        if first is not None:
-            data["first-entry"] = (first[0], pairs_to_dict(first[1]))
-        last = data["last-entry"]
-        if last is not None:
-            data["last-entry"] = (last[0], pairs_to_dict(last[1]))
-    else:
-        data["entries"] = {_id: pairs_to_dict(entry) for _id, entry in data["entries"]}
-        if isinstance(data["groups"][0], list):
-            data["groups"] = [
-                pairs_to_dict(group, decode_keys=True) for group in data["groups"]
-            ]
-        else:
-            data["groups"] = [
-                {str_if_bytes(k): v for k, v in group.items()}
-                for group in data["groups"]
-            ]
-    return data
-
-
-def parse_xread(response):
-    if response is None:
-        return []
-    return [[r[0], parse_stream_list(r[1])] for r in response]
-
-
-def parse_xread_resp3(response):
-    if response is None:
-        return {}
-    return {key: [parse_stream_list(value)] for key, value in response.items()}
-
-
-def parse_xpending(response, **options):
-    if options.get("parse_detail", False):
-        return parse_xpending_range(response)
-    consumers = [{"name": n, "pending": int(p)} for n, p in response[3] or []]
-    return {
-        "pending": response[0],
-        "min": response[1],
-        "max": response[2],
-        "consumers": consumers,
-    }
-
-
-def parse_xpending_range(response):
-    k = ("message_id", "consumer", "time_since_delivered", "times_delivered")
-    return [dict(zip(k, r)) for r in response]
-
-
-def float_or_none(response):
-    if response is None:
-        return None
-    return float(response)
-
-
-def bool_ok(response):
-    return str_if_bytes(response) == "OK"
-
-
-def parse_zadd(response, **options):
-    if response is None:
-        return None
-    if options.get("as_score"):
-        return float(response)
-    return int(response)
-
-
-def parse_client_list(response, **options):
-    clients = []
-    for c in str_if_bytes(response).splitlines():
-        # Values might contain '='
-        clients.append(dict(pair.split("=", 1) for pair in c.split(" ")))
-    return clients
-
-
-def parse_config_get(response, **options):
-    response = [str_if_bytes(i) if i is not None else None for i in response]
-    return response and pairs_to_dict(response) or {}
-
-
-def parse_scan(response, **options):
-    cursor, r = response
-    return int(cursor), r
-
-
-def parse_hscan(response, **options):
-    cursor, r = response
-    return int(cursor), r and pairs_to_dict(r) or {}
-
-
-def parse_zscan(response, **options):
-    score_cast_func = options.get("score_cast_func", float)
-    cursor, r = response
-    it = iter(r)
-    return int(cursor), list(zip(it, map(score_cast_func, it)))
-
-
-def parse_zmscore(response, **options):
-    # zmscore: list of scores (double precision floating point number) or nil
-    return [float(score) if score is not None else None for score in response]
-
-
-def parse_slowlog_get(response, **options):
-    space = " " if options.get("decode_responses", False) else b" "
-
-    def parse_item(item):
-        result = {"id": item[0], "start_time": int(item[1]), "duration": int(item[2])}
-        # Redis Enterprise injects another entry at index [3], which has
-        # the complexity info (i.e. the value N in case the command has
-        # an O(N) complexity) instead of the command.
-        if isinstance(item[3], list):
-            result["command"] = space.join(item[3])
-        else:
-            result["complexity"] = item[3]
-            result["command"] = space.join(item[4])
-        return result
-
-    return [parse_item(item) for item in response]
-
-
-def parse_stralgo(response, **options):
-    """
-    Parse the response from `STRALGO` command.
-    Without modifiers the returned value is string.
-    When LEN is given the command returns the length of the result
-    (i.e integer).
-    When IDX is given the command returns a dictionary with the LCS
-    length and all the ranges in both the strings, start and end
-    offset for each string, where there are matches.
-    When WITHMATCHLEN is given, each array representing a match will
-    also have the length of the match at the beginning of the array.
-    """
-    if options.get("len", False):
-        return int(response)
-    if options.get("idx", False):
-        if options.get("withmatchlen", False):
-            matches = [
-                [(int(match[-1]))] + list(map(tuple, match[:-1]))
-                for match in response[1]
-            ]
-        else:
-            matches = [list(map(tuple, match)) for match in response[1]]
-        return {
-            str_if_bytes(response[0]): matches,
-            str_if_bytes(response[2]): int(response[3]),
-        }
-    return str_if_bytes(response)
-
-
-def parse_cluster_info(response, **options):
-    response = str_if_bytes(response)
-    return dict(line.split(":") for line in response.splitlines() if line)
-
-
-def _parse_node_line(line):
-    line_items = line.split(" ")
-    node_id, addr, flags, master_id, ping, pong, epoch, connected = line.split(" ")[:8]
-    addr = addr.split("@")[0]
-    node_dict = {
-        "node_id": node_id,
-        "flags": flags,
-        "master_id": master_id,
-        "last_ping_sent": ping,
-        "last_pong_rcvd": pong,
-        "epoch": epoch,
-        "slots": [],
-        "migrations": [],
-        "connected": True if connected == "connected" else False,
-    }
-    if len(line_items) >= 9:
-        slots, migrations = _parse_slots(line_items[8:])
-        node_dict["slots"], node_dict["migrations"] = slots, migrations
-    return addr, node_dict
-
-
-def _parse_slots(slot_ranges):
-    slots, migrations = [], []
-    for s_range in slot_ranges:
-        if "->-" in s_range:
-            slot_id, dst_node_id = s_range[1:-1].split("->-", 1)
-            migrations.append(
-                {"slot": slot_id, "node_id": dst_node_id, "state": "migrating"}
-            )
-        elif "-<-" in s_range:
-            slot_id, src_node_id = s_range[1:-1].split("-<-", 1)
-            migrations.append(
-                {"slot": slot_id, "node_id": src_node_id, "state": "importing"}
-            )
-        else:
-            s_range = [sl for sl in s_range.split("-")]
-            slots.append(s_range)
-
-    return slots, migrations
-
-
-def parse_cluster_nodes(response, **options):
-    """
-    @see: https://redis.io/commands/cluster-nodes  # string / bytes
-    @see: https://redis.io/commands/cluster-replicas # list of string / bytes
-    """
-    if isinstance(response, (str, bytes)):
-        response = response.splitlines()
-    return dict(_parse_node_line(str_if_bytes(node)) for node in response)
-
-
-def parse_geosearch_generic(response, **options):
-    """
-    Parse the response of 'GEOSEARCH', GEORADIUS' and 'GEORADIUSBYMEMBER'
-    commands according to 'withdist', 'withhash' and 'withcoord' labels.
-    """
-    if options["store"] or options["store_dist"]:
-        # `store` and `store_dist` cant be combined
-        # with other command arguments.
-        # relevant to 'GEORADIUS' and 'GEORADIUSBYMEMBER'
-        return response
-
-    if type(response) != list:
-        response_list = [response]
-    else:
-        response_list = response
-
-    if not options["withdist"] and not options["withcoord"] and not options["withhash"]:
-        # just a bunch of places
-        return response_list
-
-    cast = {
-        "withdist": float,
-        "withcoord": lambda ll: (float(ll[0]), float(ll[1])),
-        "withhash": int,
-    }
-
-    # zip all output results with each casting function to get
-    # the properly native Python value.
-    f = [lambda x: x]
-    f += [cast[o] for o in ["withdist", "withhash", "withcoord"] if options[o]]
-    return [list(map(lambda fv: fv[0](fv[1]), zip(f, r))) for r in response_list]
-
-
-def parse_command(response, **options):
-    commands = {}
-    for command in response:
-        cmd_dict = {}
-        cmd_name = str_if_bytes(command[0])
-        cmd_dict["name"] = cmd_name
-        cmd_dict["arity"] = int(command[1])
-        cmd_dict["flags"] = [str_if_bytes(flag) for flag in command[2]]
-        cmd_dict["first_key_pos"] = command[3]
-        cmd_dict["last_key_pos"] = command[4]
-        cmd_dict["step_count"] = command[5]
-        if len(command) > 7:
-            cmd_dict["tips"] = command[7]
-            cmd_dict["key_specifications"] = command[8]
-            cmd_dict["subcommands"] = command[9]
-        commands[cmd_name] = cmd_dict
-    return commands
-
-
-def parse_command_resp3(response, **options):
-    commands = {}
-    for command in response:
-        cmd_dict = {}
-        cmd_name = str_if_bytes(command[0])
-        cmd_dict["name"] = cmd_name
-        cmd_dict["arity"] = command[1]
-        cmd_dict["flags"] = {str_if_bytes(flag) for flag in command[2]}
-        cmd_dict["first_key_pos"] = command[3]
-        cmd_dict["last_key_pos"] = command[4]
-        cmd_dict["step_count"] = command[5]
-        cmd_dict["acl_categories"] = command[6]
-        if len(command) > 7:
-            cmd_dict["tips"] = command[7]
-            cmd_dict["key_specifications"] = command[8]
-            cmd_dict["subcommands"] = command[9]
-
-        commands[cmd_name] = cmd_dict
-    return commands
-
-
-def parse_pubsub_numsub(response, **options):
-    return list(zip(response[0::2], response[1::2]))
-
-
-def parse_client_kill(response, **options):
-    if isinstance(response, int):
-        return response
-    return str_if_bytes(response) == "OK"
-
-
-def parse_acl_getuser(response, **options):
-    if response is None:
-        return None
-    if isinstance(response, list):
-        data = pairs_to_dict(response, decode_keys=True)
-    else:
-        data = {str_if_bytes(key): value for key, value in response.items()}
-
-    # convert everything but user-defined data in 'keys' to native strings
-    data["flags"] = list(map(str_if_bytes, data["flags"]))
-    data["passwords"] = list(map(str_if_bytes, data["passwords"]))
-    data["commands"] = str_if_bytes(data["commands"])
-    if isinstance(data["keys"], str) or isinstance(data["keys"], bytes):
-        data["keys"] = list(str_if_bytes(data["keys"]).split(" "))
-    if data["keys"] == [""]:
-        data["keys"] = []
-    if "channels" in data:
-        if isinstance(data["channels"], str) or isinstance(data["channels"], bytes):
-            data["channels"] = list(str_if_bytes(data["channels"]).split(" "))
-        if data["channels"] == [""]:
-            data["channels"] = []
-    if "selectors" in data:
-        if data["selectors"] != [] and isinstance(data["selectors"][0], list):
-            data["selectors"] = [
-                list(map(str_if_bytes, selector)) for selector in data["selectors"]
-            ]
-        elif data["selectors"] != []:
-            data["selectors"] = [
-                {str_if_bytes(k): str_if_bytes(v) for k, v in selector.items()}
-                for selector in data["selectors"]
-            ]
-
-    # split 'commands' into separate 'categories' and 'commands' lists
-    commands, categories = [], []
-    for command in data["commands"].split(" "):
-        categories.append(command) if "@" in command else commands.append(command)
-
-    data["commands"] = commands
-    data["categories"] = categories
-    data["enabled"] = "on" in data["flags"]
-    return data
-
-
-def parse_acl_log(response, **options):
-    if response is None:
-        return None
-    if isinstance(response, list):
-        data = []
-        for log in response:
-            log_data = pairs_to_dict(log, True, True)
-            client_info = log_data.get("client-info", "")
-            log_data["client-info"] = parse_client_info(client_info)
-
-            # float() is lossy comparing to the "double" in C
-            log_data["age-seconds"] = float(log_data["age-seconds"])
-            data.append(log_data)
-    else:
-        data = bool_ok(response)
-    return data
-
-
-def parse_client_info(value):
-    """
-    Parsing client-info in ACL Log in following format.
-    "key1=value1 key2=value2 key3=value3"
-    """
-    client_info = {}
-    infos = str_if_bytes(value).split(" ")
-    for info in infos:
-        key, value = info.split("=")
-        client_info[key] = value
-
-    # Those fields are defined as int in networking.c
-    for int_key in {
-        "id",
-        "age",
-        "idle",
-        "db",
-        "sub",
-        "psub",
-        "multi",
-        "qbuf",
-        "qbuf-free",
-        "obl",
-        "argv-mem",
-        "oll",
-        "omem",
-        "tot-mem",
-    }:
-        client_info[int_key] = int(client_info[int_key])
-    return client_info
-
-
-def parse_module_result(response):
-    if isinstance(response, ModuleError):
-        raise response
-    return True
-
-
-def parse_set_result(response, **options):
-    """
-    Handle SET result since GET argument is available since Redis 6.2.
-    Parsing SET result into:
-    - BOOL
-    - String when GET argument is used
-    """
-    if options.get("get"):
-        # Redis will return a getCommand result.
-        # See `setGenericCommand` in t_string.c
-        return response
-    return response and str_if_bytes(response) == "OK"
-
-
 class AbstractRedis:
-    RESPONSE_CALLBACKS = {
-        **string_keys_to_dict("EXPIRE EXPIREAT PEXPIRE PEXPIREAT AUTH", bool),
-        **string_keys_to_dict("EXISTS", int),
-        **string_keys_to_dict("INCRBYFLOAT HINCRBYFLOAT", float),
-        **string_keys_to_dict("READONLY MSET", bool_ok),
-        "CLUSTER DELSLOTS": bool_ok,
-        "CLUSTER ADDSLOTS": bool_ok,
-        "COMMAND": parse_command,
-        "INFO": parse_info,
-        "SET": parse_set_result,
-        "CLIENT ID": int,
-        "CLIENT KILL": parse_client_kill,
-        "CLIENT LIST": parse_client_list,
-        "CLIENT INFO": parse_client_info,
-        "CLIENT SETNAME": bool_ok,
-        "CLIENT TRACKINGINFO": lambda r: list(map(str_if_bytes, r)),
-        "LASTSAVE": timestamp_to_datetime,
-        "RESET": str_if_bytes,
-        "SLOWLOG GET": parse_slowlog_get,
-        "TIME": lambda x: (int(x[0]), int(x[1])),
-        **string_keys_to_dict("BLPOP BRPOP", lambda r: r and tuple(r) or None),
-        "SCAN": parse_scan,
-        "CLIENT GETNAME": str_if_bytes,
-        "SSCAN": parse_scan,
-        "ACL LOG": parse_acl_log,
-        "ACL WHOAMI": str_if_bytes,
-        "ACL GENPASS": str_if_bytes,
-        "ACL CAT": lambda r: list(map(str_if_bytes, r)),
-        "HSCAN": parse_hscan,
-        "ZSCAN": parse_zscan,
-        **string_keys_to_dict(
-            "BZPOPMIN BZPOPMAX", lambda r: r and (r[0], r[1], float(r[2])) or None
-        ),
-        "CLUSTER COUNT-FAILURE-REPORTS": lambda x: int(x),
-        "CLUSTER COUNTKEYSINSLOT": lambda x: int(x),
-        "CLUSTER FAILOVER": bool_ok,
-        "CLUSTER FORGET": bool_ok,
-        "CLUSTER INFO": parse_cluster_info,
-        "CLUSTER KEYSLOT": lambda x: int(x),
-        "CLUSTER MEET": bool_ok,
-        "CLUSTER NODES": parse_cluster_nodes,
-        "CLUSTER REPLICATE": bool_ok,
-        "CLUSTER RESET": bool_ok,
-        "CLUSTER SAVECONFIG": bool_ok,
-        "CLUSTER SETSLOT": bool_ok,
-        "CLUSTER SLAVES": parse_cluster_nodes,
-        **string_keys_to_dict("GEODIST", float_or_none),
-        "GEOHASH": lambda r: list(map(str_if_bytes, r)),
-        "GEOPOS": lambda r: list(
-            map(lambda ll: (float(ll[0]), float(ll[1])) if ll is not None else None, r)
-        ),
-        "GEOSEARCH": parse_geosearch_generic,
-        "GEORADIUS": parse_geosearch_generic,
-        "GEORADIUSBYMEMBER": parse_geosearch_generic,
-        "XAUTOCLAIM": parse_xautoclaim,
-        "XINFO STREAM": parse_xinfo_stream,
-        "XPENDING": parse_xpending,
-        **string_keys_to_dict("XREAD XREADGROUP", parse_xread),
-        "COMMAND GETKEYS": lambda r: list(map(str_if_bytes, r)),
-        **string_keys_to_dict("SORT", sort_return_tuples),
-        "PING": lambda r: str_if_bytes(r) == "PONG",
-        "ACL SETUSER": bool_ok,
-        "PUBSUB NUMSUB": parse_pubsub_numsub,
-        "SCRIPT FLUSH": bool_ok,
-        "SCRIPT LOAD": str_if_bytes,
-        "ACL GETUSER": parse_acl_getuser,
-        "CONFIG SET": bool_ok,
-        **string_keys_to_dict("XREVRANGE XRANGE", parse_stream_list),
-        "XCLAIM": parse_xclaim,
-        "CLUSTER SET-CONFIG-EPOCH": bool_ok,
-        "CLUSTER REPLICAS": parse_cluster_nodes,
-        "ACL LIST": lambda r: list(map(str_if_bytes, r)),
-    }
-
-    RESP2_RESPONSE_CALLBACKS = {
-        "CONFIG GET": parse_config_get,
-        **string_keys_to_dict(
-            "SDIFF SINTER SMEMBERS SUNION", lambda r: r and set(r) or set()
-        ),
-        **string_keys_to_dict("READWRITE", bool_ok),
-        **string_keys_to_dict(
-            "ZPOPMAX ZPOPMIN ZINTER ZDIFF ZUNION ZRANGE ZRANGEBYSCORE "
-            "ZREVRANGE ZREVRANGEBYSCORE",
-            zset_score_pairs,
-        ),
-        **string_keys_to_dict("ZSCORE ZINCRBY", float_or_none),
-        "ZADD": parse_zadd,
-        "ZMSCORE": parse_zmscore,
-        "HGETALL": lambda r: r and pairs_to_dict(r) or {},
-        "MEMORY STATS": parse_memory_stats,
-        "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
-        "STRALGO": parse_stralgo,
-        # **string_keys_to_dict(
-        #     "COPY "
-        #     "HEXISTS HMSET MOVE MSETNX PERSIST "
-        #     "PSETEX RENAMENX SMOVE SETEX SETNX",
-        #     bool,
-        # ),
-        # **string_keys_to_dict(
-        #     "HSTRLEN INCRBY LINSERT LLEN LPUSHX PFADD PFCOUNT RPUSHX SADD "
-        #     "SCARD SDIFFSTORE SETBIT SETRANGE SINTERSTORE SREM STRLEN "
-        #     "SUNIONSTORE UNLINK XACK XDEL XLEN XTRIM ZCARD ZLEXCOUNT ZREM "
-        #     "ZREMRANGEBYLEX ZREMRANGEBYRANK ZREMRANGEBYSCORE",
-        #     int,
-        # ),
-        # **string_keys_to_dict(
-        #     "FLUSHALL FLUSHDB LSET LTRIM PFMERGE ASKING "
-        #     "RENAME SAVE SELECT SHUTDOWN SLAVEOF SWAPDB WATCH UNWATCH ",
-        #     bool_ok,
-        # ),
-        # **string_keys_to_dict("ZRANK ZREVRANK", int_or_none),
-        # **string_keys_to_dict("BGREWRITEAOF BGSAVE", lambda r: True),
-        # "ACL HELP": lambda r: list(map(str_if_bytes, r)),
-        # "ACL LOAD": bool_ok,
-        # "ACL SAVE": bool_ok,
-        # "ACL USERS": lambda r: list(map(str_if_bytes, r)),
-        # "CLIENT UNBLOCK": lambda r: r and int(r) == 1 or False,
-        # "CLIENT PAUSE": bool_ok,
-        # "CLUSTER ADDSLOTSRANGE": bool_ok,
-        # "CLUSTER DELSLOTSRANGE": bool_ok,
-        # "CLUSTER GETKEYSINSLOT": lambda r: list(map(str_if_bytes, r)),
-        # "CONFIG RESETSTAT": bool_ok,
-        # "DEBUG OBJECT": parse_debug_object,
-        # "FUNCTION DELETE": bool_ok,
-        # "FUNCTION FLUSH": bool_ok,
-        # "FUNCTION RESTORE": bool_ok,
-        # "MEMORY PURGE": bool_ok,
-        # "MEMORY USAGE": int_or_none,
-        # "MODULE LOAD": parse_module_result,
-        # "MODULE UNLOAD": parse_module_result,
-        # "OBJECT": parse_object,
-        # "QUIT": bool_ok,
-        # "RANDOMKEY": lambda r: r and r or None,
-        # "SCRIPT EXISTS": lambda r: list(map(bool, r)),
-        # "SCRIPT KILL": bool_ok,
-        # "SENTINEL CKQUORUM": bool_ok,
-        # "SENTINEL FAILOVER": bool_ok,
-        # "SENTINEL FLUSHCONFIG": bool_ok,
-        # "SENTINEL GET-MASTER-ADDR-BY-NAME": parse_sentinel_get_master,
-        # "SENTINEL MASTER": parse_sentinel_master,
-        # "SENTINEL MASTERS": parse_sentinel_masters,
-        # "SENTINEL MONITOR": bool_ok,
-        # "SENTINEL RESET": bool_ok,
-        # "SENTINEL REMOVE": bool_ok,
-        # "SENTINEL SENTINELS": parse_sentinel_slaves_and_sentinels,
-        # "SENTINEL SET": bool_ok,
-        # "SENTINEL SLAVES": parse_sentinel_slaves_and_sentinels,
-        # "SLOWLOG RESET": bool_ok,
-        # "XGROUP CREATE": bool_ok,
-        # "XGROUP DESTROY": bool,
-        # "XGROUP SETID": bool_ok,
-        "XINFO CONSUMERS": parse_list_of_dicts,
-        "XINFO GROUPS": parse_list_of_dicts,
-    }
-
-    RESP3_RESPONSE_CALLBACKS = {
-        **string_keys_to_dict(
-            "ZRANGE ZINTER ZPOPMAX ZPOPMIN ZRANGEBYSCORE ZREVRANGE ZREVRANGEBYSCORE "
-            "ZUNION HGETALL XREADGROUP",
-            lambda r, **kwargs: r,
-        ),
-        "CONFIG GET": lambda r: {
-            str_if_bytes(key)
-            if key is not None
-            else None: str_if_bytes(value)
-            if value is not None
-            else None
-            for key, value in r.items()
-        },
-        "ACL LOG": lambda r: [
-            {str_if_bytes(key): str_if_bytes(value) for key, value in x.items()}
-            for x in r
-        ]
-        if isinstance(r, list)
-        else bool_ok(r),
-        **string_keys_to_dict("XREAD XREADGROUP", parse_xread_resp3),
-        "COMMAND": parse_command_resp3,
-        "STRALGO": lambda r, **options: {
-            str_if_bytes(key): str_if_bytes(value) for key, value in r.items()
-        }
-        if isinstance(r, dict)
-        else str_if_bytes(r),
-        "XINFO CONSUMERS": lambda r: [
-            {str_if_bytes(key): value for key, value in x.items()} for x in r
-        ],
-        "MEMORY STATS": lambda r: {
-            str_if_bytes(key): value for key, value in r.items()
-        },
-        "XINFO GROUPS": lambda r: [
-            {str_if_bytes(key): value for key, value in d.items()} for d in r
-        ],
-    }
+    pass
 
 
-class Redis(AbstractRedis, RedisModuleCommands, CoreCommands, SentinelCommands):
+class Redis(RedisModuleCommands, CoreCommands, SentinelCommands):
     """
     Implementation of the Redis protocol.
 
     This abstract class provides a Python interface to all Redis commands
     and an implementation of the Redis protocol.
 
     Pipelines derive from this, implementing how
@@ -972,16 +124,20 @@
         or "Yes"/"No". Values that cannot be properly cast cause a
         ``ValueError`` to be raised. Once parsed, the querystring arguments
         and keyword arguments are passed to the ``ConnectionPool``'s
         class initializer. In the case of conflicting arguments, querystring
         arguments always win.
 
         """
+        single_connection_client = kwargs.pop("single_connection_client", False)
         connection_pool = ConnectionPool.from_url(url, **kwargs)
-        return cls(connection_pool=connection_pool)
+        return cls(
+            connection_pool=connection_pool,
+            single_connection_client=single_connection_client,
+        )
 
     def __init__(
         self,
         host="localhost",
         port=6379,
         db=0,
         password=None,
@@ -1110,20 +266,20 @@
                     )
             connection_pool = ConnectionPool(**kwargs)
         self.connection_pool = connection_pool
         self.connection = None
         if single_connection_client:
             self.connection = self.connection_pool.get_connection("_")
 
-        self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
+        self.response_callbacks = CaseInsensitiveDict(_RedisCallbacks)
 
         if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+            self.response_callbacks.update(_RedisCallbacksRESP3)
         else:
-            self.response_callbacks.update(self.__class__.RESP2_RESPONSE_CALLBACKS)
+            self.response_callbacks.update(_RedisCallbacksRESP2)
 
     def __repr__(self):
         return f"{type(self).__name__}<{repr(self.connection_pool)}>"
 
     def get_encoder(self):
         """Get the connection pool's encoder"""
         return self.connection_pool.get_encoder()
@@ -1621,15 +777,15 @@
 
         def try_read():
             if not block:
                 if not conn.can_read(timeout=timeout):
                     return None
             else:
                 conn.connect()
-            return conn.read_response(push_request=True)
+            return conn.read_response(disconnect_on_error=False, push_request=True)
 
         response = self._execute(conn, try_read)
 
         if self.is_health_check_response(response):
             # ignore the health check message as user might not expect it
             self.health_check_response_counter -= 1
             return None
```

### Comparing `redis-5.0.0rc1/redis/cluster.py` & `redis-5.0.0rc2/redis/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import socket
 import sys
 import threading
 import time
 from collections import OrderedDict
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+from redis._parsers import CommandsParser, Encoder
+from redis._parsers.helpers import parse_scan
 from redis.backoff import default_backoff
-from redis.client import CaseInsensitiveDict, PubSub, Redis, parse_scan
+from redis.client import CaseInsensitiveDict, PubSub, Redis
 from redis.commands import READ_COMMANDS, RedisClusterCommands
 from redis.commands.helpers import list_or_args
 from redis.connection import ConnectionPool, DefaultParser, parse_url
 from redis.crc import REDIS_CLUSTER_HASH_SLOTS, key_slot
 from redis.exceptions import (
     AskError,
     AuthenticationError,
@@ -26,15 +28,14 @@
     RedisError,
     ResponseError,
     SlotNotCoveredError,
     TimeoutError,
     TryAgainError,
 )
 from redis.lock import Lock
-from redis.parsers import CommandsParser, Encoder
 from redis.retry import Retry
 from redis.utils import (
     HIREDIS_AVAILABLE,
     dict_merge,
     list_keys_to_dict,
     merge_result,
     safe_str,
@@ -112,14 +113,21 @@
                 dict_node[node[i]] = node[i + 1]
             shard["nodes"].append(dict_node)
         shards.append(shard)
 
     return shards
 
 
+def parse_cluster_myshardid(resp, **options):
+    """
+    Parse CLUSTER MYSHARDID response.
+    """
+    return resp.decode("utf-8")
+
+
 PRIMARY = "primary"
 REPLICA = "replica"
 SLOT_ID = "slot-id"
 
 REDIS_ALLOWED_KEYS = (
     "charset",
     "connection_class",
@@ -232,14 +240,15 @@
                 "KEYS",
                 "DBSIZE",
                 "BGSAVE",
                 "SLOWLOG GET",
                 "SLOWLOG LEN",
                 "SLOWLOG RESET",
                 "WAIT",
+                "WAITAOF",
                 "SAVE",
                 "MEMORY PURGE",
                 "MEMORY MALLOC-STATS",
                 "MEMORY STATS",
                 "LASTSAVE",
                 "CLIENT TRACKINGINFO",
                 "CLIENT PAUSE",
@@ -342,14 +351,15 @@
             "FT.SYNADD",
         ],
     )
 
     CLUSTER_COMMANDS_RESPONSE_CALLBACKS = {
         "CLUSTER SLOTS": parse_cluster_slots,
         "CLUSTER SHARDS": parse_cluster_shards,
+        "CLUSTER MYSHARDID": parse_cluster_myshardid,
     }
 
     RESULT_CALLBACKS = dict_merge(
         list_keys_to_dict(["PUBSUB NUMSUB", "PUBSUB SHARDNUMSUB"], parse_pubsub_numsub),
         list_keys_to_dict(
             ["PUBSUB NUMPAT"], lambda command, res: sum(list(res.values()))
         ),
@@ -469,14 +479,15 @@
         cluster_error_retry_attempts: int = 3,
         retry: Optional["Retry"] = None,
         require_full_coverage: bool = False,
         reinitialize_steps: int = 5,
         read_from_replicas: bool = False,
         dynamic_startup_nodes: bool = True,
         url: Optional[str] = None,
+        address_remap: Optional[Callable[[str, int], Tuple[str, int]]] = None,
         **kwargs,
     ):
         """
          Initialize a new RedisCluster client.
 
          :param startup_nodes:
              List of nodes from which initial bootstrapping can be done
@@ -517,14 +528,20 @@
             and the cluster does not need to be reinitialized on this current
             error handling, only the MOVED slot will be patched with the
             redirected node.
             To reinitialize the cluster on every MOVED error, set
             reinitialize_steps to 1.
             To avoid reinitializing the cluster on moved errors, set
             reinitialize_steps to 0.
+        :param address_remap:
+            An optional callable which, when provided with an internal network
+            address of a node, e.g. a `(host, port)` tuple, will return the address
+            where the node is reachable.  This can be used to map the addresses at
+            which the nodes _think_ they are, to addresses at which a client may
+            reach them, such as when they sit behind a proxy.
 
          :**kwargs:
              Extra arguments that will be sent into Redis instance when created
              (See Official redis-py doc for supported kwargs
          [https://github.com/andymccurdy/redis-py/blob/master/redis/client.py])
              Some kwargs are not supported and will raise a
              RedisClusterException:
@@ -597,14 +614,15 @@
         self.reinitialize_counter = 0
         self.reinitialize_steps = reinitialize_steps
         self.nodes_manager = NodesManager(
             startup_nodes=startup_nodes,
             from_url=from_url,
             require_full_coverage=require_full_coverage,
             dynamic_startup_nodes=dynamic_startup_nodes,
+            address_remap=address_remap,
             **kwargs,
         )
 
         self.cluster_response_callbacks = CaseInsensitiveDict(
             self.__class__.CLUSTER_COMMANDS_RESPONSE_CALLBACKS
         )
         self.result_callbacks = CaseInsensitiveDict(self.__class__.RESULT_CALLBACKS)
@@ -1272,25 +1290,27 @@
         self,
         startup_nodes,
         from_url=False,
         require_full_coverage=False,
         lock=None,
         dynamic_startup_nodes=True,
         connection_pool_class=ConnectionPool,
+        address_remap: Optional[Callable[[str, int], Tuple[str, int]]] = None,
         **kwargs,
     ):
         self.nodes_cache = {}
         self.slots_cache = {}
         self.startup_nodes = {}
         self.default_node = None
         self.populate_startup_nodes(startup_nodes)
         self.from_url = from_url
         self._require_full_coverage = require_full_coverage
         self._dynamic_startup_nodes = dynamic_startup_nodes
         self.connection_pool_class = connection_pool_class
+        self.address_remap = address_remap
         self._moved_exception = None
         self.connection_kwargs = kwargs
         self.read_load_balancer = LoadBalancer()
         if lock is None:
             lock = threading.Lock()
         self._lock = lock
         self.initialize()
@@ -1505,14 +1525,15 @@
 
             for slot in cluster_slots:
                 primary_node = slot[2]
                 host = str_if_bytes(primary_node[0])
                 if host == "":
                     host = startup_node.host
                 port = int(primary_node[1])
+                host, port = self.remap_host_port(host, port)
 
                 target_node = self._get_or_create_cluster_node(
                     host, port, PRIMARY, tmp_nodes_cache
                 )
                 # add this node to the nodes cache
                 tmp_nodes_cache[target_node.name] = target_node
 
@@ -1521,14 +1542,15 @@
                         tmp_slots[i] = []
                         tmp_slots[i].append(target_node)
                         replica_nodes = [slot[j] for j in range(3, len(slot))]
 
                         for replica_node in replica_nodes:
                             host = str_if_bytes(replica_node[0])
                             port = replica_node[1]
+                            host, port = self.remap_host_port(host, port)
 
                             target_replica_node = self._get_or_create_cluster_node(
                                 host, port, REPLICA, tmp_nodes_cache
                             )
                             tmp_slots[i].append(target_replica_node)
                             # add this node to the nodes cache
                             tmp_nodes_cache[
@@ -1594,14 +1616,24 @@
     def reset(self):
         try:
             self.read_load_balancer.reset()
         except TypeError:
             # The read_load_balancer is None, do nothing
             pass
 
+    def remap_host_port(self, host: str, port: int) -> Tuple[str, int]:
+        """
+        Remap the host and port returned from the cluster to a different
+        internal value.  Useful if the client is not connecting directly
+        to the cluster.
+        """
+        if self.address_remap:
+            return self.address_remap((host, port))
+        return host, port
+
 
 class ClusterPubSub(PubSub):
     """
     Wrapper for PubSub class.
 
     IMPORTANT: before using ClusterPubSub, read about the known limitations
     with pubsub in Cluster mode and learn how to workaround them:
```

### Comparing `redis-5.0.0rc1/redis/commands/__init__.py` & `redis-5.0.0rc2/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/bf/__init__.py` & `redis-5.0.0rc2/redis/commands/bf/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from redis.client import bool_ok
+from redis._parsers.helpers import bool_ok
 
 from ..helpers import parse_to_list
 from .commands import *  # noqa
 from .info import BFInfo, CFInfo, CMSInfo, TDigestInfo, TopKInfo
 
 
 class AbstractBloom(object):
@@ -87,167 +87,167 @@
             params.extend(["BUCKETSIZE", bucket_size])
 
 
 class CMSBloom(CMSCommands, AbstractBloom):
     def __init__(self, client, **kwargs):
         """Create a new RedisBloom client."""
         # Set the module commands' callbacks
-        MODULE_CALLBACKS = {
+        _MODULE_CALLBACKS = {
             CMS_INITBYDIM: bool_ok,
             CMS_INITBYPROB: bool_ok,
             # CMS_INCRBY: spaceHolder,
             # CMS_QUERY: spaceHolder,
             CMS_MERGE: bool_ok,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             CMS_INFO: CMSInfo,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.commandmixin = CMSCommands
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in MODULE_CALLBACKS.items():
+        for k, v in _MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
 
 
 class TOPKBloom(TOPKCommands, AbstractBloom):
     def __init__(self, client, **kwargs):
         """Create a new RedisBloom client."""
         # Set the module commands' callbacks
-        MODULE_CALLBACKS = {
+        _MODULE_CALLBACKS = {
             TOPK_RESERVE: bool_ok,
             # TOPK_QUERY: spaceHolder,
             # TOPK_COUNT: spaceHolder,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             TOPK_ADD: parse_to_list,
             TOPK_INCRBY: parse_to_list,
-            TOPK_LIST: parse_to_list,
             TOPK_INFO: TopKInfo,
+            TOPK_LIST: parse_to_list,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.commandmixin = TOPKCommands
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in MODULE_CALLBACKS.items():
+        for k, v in _MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
 
 
 class CFBloom(CFCommands, AbstractBloom):
     def __init__(self, client, **kwargs):
         """Create a new RedisBloom client."""
         # Set the module commands' callbacks
-        MODULE_CALLBACKS = {
+        _MODULE_CALLBACKS = {
             CF_RESERVE: bool_ok,
             # CF_ADD: spaceHolder,
             # CF_ADDNX: spaceHolder,
             # CF_INSERT: spaceHolder,
             # CF_INSERTNX: spaceHolder,
             # CF_EXISTS: spaceHolder,
             # CF_DEL: spaceHolder,
             # CF_COUNT: spaceHolder,
             # CF_SCANDUMP: spaceHolder,
             # CF_LOADCHUNK: spaceHolder,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             CF_INFO: CFInfo,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.commandmixin = CFCommands
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in MODULE_CALLBACKS.items():
+        for k, v in _MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
 
 
 class TDigestBloom(TDigestCommands, AbstractBloom):
     def __init__(self, client, **kwargs):
         """Create a new RedisBloom client."""
         # Set the module commands' callbacks
-        MODULE_CALLBACKS = {
+        _MODULE_CALLBACKS = {
             TDIGEST_CREATE: bool_ok,
             # TDIGEST_RESET: bool_ok,
             # TDIGEST_ADD: spaceHolder,
             # TDIGEST_MERGE: spaceHolder,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             TDIGEST_BYRANK: parse_to_list,
             TDIGEST_BYREVRANK: parse_to_list,
             TDIGEST_CDF: parse_to_list,
-            TDIGEST_QUANTILE: parse_to_list,
+            TDIGEST_INFO: TDigestInfo,
             TDIGEST_MIN: float,
             TDIGEST_MAX: float,
             TDIGEST_TRIMMED_MEAN: float,
-            TDIGEST_INFO: TDigestInfo,
+            TDIGEST_QUANTILE: parse_to_list,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.commandmixin = TDigestCommands
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in MODULE_CALLBACKS.items():
+        for k, v in _MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
 
 
 class BFBloom(BFCommands, AbstractBloom):
     def __init__(self, client, **kwargs):
         """Create a new RedisBloom client."""
         # Set the module commands' callbacks
-        MODULE_CALLBACKS = {
+        _MODULE_CALLBACKS = {
             BF_RESERVE: bool_ok,
             # BF_ADD: spaceHolder,
             # BF_MADD: spaceHolder,
             # BF_INSERT: spaceHolder,
             # BF_EXISTS: spaceHolder,
             # BF_MEXISTS: spaceHolder,
             # BF_SCANDUMP: spaceHolder,
             # BF_LOADCHUNK: spaceHolder,
             # BF_CARD: spaceHolder,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             BF_INFO: BFInfo,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.commandmixin = BFCommands
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            _MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in MODULE_CALLBACKS.items():
+        for k, v in _MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
```

### Comparing `redis-5.0.0rc1/redis/commands/bf/commands.py` & `redis-5.0.0rc2/redis/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/bf/info.py` & `redis-5.0.0rc2/redis/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/cluster.py` & `redis-5.0.0rc2/redis/commands/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 from .helpers import list_or_args
 from .redismodules import RedisModuleCommands
 
 if TYPE_CHECKING:
     from redis.asyncio.cluster import TargetNodesT
 
-
 # Not complete, but covers the major ones
 # https://redis.io/commands
 READ_COMMANDS = frozenset(
     [
         "BITCOUNT",
         "BITPOS",
         "EVAL_RO",
@@ -630,14 +629,22 @@
         """
         Returns details about the shards of the cluster.
 
         For more information see https://redis.io/commands/cluster-shards
         """
         return self.execute_command("CLUSTER SHARDS", target_nodes=target_nodes)
 
+    def cluster_myshardid(self, target_nodes=None):
+        """
+        Returns the shard ID of the node.
+
+        For more information see https://redis.io/commands/cluster-myshardid/
+        """
+        return self.execute_command("CLUSTER MYSHARDID", target_nodes=target_nodes)
+
     def cluster_links(self, target_node: "TargetNodesT") -> ResponseT:
         """
         Each node in a Redis Cluster maintains a pair of long-lived TCP link with each
         peer in the cluster: One for sending outbound messages towards the peer and one
         for receiving inbound messages from the peer.
 
         This command outputs information of all such peer links as an array.
```

### Comparing `redis-5.0.0rc1/redis/commands/core.py` & `redis-5.0.0rc2/redis/commands/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,14 +757,25 @@
         """
         Sets the client eviction mode for the current connection.
 
         For more information see https://redis.io/commands/client-no-evict
         """
         return self.execute_command("CLIENT NO-EVICT", mode)
 
+    def client_no_touch(self, mode: str) -> Union[Awaitable[str], str]:
+        """
+        # The command controls whether commands sent by the client will alter
+        # the LRU/LFU of the keys they access.
+        # When turned on, the current client will not change LFU/LRU stats,
+        # unless it sends the TOUCH command.
+
+        For more information see https://redis.io/commands/client-no-touch
+        """
+        return self.execute_command("CLIENT NO-TOUCH", mode)
+
     def command(self, **kwargs):
         """
         Returns dict reply of details about all Redis commands.
 
         For more information see https://redis.io/commands/command
         """
         return self.execute_command("COMMAND", **kwargs)
@@ -1326,14 +1337,29 @@
         we finally have at least ``num_replicas``, or when the ``timeout`` was
         reached.
 
         For more information see https://redis.io/commands/wait
         """
         return self.execute_command("WAIT", num_replicas, timeout, **kwargs)
 
+    def waitaof(
+        self, num_local: int, num_replicas: int, timeout: int, **kwargs
+    ) -> ResponseT:
+        """
+        This command blocks the current client until all previous write
+        commands by that client are acknowledged as having been fsynced
+        to the AOF of the local Redis and/or at least the specified number
+        of replicas.
+
+        For more information see https://redis.io/commands/waitaof
+        """
+        return self.execute_command(
+            "WAITAOF", num_local, num_replicas, timeout, **kwargs
+        )
+
     def hello(self):
         """
         This function throws a NotImplementedError since it is intentionally
         not supported.
         """
         raise NotImplementedError(
             "HELLO is intentionally not implemented in the client."
@@ -3485,16 +3511,16 @@
         For more information see https://redis.io/commands/xadd
         """
         pieces: list[EncodableT] = []
         if maxlen is not None and minid is not None:
             raise DataError("Only one of ```maxlen``` or ```minid``` may be specified")
 
         if maxlen is not None:
-            if not isinstance(maxlen, int) or maxlen < 1:
-                raise DataError("XADD maxlen must be a positive integer")
+            if not isinstance(maxlen, int) or maxlen < 0:
+                raise DataError("XADD maxlen must be non-negative integer")
             pieces.append(b"MAXLEN")
             if approximate:
                 pieces.append(b"~")
             pieces.append(str(maxlen))
         if minid is not None:
             pieces.append(b"MINID")
             if approximate:
@@ -4643,21 +4669,30 @@
         if start is not None and num is not None:
             pieces.extend(["LIMIT", start, num])
         if withscores:
             pieces.append("WITHSCORES")
         options = {"withscores": withscores, "score_cast_func": score_cast_func}
         return self.execute_command(*pieces, **options)
 
-    def zrank(self, name: KeyT, value: EncodableT) -> ResponseT:
+    def zrank(
+        self,
+        name: KeyT,
+        value: EncodableT,
+        withscore: bool = False,
+    ) -> ResponseT:
         """
         Returns a 0-based value indicating the rank of ``value`` in sorted set
-        ``name``
+        ``name``.
+        The optional WITHSCORE argument supplements the command's
+        reply with the score of the element returned.
 
         For more information see https://redis.io/commands/zrank
         """
+        if withscore:
+            return self.execute_command("ZRANK", name, value, "WITHSCORE")
         return self.execute_command("ZRANK", name, value)
 
     def zrem(self, name: KeyT, *values: FieldT) -> ResponseT:
         """
         Remove member ``values`` from sorted set ``name``
 
         For more information see https://redis.io/commands/zrem
@@ -4693,21 +4728,30 @@
         Remove all elements in the sorted set ``name`` with scores
         between ``min`` and ``max``. Returns the number of elements removed.
 
         For more information see https://redis.io/commands/zremrangebyscore
         """
         return self.execute_command("ZREMRANGEBYSCORE", name, min, max)
 
-    def zrevrank(self, name: KeyT, value: EncodableT) -> ResponseT:
+    def zrevrank(
+        self,
+        name: KeyT,
+        value: EncodableT,
+        withscore: bool = False,
+    ) -> ResponseT:
         """
         Returns a 0-based value indicating the descending rank of
-        ``value`` in sorted set ``name``
+        ``value`` in sorted set ``name``.
+        The optional ``withscore`` argument supplements the command's
+        reply with the score of the element returned.
 
         For more information see https://redis.io/commands/zrevrank
         """
+        if withscore:
+            return self.execute_command("ZREVRANK", name, value, "WITHSCORE")
         return self.execute_command("ZREVRANK", name, value)
 
     def zscore(self, name: KeyT, value: EncodableT) -> ResponseT:
         """
         Return the score of element ``value`` in sorted set ``name``
 
         For more information see https://redis.io/commands/zscore
```

### Comparing `redis-5.0.0rc1/redis/commands/graph/__init__.py` & `redis-5.0.0rc2/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/commands.py` & `redis-5.0.0rc2/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/edge.py` & `redis-5.0.0rc2/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/execution_plan.py` & `redis-5.0.0rc2/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/node.py` & `redis-5.0.0rc2/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/path.py` & `redis-5.0.0rc2/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/graph/query_result.py` & `redis-5.0.0rc2/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/helpers.py` & `redis-5.0.0rc2/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/json/__init__.py` & `redis-5.0.0rc2/redis/commands/json/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,60 +27,62 @@
         :param decoder:
         :type json.JSONDecoder: An instance of json.JSONDecoder
 
         :param encoder:
         :type json.JSONEncoder: An instance of json.JSONEncoder
         """
         # Set the module commands' callbacks
-        self.MODULE_CALLBACKS = {
+        self._MODULE_CALLBACKS = {
             "JSON.ARRPOP": self._decode,
+            "JSON.DEBUG": self._decode,
+            "JSON.MERGE": lambda r: r and nativestr(r) == "OK",
             "JSON.MGET": bulk_of_jsons(self._decode),
+            "JSON.MSET": lambda r: r and nativestr(r) == "OK",
+            "JSON.RESP": self._decode,
             "JSON.SET": lambda r: r and nativestr(r) == "OK",
-            "JSON.DEBUG": self._decode,
             "JSON.TOGGLE": self._decode,
-            "JSON.RESP": self._decode,
         }
 
-        RESP2_MODULE_CALLBACKS = {
-            "JSON.ARRTRIM": self._decode,
-            "JSON.OBJLEN": self._decode,
+        _RESP2_MODULE_CALLBACKS = {
             "JSON.ARRAPPEND": self._decode,
             "JSON.ARRINDEX": self._decode,
             "JSON.ARRINSERT": self._decode,
-            "JSON.TOGGLE": self._decode,
-            "JSON.STRAPPEND": self._decode,
-            "JSON.STRLEN": self._decode,
             "JSON.ARRLEN": self._decode,
+            "JSON.ARRTRIM": self._decode,
             "JSON.CLEAR": int,
             "JSON.DEL": int,
             "JSON.FORGET": int,
+            "JSON.GET": self._decode,
             "JSON.NUMINCRBY": self._decode,
             "JSON.NUMMULTBY": self._decode,
             "JSON.OBJKEYS": self._decode,
-            "JSON.GET": self._decode,
+            "JSON.STRAPPEND": self._decode,
+            "JSON.OBJLEN": self._decode,
+            "JSON.STRLEN": self._decode,
+            "JSON.TOGGLE": self._decode,
         }
 
-        RESP3_MODULE_CALLBACKS = {
+        _RESP3_MODULE_CALLBACKS = {
             "JSON.GET": lambda response: [
                 [self._decode(r) for r in res] for res in response
             ]
             if response
             else response
         }
 
         self.client = client
         self.execute_command = client.execute_command
         self.MODULE_VERSION = version
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            self.MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            self._MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            self.MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            self._MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for key, value in self.MODULE_CALLBACKS.items():
+        for key, value in self._MODULE_CALLBACKS.items():
             self.client.set_response_callback(key, value)
 
         self.__encoder__ = encoder
         self.__decoder__ = decoder
 
     def _decode(self, obj):
         """Get the decoder."""
@@ -128,15 +130,15 @@
                 reinitialize_steps=self.client.reinitialize_steps,
                 lock=self.client._lock,
             )
 
         else:
             p = Pipeline(
                 connection_pool=self.client.connection_pool,
-                response_callbacks=self.MODULE_CALLBACKS,
+                response_callbacks=self._MODULE_CALLBACKS,
                 transaction=transaction,
                 shard_hint=shard_hint,
             )
 
         p._encode = self._encode
         p._decode = self._decode
         return p
```

### Comparing `redis-5.0.0rc1/redis/commands/json/commands.py` & `redis-5.0.0rc2/redis/commands/json/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from json import JSONDecodeError, loads
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from redis.exceptions import DataError
 from redis.utils import deprecated_function
 
 from ._util import JsonType
 from .decoders import decode_dict_keys
 from .path import Path
@@ -249,14 +249,54 @@
             )
         elif nx:
             pieces.append("NX")
         elif xx:
             pieces.append("XX")
         return self.execute_command("JSON.SET", *pieces)
 
+    def mset(self, triplets: List[Tuple[str, str, JsonType]]) -> Optional[str]:
+        """
+        Set the JSON value at key ``name`` under the ``path`` to ``obj``
+        for one or more keys.
+
+        ``triplets`` is a list of one or more triplets of key, path, value.
+
+        For the purpose of using this within a pipeline, this command is also
+        aliased to JSON.MSET.
+
+        For more information see `JSON.MSET <https://redis.io/commands/json.mset>`_.
+        """
+        pieces = []
+        for triplet in triplets:
+            pieces.extend([triplet[0], str(triplet[1]), self._encode(triplet[2])])
+        return self.execute_command("JSON.MSET", *pieces)
+
+    def merge(
+        self,
+        name: str,
+        path: str,
+        obj: JsonType,
+        decode_keys: Optional[bool] = False,
+    ) -> Optional[str]:
+        """
+        Merges a given JSON value into matching paths. Consequently, JSON values
+        at matching paths are updated, deleted, or expanded with new children
+
+        ``decode_keys`` If set to True, the keys of ``obj`` will be decoded
+        with utf-8.
+
+        For more information see `JSON.MERGE <https://redis.io/commands/json.merge>`_.
+        """
+        if decode_keys:
+            obj = decode_dict_keys(obj)
+
+        pieces = [name, str(path), self._encode(obj)]
+
+        return self.execute_command("JSON.MERGE", *pieces)
+
     def set_file(
         self,
         name: str,
         path: str,
         file_name: str,
         nx: Optional[bool] = False,
         xx: Optional[bool] = False,
```

### Comparing `redis-5.0.0rc1/redis/commands/json/decoders.py` & `redis-5.0.0rc2/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/redismodules.py` & `redis-5.0.0rc2/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/__init__.py` & `redis-5.0.0rc2/redis/commands/search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,20 +91,20 @@
     def __init__(self, client, index_name="idx"):
         """
         Create a new Client for the given index_name.
         The default name is `idx`
 
         If conn is not None, we employ an already existing redis connection
         """
-        self.MODULE_CALLBACKS = {}
+        self._MODULE_CALLBACKS = {}
         self.client = client
         self.index_name = index_name
         self.execute_command = client.execute_command
         self._pipeline = client.pipeline
-        self.RESP2_MODULE_CALLBACKS = {
+        self._RESP2_MODULE_CALLBACKS = {
             INFO_CMD: self._parse_info,
             SEARCH_CMD: self._parse_search,
             AGGREGATE_CMD: self._parse_aggregate,
             PROFILE_CMD: self._parse_profile,
             SPELLCHECK_CMD: self._parse_spellcheck,
             CONFIG_CMD: self._parse_config_get,
             SYNDUMP_CMD: self._parse_syndump,
@@ -112,15 +112,15 @@
 
     def pipeline(self, transaction=True, shard_hint=None):
         """Creates a pipeline for the SEARCH module, that can be used for executing
         SEARCH commands, as well as classic core commands.
         """
         p = Pipeline(
             connection_pool=self.client.connection_pool,
-            response_callbacks=self.MODULE_CALLBACKS,
+            response_callbacks=self._MODULE_CALLBACKS,
             transaction=transaction,
             shard_hint=shard_hint,
         )
         p.index_name = self.index_name
         return p
 
 
@@ -170,15 +170,15 @@
 
     def pipeline(self, transaction=True, shard_hint=None):
         """Creates a pipeline for the SEARCH module, that can be used for executing
         SEARCH commands, as well as classic core commands.
         """
         p = AsyncPipeline(
             connection_pool=self.client.connection_pool,
-            response_callbacks=self.MODULE_CALLBACKS,
+            response_callbacks=self._MODULE_CALLBACKS,
             transaction=transaction,
             shard_hint=shard_hint,
         )
         p.index_name = self.index_name
         return p
```

### Comparing `redis-5.0.0rc1/redis/commands/search/aggregation.py` & `redis-5.0.0rc2/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/commands.py` & `redis-5.0.0rc2/redis/commands/search/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 class SearchCommands:
     """Search commands."""
 
     def _parse_results(self, cmd, res, **kwargs):
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
             return res
         else:
-            return self.RESP2_MODULE_CALLBACKS[cmd](res, **kwargs)
+            return self._RESP2_MODULE_CALLBACKS[cmd](res, **kwargs)
 
     def _parse_info(self, res, **kwargs):
         it = map(to_string, res)
         return dict(zip(it, it))
 
     def _parse_search(self, res, **kwargs):
         return Result(
```

### Comparing `redis-5.0.0rc1/redis/commands/search/field.py` & `redis-5.0.0rc2/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/indexDefinition.py` & `redis-5.0.0rc2/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/query.py` & `redis-5.0.0rc2/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/querystring.py` & `redis-5.0.0rc2/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/reducers.py` & `redis-5.0.0rc2/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/result.py` & `redis-5.0.0rc2/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/search/suggestion.py` & `redis-5.0.0rc2/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/sentinel.py` & `redis-5.0.0rc2/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/timeseries/__init__.py` & `redis-5.0.0rc2/redis/commands/timeseries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import redis
-from redis.client import bool_ok
+from redis._parsers.helpers import bool_ok
 
 from ..helpers import parse_to_list
 from .commands import (
     ALTER_CMD,
     CREATE_CMD,
     CREATERULE_CMD,
     DEL_CMD,
@@ -29,43 +29,43 @@
     The client allows to interact with RedisTimeSeries and use all of it's
     functionality.
     """
 
     def __init__(self, client=None, **kwargs):
         """Create a new RedisTimeSeries client."""
         # Set the module commands' callbacks
-        self.MODULE_CALLBACKS = {
-            CREATE_CMD: bool_ok,
+        self._MODULE_CALLBACKS = {
             ALTER_CMD: bool_ok,
+            CREATE_CMD: bool_ok,
             CREATERULE_CMD: bool_ok,
             DELETERULE_CMD: bool_ok,
         }
 
-        RESP2_MODULE_CALLBACKS = {
+        _RESP2_MODULE_CALLBACKS = {
             DEL_CMD: int,
             GET_CMD: parse_get,
-            QUERYINDEX_CMD: parse_to_list,
-            RANGE_CMD: parse_range,
-            REVRANGE_CMD: parse_range,
+            INFO_CMD: TSInfo,
             MGET_CMD: parse_m_get,
             MRANGE_CMD: parse_m_range,
             MREVRANGE_CMD: parse_m_range,
-            INFO_CMD: TSInfo,
+            RANGE_CMD: parse_range,
+            REVRANGE_CMD: parse_range,
+            QUERYINDEX_CMD: parse_to_list,
         }
-        RESP3_MODULE_CALLBACKS = {}
+        _RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.execute_command = client.execute_command
 
         if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
-            self.MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+            self._MODULE_CALLBACKS.update(_RESP3_MODULE_CALLBACKS)
         else:
-            self.MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+            self._MODULE_CALLBACKS.update(_RESP2_MODULE_CALLBACKS)
 
-        for k, v in self.MODULE_CALLBACKS.items():
+        for k, v in self._MODULE_CALLBACKS.items():
             self.client.set_response_callback(k, v)
 
     def pipeline(self, transaction=True, shard_hint=None):
         """Creates a pipeline for the TimeSeries module, that can be used
         for executing only TimeSeries commands and core commands.
 
         Usage example:
@@ -89,15 +89,15 @@
                 reinitialize_steps=self.client.reinitialize_steps,
                 lock=self.client._lock,
             )
 
         else:
             p = Pipeline(
                 connection_pool=self.client.connection_pool,
-                response_callbacks=self.MODULE_CALLBACKS,
+                response_callbacks=self._MODULE_CALLBACKS,
                 transaction=transaction,
                 shard_hint=shard_hint,
             )
         return p
 
 
 class ClusterPipeline(TimeSeriesCommands, redis.cluster.ClusterPipeline):
```

### Comparing `redis-5.0.0rc1/redis/commands/timeseries/commands.py` & `redis-5.0.0rc2/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/timeseries/info.py` & `redis-5.0.0rc2/redis/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/commands/timeseries/utils.py` & `redis-5.0.0rc2/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/connection.py` & `redis-5.0.0rc2/redis/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from abc import abstractmethod
 from itertools import chain
 from queue import Empty, Full, LifoQueue
 from time import time
 from typing import Optional, Type, Union
 from urllib.parse import parse_qs, unquote, urlparse
 
+from ._parsers import Encoder, _HiredisParser, _RESP2Parser, _RESP3Parser
 from .backoff import NoBackoff
 from .credentials import CredentialProvider, UsernamePasswordCredentialProvider
 from .exceptions import (
     AuthenticationError,
     AuthenticationWrongNumberOfArgsError,
     ChildDeadlockedError,
     ConnectionError,
     DataError,
     RedisError,
     ResponseError,
     TimeoutError,
 )
-from .parsers import Encoder, _HiredisParser, _RESP2Parser, _RESP3Parser
 from .retry import Retry
 from .utils import (
     CRYPTOGRAPHY_AVAILABLE,
     HIREDIS_AVAILABLE,
     HIREDIS_PACK_AVAILABLE,
     SSL_AVAILABLE,
     str_if_bytes,
@@ -125,14 +125,16 @@
 class AbstractConnection:
     "Manages communication to and from a Redis server"
 
     def __init__(
         self,
         db=0,
         password=None,
+        socket_timeout=None,
+        socket_connect_timeout=None,
         retry_on_timeout=False,
         retry_on_error=SENTINEL,
         encoding="utf-8",
         encoding_errors="strict",
         decode_responses=False,
         parser_class=DefaultParser,
         socket_read_size=65536,
@@ -161,14 +163,18 @@
             )
         self.pid = os.getpid()
         self.db = db
         self.client_name = client_name
         self.credential_provider = credential_provider
         self.password = password
         self.username = username
+        self.socket_timeout = socket_timeout
+        if socket_connect_timeout is None:
+            socket_connect_timeout = socket_timeout
+        self.socket_connect_timeout = socket_connect_timeout
         self.retry_on_timeout = retry_on_timeout
         if retry_on_error is SENTINEL:
             retry_on_error = []
         if retry_on_timeout:
             # Add TimeoutError to the errors list to retry on
             retry_on_error.append(TimeoutError)
         self.retry_on_error = retry_on_error
@@ -359,28 +365,30 @@
             self.send_command("SELECT", self.db)
             if str_if_bytes(self.read_response()) != "OK":
                 raise ConnectionError("Invalid Database")
 
     def disconnect(self, *args):
         "Disconnects from the Redis server"
         self._parser.on_disconnect()
-        if self._sock is None:
+
+        conn_sock = self._sock
+        self._sock = None
+        if conn_sock is None:
             return
 
         if os.getpid() == self.pid:
             try:
-                self._sock.shutdown(socket.SHUT_RDWR)
+                conn_sock.shutdown(socket.SHUT_RDWR)
             except OSError:
                 pass
 
         try:
-            self._sock.close()
+            conn_sock.close()
         except OSError:
             pass
-        self._sock = None
 
     def _send_ping(self):
         """Send PING, expect PONG in return"""
         self.send_command("PING", check_health=False)
         if str_if_bytes(self.read_response()) != "PONG":
             raise ConnectionError("Bad response from PING health check")
 
@@ -412,15 +420,19 @@
             self.disconnect()
             if len(e.args) == 1:
                 errno, errmsg = "UNKNOWN", e.args[0]
             else:
                 errno = e.args[0]
                 errmsg = e.args[1]
             raise ConnectionError(f"Error {errno} while writing to socket. {errmsg}.")
-        except Exception:
+        except BaseException:
+            # BaseExceptions can be raised when a socket send operation is not
+            # finished, e.g. due to a timeout.  Ideally, a caller could then re-try
+            # to send un-sent data. However, the send_packed_command() API
+            # does not support it so there is no point in keeping the connection open.
             self.disconnect()
             raise
 
     def send_command(self, *args, **kwargs):
         """Pack and send a command to the Redis server"""
         self.send_packed_command(
             self._command_packer.pack(*args),
@@ -437,36 +449,48 @@
 
         try:
             return self._parser.can_read(timeout)
         except OSError as e:
             self.disconnect()
             raise ConnectionError(f"Error while reading from {host_error}: {e.args}")
 
-    def read_response(self, disable_decoding=False, push_request=False):
+    def read_response(
+        self,
+        disable_decoding=False,
+        *,
+        disconnect_on_error=True,
+        push_request=False,
+    ):
         """Read the response from a previously sent command"""
 
         host_error = self._host_error()
 
         try:
             if self.protocol in ["3", 3] and not HIREDIS_AVAILABLE:
                 response = self._parser.read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
             else:
                 response = self._parser.read_response(disable_decoding=disable_decoding)
         except socket.timeout:
-            self.disconnect()
+            if disconnect_on_error:
+                self.disconnect()
             raise TimeoutError(f"Timeout reading from {host_error}")
         except OSError as e:
-            self.disconnect()
+            if disconnect_on_error:
+                self.disconnect()
             raise ConnectionError(
                 f"Error while reading from {host_error}" f" : {e.args}"
             )
-        except Exception:
-            self.disconnect()
+        except BaseException:
+            # Also by default close in case of BaseException.  A lot of code
+            # relies on this behaviour when doing Command/Response pairs.
+            # See #1128.
+            if disconnect_on_error:
+                self.disconnect()
             raise
 
         if self.health_check_interval:
             self.next_health_check = time() + self.health_check_interval
 
         if isinstance(response, ResponseError):
             raise response
@@ -510,25 +534,21 @@
 class Connection(AbstractConnection):
     "Manages TCP communication to and from a Redis server"
 
     def __init__(
         self,
         host="localhost",
         port=6379,
-        socket_timeout=None,
-        socket_connect_timeout=None,
         socket_keepalive=False,
         socket_keepalive_options=None,
         socket_type=0,
         **kwargs,
     ):
         self.host = host
         self.port = int(port)
-        self.socket_timeout = socket_timeout
-        self.socket_connect_timeout = socket_connect_timeout or socket_timeout
         self.socket_keepalive = socket_keepalive
         self.socket_keepalive_options = socket_keepalive_options or {}
         self.socket_type = socket_type
         super().__init__(**kwargs)
 
     def repr_pieces(self):
         pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
@@ -755,16 +775,17 @@
         if self.client_name:
             pieces.append(("client_name", self.client_name))
         return pieces
 
     def _connect(self):
         "Create a Unix domain socket connection"
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
-        sock.settimeout(self.socket_timeout)
+        sock.settimeout(self.socket_connect_timeout)
         sock.connect(self.path)
+        sock.settimeout(self.socket_timeout)
         return sock
 
     def _host_error(self):
         return self.path
 
     def _error_message(self, exception):
         # args for socket.error can either be (errno, "message")
```

### Comparing `redis-5.0.0rc1/redis/crc.py` & `redis-5.0.0rc2/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/credentials.py` & `redis-5.0.0rc2/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/exceptions.py` & `redis-5.0.0rc2/redis/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,14 +45,26 @@
     pass
 
 
 class NoScriptError(ResponseError):
     pass
 
 
+class OutOfMemoryError(ResponseError):
+    """
+    Indicates the database is full. Can only occur when either:
+      * Redis maxmemory-policy=noeviction
+      * Redis maxmemory-policy=volatile* and there are no evictable keys
+
+    For more information see `Memory optimization in Redis <https://redis.io/docs/management/optimization/memory-optimization/#memory-allocation>`_. # noqa
+    """
+
+    pass
+
+
 class ExecAbortError(ResponseError):
     pass
 
 
 class ReadOnlyError(ResponseError):
     pass
 
@@ -127,14 +139,15 @@
 class AskError(ResponseError):
     """
     Error indicated ASK error received from cluster.
     When a slot is set as MIGRATING, the node will accept all queries that
     pertain to this hash slot, but only if the key in question exists,
     otherwise the query is forwarded using a -ASK redirection to the node that
     is target of the migration.
+
     src node: MIGRATING to dst node
         get > ASK error
         ask dst node > ASKING command
     dst node: IMPORTING from src node
         asking command only affects next command
         any op will be allowed after asking command
     """
```

### Comparing `redis-5.0.0rc1/redis/lock.py` & `redis-5.0.0rc2/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/ocsp.py` & `redis-5.0.0rc2/redis/ocsp.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/parsers/__init__.py` & `redis-5.0.0rc2/redis/_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/parsers/base.py` & `redis-5.0.0rc2/redis/_parsers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     AuthenticationWrongNumberOfArgsError,
     BusyLoadingError,
     ConnectionError,
     ExecAbortError,
     ModuleError,
     NoPermissionError,
     NoScriptError,
+    OutOfMemoryError,
     ReadOnlyError,
     RedisError,
     ResponseError,
 )
 from ..typing import EncodableT
 from .encoders import Encoder
 from .socket import SERVER_CLOSED_CONNECTION_ERROR, SocketBuffer
@@ -60,29 +61,31 @@
             "for 'AUTH' command": AuthenticationWrongNumberOfArgsError,
             MODULE_LOAD_ERROR: ModuleError,
             MODULE_EXPORTS_DATA_TYPES_ERROR: ModuleError,
             NO_SUCH_MODULE_ERROR: ModuleError,
             MODULE_UNLOAD_NOT_POSSIBLE_ERROR: ModuleError,
             **NO_AUTH_SET_ERROR,
         },
+        "OOM": OutOfMemoryError,
         "WRONGPASS": AuthenticationError,
         "EXECABORT": ExecAbortError,
         "LOADING": BusyLoadingError,
         "NOSCRIPT": NoScriptError,
         "READONLY": ReadOnlyError,
         "NOAUTH": AuthenticationError,
         "NOPERM": NoPermissionError,
     }
 
-    def parse_error(self, response):
+    @classmethod
+    def parse_error(cls, response):
         "Parse an error response"
         error_code = response.split(" ")[0]
-        if error_code in self.EXCEPTION_CLASSES:
+        if error_code in cls.EXCEPTION_CLASSES:
             response = response[len(error_code) + 1 :]
-            exception_class = self.EXCEPTION_CLASSES[error_code]
+            exception_class = cls.EXCEPTION_CLASSES[error_code]
             if isinstance(exception_class, dict):
                 exception_class = exception_class.get(response, ResponseError)
             return exception_class(response)
         return ResponseError(response)
 
     def on_disconnect(self):
         raise NotImplementedError()
```

### Comparing `redis-5.0.0rc1/redis/parsers/commands.py` & `redis-5.0.0rc2/redis/_parsers/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/parsers/encoders.py` & `redis-5.0.0rc2/redis/_parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/parsers/hiredis.py` & `redis-5.0.0rc2/redis/_parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/parsers/resp2.py` & `redis-5.0.0rc2/redis/_parsers/resp2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from .socket import SERVER_CLOSED_CONNECTION_ERROR
 
 
 class _RESP2Parser(_RESPBase):
     """RESP2 protocol implementation"""
 
     def read_response(self, disable_decoding=False):
-        pos = self._buffer.get_pos()
+        pos = self._buffer.get_pos() if self._buffer else None
         try:
             result = self._read_response(disable_decoding=disable_decoding)
         except BaseException:
-            self._buffer.rewind(pos)
+            if self._buffer:
+                self._buffer.rewind(pos)
             raise
         else:
             self._buffer.purge()
             return result
 
     def _read_response(self, disable_decoding=False):
         raw = self._buffer.readline()
```

### Comparing `redis-5.0.0rc1/redis/parsers/resp3.py` & `redis-5.0.0rc2/redis/_parsers/resp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 
     def handle_push_response(self, response):
         logger = getLogger("push_response")
         logger.info("Push response: " + str(response))
         return response
 
     def read_response(self, disable_decoding=False, push_request=False):
-        pos = self._buffer.get_pos()
+        pos = self._buffer.get_pos() if self._buffer else None
         try:
             result = self._read_response(
                 disable_decoding=disable_decoding, push_request=push_request
             )
         except BaseException:
-            self._buffer.rewind(pos)
+            if self._buffer:
+                self._buffer.rewind(pos)
             raise
         else:
             self._buffer.purge()
             return result
 
     def _read_response(self, disable_decoding=False, push_request=False):
         raw = self._buffer.readline()
```

### Comparing `redis-5.0.0rc1/redis/parsers/socket.py` & `redis-5.0.0rc2/redis/_parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/retry.py` & `redis-5.0.0rc2/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis/sentinel.py` & `redis-5.0.0rc2/redis/sentinel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import weakref
+from typing import Optional
 
 from redis.client import Redis
 from redis.commands import SentinelCommands
 from redis.connection import Connection, ConnectionPool, SSLConnection
 from redis.exceptions import ConnectionError, ReadOnlyError, ResponseError, TimeoutError
 from redis.utils import str_if_bytes
 
@@ -49,17 +50,22 @@
                 except ConnectionError:
                     continue
             raise SlaveNotFoundError  # Never be here
 
     def connect(self):
         return self.retry.call_with_retry(self._connect_retry, lambda error: None)
 
-    def read_response(self, disable_decoding=False):
+    def read_response(
+        self, disable_decoding=False, *, disconnect_on_error: Optional[bool] = False
+    ):
         try:
-            return super().read_response(disable_decoding=disable_decoding)
+            return super().read_response(
+                disable_decoding=disable_decoding,
+                disconnect_on_error=disconnect_on_error,
+            )
         except ReadOnlyError:
             if self.connection_pool.is_master:
                 # When talking to a master, a ReadOnlyError when likely
                 # indicates that the previous master that we're still connected
                 # to has been demoted to a slave and there's a new master.
                 # calling disconnect will force the connection to re-query
                 # sentinel during the next connect() attempt.
@@ -68,14 +74,62 @@
             raise
 
 
 class SentinelManagedSSLConnection(SentinelManagedConnection, SSLConnection):
     pass
 
 
+class SentinelConnectionPoolProxy:
+    def __init__(
+        self,
+        connection_pool,
+        is_master,
+        check_connection,
+        service_name,
+        sentinel_manager,
+    ):
+        self.connection_pool_ref = weakref.ref(connection_pool)
+        self.is_master = is_master
+        self.check_connection = check_connection
+        self.service_name = service_name
+        self.sentinel_manager = sentinel_manager
+        self.reset()
+
+    def reset(self):
+        self.master_address = None
+        self.slave_rr_counter = None
+
+    def get_master_address(self):
+        master_address = self.sentinel_manager.discover_master(self.service_name)
+        if self.is_master and self.master_address != master_address:
+            self.master_address = master_address
+            # disconnect any idle connections so that they reconnect
+            # to the new master the next time that they are used.
+            connection_pool = self.connection_pool_ref()
+            if connection_pool is not None:
+                connection_pool.disconnect(inuse_connections=False)
+        return master_address
+
+    def rotate_slaves(self):
+        slaves = self.sentinel_manager.discover_slaves(self.service_name)
+        if slaves:
+            if self.slave_rr_counter is None:
+                self.slave_rr_counter = random.randint(0, len(slaves) - 1)
+            for _ in range(len(slaves)):
+                self.slave_rr_counter = (self.slave_rr_counter + 1) % len(slaves)
+                slave = slaves[self.slave_rr_counter]
+                yield slave
+        # Fallback to the master connection
+        try:
+            yield self.get_master_address()
+        except MasterNotFoundError:
+            pass
+        raise SlaveNotFoundError(f"No slave found for {self.service_name!r}")
+
+
 class SentinelConnectionPool(ConnectionPool):
     """
     Sentinel backed connection pool.
 
     If ``check_connection`` flag is set to True, SentinelManagedConnection
     sends a PING command right after establishing the connection.
     """
@@ -85,61 +139,51 @@
             "connection_class",
             SentinelManagedSSLConnection
             if kwargs.pop("ssl", False)
             else SentinelManagedConnection,
         )
         self.is_master = kwargs.pop("is_master", True)
         self.check_connection = kwargs.pop("check_connection", False)
+        self.proxy = SentinelConnectionPoolProxy(
+            connection_pool=self,
+            is_master=self.is_master,
+            check_connection=self.check_connection,
+            service_name=service_name,
+            sentinel_manager=sentinel_manager,
+        )
         super().__init__(**kwargs)
-        self.connection_kwargs["connection_pool"] = weakref.proxy(self)
+        self.connection_kwargs["connection_pool"] = self.proxy
         self.service_name = service_name
         self.sentinel_manager = sentinel_manager
 
     def __repr__(self):
         role = "master" if self.is_master else "slave"
         return f"{type(self).__name__}<service={self.service_name}({role})"
 
     def reset(self):
         super().reset()
-        self.master_address = None
-        self.slave_rr_counter = None
+        self.proxy.reset()
+
+    @property
+    def master_address(self):
+        return self.proxy.master_address
 
     def owns_connection(self, connection):
         check = not self.is_master or (
             self.is_master and self.master_address == (connection.host, connection.port)
         )
         parent = super()
         return check and parent.owns_connection(connection)
 
     def get_master_address(self):
-        master_address = self.sentinel_manager.discover_master(self.service_name)
-        if self.is_master:
-            if self.master_address != master_address:
-                self.master_address = master_address
-                # disconnect any idle connections so that they reconnect
-                # to the new master the next time that they are used.
-                self.disconnect(inuse_connections=False)
-        return master_address
+        return self.proxy.get_master_address()
 
     def rotate_slaves(self):
         "Round-robin slave balancer"
-        slaves = self.sentinel_manager.discover_slaves(self.service_name)
-        if slaves:
-            if self.slave_rr_counter is None:
-                self.slave_rr_counter = random.randint(0, len(slaves) - 1)
-            for _ in range(len(slaves)):
-                self.slave_rr_counter = (self.slave_rr_counter + 1) % len(slaves)
-                slave = slaves[self.slave_rr_counter]
-                yield slave
-        # Fallback to the master connection
-        try:
-            yield self.get_master_address()
-        except MasterNotFoundError:
-            pass
-        raise SlaveNotFoundError(f"No slave found for {self.service_name!r}")
+        return self.proxy.rotate_slaves()
 
 
 class Sentinel(SentinelCommands):
     """
     Redis Sentinel cluster client
 
     >>> from redis.sentinel import Sentinel
@@ -226,28 +270,34 @@
         """
         Asks sentinel servers for the Redis master's address corresponding
         to the service labeled ``service_name``.
 
         Returns a pair (address, port) or raises MasterNotFoundError if no
         master is found.
         """
+        collected_errors = list()
         for sentinel_no, sentinel in enumerate(self.sentinels):
             try:
                 masters = sentinel.sentinel_masters()
-            except (ConnectionError, TimeoutError):
+            except (ConnectionError, TimeoutError) as e:
+                collected_errors.append(f"{sentinel} - {e!r}")
                 continue
             state = masters.get(service_name)
             if state and self.check_master_state(state, service_name):
                 # Put this sentinel at the top of the list
                 self.sentinels[0], self.sentinels[sentinel_no] = (
                     sentinel,
                     self.sentinels[0],
                 )
                 return state["ip"], state["port"]
-        raise MasterNotFoundError(f"No master found for {service_name!r}")
+
+        error_info = ""
+        if len(collected_errors) > 0:
+            error_info = f" : {', '.join(collected_errors)}"
+        raise MasterNotFoundError(f"No master found for {service_name!r}{error_info}")
 
     def filter_slaves(self, slaves):
         "Remove slaves that are in an ODOWN or SDOWN state"
         slaves_alive = []
         for slave in slaves:
             if slave["is_odown"] or slave["is_sdown"]:
                 continue
```

### Comparing `redis-5.0.0rc1/redis/typing.py` & `redis-5.0.0rc2/redis/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     TypeVar,
     Union,
 )
 
 from redis.compat import Protocol
 
 if TYPE_CHECKING:
+    from redis._parsers import Encoder
     from redis.asyncio.connection import ConnectionPool as AsyncConnectionPool
     from redis.connection import ConnectionPool
-    from redis.parsers import Encoder
 
 
 Number = Union[int, float]
 EncodedT = Union[bytes, memoryview]
 DecodedT = Union[str, int, float]
 EncodableT = Union[EncodedT, DecodedT]
 AbsExpiryT = Union[int, datetime]
@@ -54,12 +54,12 @@
 class CommandsProtocol(Protocol):
     connection_pool: Union["AsyncConnectionPool", "ConnectionPool"]
 
     def execute_command(self, *args, **options):
         ...
 
 
-class ClusterCommandsProtocol(CommandsProtocol):
+class ClusterCommandsProtocol(CommandsProtocol, Protocol):
     encoder: "Encoder"
 
     def execute_command(self, *args, **options) -> Union[Any, Awaitable]:
         ...
```

### Comparing `redis-5.0.0rc1/redis/utils.py` & `redis-5.0.0rc2/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/redis.egg-info/PKG-INFO` & `redis-5.0.0rc2/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0rc1/redis.egg-info/SOURCES.txt` & `redis-5.0.0rc2/redis.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 redis/typing.py
 redis/utils.py
 redis.egg-info/PKG-INFO
 redis.egg-info/SOURCES.txt
 redis.egg-info/dependency_links.txt
 redis.egg-info/requires.txt
 redis.egg-info/top_level.txt
+redis/_parsers/__init__.py
+redis/_parsers/base.py
+redis/_parsers/commands.py
+redis/_parsers/encoders.py
+redis/_parsers/helpers.py
+redis/_parsers/hiredis.py
+redis/_parsers/resp2.py
+redis/_parsers/resp3.py
+redis/_parsers/socket.py
 redis/asyncio/__init__.py
 redis/asyncio/client.py
 redis/asyncio/cluster.py
 redis/asyncio/connection.py
 redis/asyncio/lock.py
 redis/asyncio/retry.py
 redis/asyncio/sentinel.py
@@ -65,31 +74,23 @@
 redis/commands/search/reducers.py
 redis/commands/search/result.py
 redis/commands/search/suggestion.py
 redis/commands/timeseries/__init__.py
 redis/commands/timeseries/commands.py
 redis/commands/timeseries/info.py
 redis/commands/timeseries/utils.py
-redis/parsers/__init__.py
-redis/parsers/base.py
-redis/parsers/commands.py
-redis/parsers/encoders.py
-redis/parsers/hiredis.py
-redis/parsers/resp2.py
-redis/parsers/resp3.py
-redis/parsers/socket.py
 tests/__init__.py
-tests/asynctests
 tests/conftest.py
 tests/mocks.py
-tests/synctests
+tests/ssl_utils.py
 tests/test_bloom.py
 tests/test_cluster.py
 tests/test_command_parser.py
 tests/test_commands.py
+tests/test_connect.py
 tests/test_connection.py
 tests/test_connection_pool.py
 tests/test_credentials.py
 tests/test_encoding.py
 tests/test_function.py
 tests/test_graph.py
 tests/test_helpers.py
@@ -108,17 +109,19 @@
 tests/test_asyncio/__init__.py
 tests/test_asyncio/compat.py
 tests/test_asyncio/conftest.py
 tests/test_asyncio/mocks.py
 tests/test_asyncio/test_bloom.py
 tests/test_asyncio/test_cluster.py
 tests/test_asyncio/test_commands.py
+tests/test_asyncio/test_connect.py
 tests/test_asyncio/test_connection.py
 tests/test_asyncio/test_connection_pool.py
 tests/test_asyncio/test_credentials.py
+tests/test_asyncio/test_cwe_404.py
 tests/test_asyncio/test_encoding.py
 tests/test_asyncio/test_graph.py
 tests/test_asyncio/test_json.py
 tests/test_asyncio/test_lock.py
 tests/test_asyncio/test_monitor.py
 tests/test_asyncio/test_pipeline.py
 tests/test_asyncio/test_pubsub.py
```

### Comparing `redis-5.0.0rc1/setup.py` & `redis-5.0.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.0.0rc1",
+    version="5.0.0rc2",
     packages=find_packages(
         include=[
             "redis",
+            "redis._parsers",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
             "redis.commands.json",
             "redis.commands.search",
             "redis.commands.timeseries",
             "redis.commands.graph",
@@ -31,15 +32,15 @@
     },
     author="Redis Inc.",
     author_email="oss@redis.com",
     python_requires=">=3.7",
     install_requires=[
         'importlib-metadata >= 1.0; python_version < "3.8"',
         'typing-extensions; python_version<"3.8"',
-        'async-timeout>=4.0.2; python_version<"3.11"',
+        'async-timeout>=4.0.2; python_full_version<="3.11.2"',
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `redis-5.0.0rc1/tests/conftest.py` & `redis-5.0.0rc2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
     r = _get_client(redis.Redis, request, **kwargs)
     return _gen_cluster_mock_resp(r, "OK")
 
 
 @pytest.fixture()
 def mock_cluster_resp_int(request, **kwargs):
     r = _get_client(redis.Redis, request, **kwargs)
-    return _gen_cluster_mock_resp(r, "2")
+    return _gen_cluster_mock_resp(r, 2)
 
 
 @pytest.fixture()
 def mock_cluster_resp_info(request, **kwargs):
     r = _get_client(redis.Redis, request, **kwargs)
     response = (
         "cluster_state:ok\r\ncluster_slots_assigned:16384\r\n"
@@ -423,15 +423,15 @@
     return _gen_cluster_mock_resp(r, response)
 
 
 @pytest.fixture(scope="session")
 def master_host(request):
     url = request.config.getoption("--redis-url")
     parts = urlparse(url)
-    yield parts.hostname, parts.port
+    return parts.hostname, (parts.port or 6379)
 
 
 def wait_for_command(client, monitor, command, key=None):
     # issue a command with a key name that's local to this process.
     # if we find a command with our key before the command we're waiting
     # for, something went wrong
     if key is None:
```

### Comparing `redis-5.0.0rc1/tests/mocks.py` & `redis-5.0.0rc2/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/conftest.py` & `redis-5.0.0rc2/tests/test_asyncio/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import random
 from contextlib import asynccontextmanager as _asynccontextmanager
 from typing import Union
-from urllib.parse import urlparse
 
 import pytest
 import pytest_asyncio
 import redis.asyncio as redis
 from packaging.version import Version
+from redis._parsers import _AsyncHiredisParser, _AsyncRESP2Parser
 from redis.asyncio.client import Monitor
 from redis.asyncio.connection import parse_url
 from redis.asyncio.retry import Retry
 from redis.backoff import NoBackoff
-from redis.parsers import _AsyncHiredisParser, _AsyncRESP2Parser
 from redis.utils import HIREDIS_AVAILABLE
 from tests.conftest import REDIS_INFO
 
 from .compat import mock
 
 
 async def _get_info(redis_url):
@@ -151,15 +150,15 @@
     r = await create_redis(**kwargs)
     return _gen_cluster_mock_resp(r, "OK")
 
 
 @pytest_asyncio.fixture()
 async def mock_cluster_resp_int(create_redis, **kwargs):
     r = await create_redis(**kwargs)
-    return _gen_cluster_mock_resp(r, "2")
+    return _gen_cluster_mock_resp(r, 2)
 
 
 @pytest_asyncio.fixture()
 async def mock_cluster_resp_info(create_redis, **kwargs):
     r = await create_redis(**kwargs)
     response = (
         "cluster_state:ok\r\ncluster_slots_assigned:16384\r\n"
@@ -203,21 +202,14 @@
         "['1df047e5a594f945d82fc140be97a1452bcbf93e 172.17.0.7:7007 "
         "slave 19efe5a631f3296fdf21a5441680f893e8cc96ec 0 "
         "1447836789290 3 connected']"
     )
     return _gen_cluster_mock_resp(r, response)
 
 
-@pytest_asyncio.fixture(scope="session")
-def master_host(request):
-    url = request.config.getoption("--redis-url")
-    parts = urlparse(url)
-    return parts.hostname
-
-
 async def wait_for_command(
     client: redis.Redis, monitor: Monitor, command: str, key: Union[str, None] = None
 ):
     # issue a command with a key name that's local to this process.
     # if we find a command with our key before the command we're waiting
     # for, something went wrong
     if key is None:
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/mocks.py` & `redis-5.0.0rc2/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_bloom.py` & `redis-5.0.0rc2/tests/test_asyncio/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_cluster.py` & `redis-5.0.0rc2/tests/test_asyncio/test_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 import binascii
 import datetime
-import os
 import warnings
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Type, Union
 from urllib.parse import urlparse
 
 import pytest
 import pytest_asyncio
 from _pytest.fixtures import FixtureRequest
+from redis._parsers import AsyncCommandsParser
 from redis.asyncio.cluster import ClusterNode, NodesManager, RedisCluster
-from redis.asyncio.connection import Connection, SSLConnection
+from redis.asyncio.connection import Connection, SSLConnection, async_timeout
 from redis.asyncio.retry import Retry
 from redis.backoff import ExponentialBackoff, NoBackoff, default_backoff
 from redis.cluster import PIPELINE_BLOCKED_COMMANDS, PRIMARY, REPLICA, get_node_name
 from redis.crc import REDIS_CLUSTER_HASH_SLOTS, key_slot
 from redis.exceptions import (
     AskError,
     ClusterDownError,
@@ -23,36 +23,89 @@
     MaxConnectionsError,
     MovedError,
     NoPermissionError,
     RedisClusterException,
     RedisError,
     ResponseError,
 )
-from redis.parsers import AsyncCommandsParser
 from redis.utils import str_if_bytes
 from tests.conftest import (
     assert_resp_response,
     skip_if_redis_enterprise,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
 )
 
+from ..ssl_utils import get_ssl_filename
 from .compat import mock
 
 pytestmark = pytest.mark.onlycluster
 
 
 default_host = "127.0.0.1"
 default_port = 7000
 default_cluster_slots = [
     [0, 8191, ["127.0.0.1", 7000, "node_0"], ["127.0.0.1", 7003, "node_3"]],
     [8192, 16383, ["127.0.0.1", 7001, "node_1"], ["127.0.0.1", 7002, "node_2"]],
 ]
 
 
+class NodeProxy:
+    """A class to proxy a node connection to a different port"""
+
+    def __init__(self, addr, redis_addr):
+        self.addr = addr
+        self.redis_addr = redis_addr
+        self.send_event = asyncio.Event()
+        self.server = None
+        self.task = None
+        self.n_connections = 0
+
+    async def start(self):
+        # test that we can connect to redis
+        async with async_timeout(2):
+            _, redis_writer = await asyncio.open_connection(*self.redis_addr)
+        redis_writer.close()
+        self.server = await asyncio.start_server(
+            self.handle, *self.addr, reuse_address=True
+        )
+        self.task = asyncio.create_task(self.server.serve_forever())
+
+    async def handle(self, reader, writer):
+        # establish connection to redis
+        redis_reader, redis_writer = await asyncio.open_connection(*self.redis_addr)
+        try:
+            self.n_connections += 1
+            pipe1 = asyncio.create_task(self.pipe(reader, redis_writer))
+            pipe2 = asyncio.create_task(self.pipe(redis_reader, writer))
+            await asyncio.gather(pipe1, pipe2)
+        finally:
+            redis_writer.close()
+
+    async def aclose(self):
+        self.task.cancel()
+        try:
+            await self.task
+        except asyncio.CancelledError:
+            pass
+        await self.server.wait_closed()
+
+    async def pipe(
+        self,
+        reader: asyncio.StreamReader,
+        writer: asyncio.StreamWriter,
+    ):
+        while True:
+            data = await reader.read(1000)
+            if not data:
+                break
+            writer.write(data)
+            await writer.drain()
+
+
 @pytest_asyncio.fixture()
 async def slowlog(r: RedisCluster) -> None:
     """
     Set the slowlog threshold to 0, and the
     max length to 128. This will force every
     command into the slowlog and allow us
     to test it
@@ -336,31 +389,14 @@
         async with RedisCluster.from_url(url) as rc:
             await rc.set("a", 1)
             await rc.get("a") == 1
 
         rc = RedisCluster.from_url("rediss://localhost:16379")
         assert rc.connection_kwargs["connection_class"] is SSLConnection
 
-    async def test_asynckills(self, r) -> None:
-
-        await r.set("foo", "foo")
-        await r.set("bar", "bar")
-
-        t = asyncio.create_task(r.get("foo"))
-        await asyncio.sleep(1)
-        t.cancel()
-        try:
-            await t
-        except asyncio.CancelledError:
-            pytest.fail("connection is left open with unread response")
-
-        assert await r.get("bar") == b"bar"
-        assert await r.ping()
-        assert await r.get("foo") == b"foo"
-
     async def test_max_connections(
         self, create_redis: Callable[..., RedisCluster]
     ) -> None:
         rc = await create_redis(cls=RedisCluster, max_connections=10)
         for node in rc.get_nodes():
             assert node.max_connections == 10
 
@@ -822,14 +858,57 @@
         # Test that the command succeed from a different node
         nodes = await r.cluster_nodes()
         assert "myself" not in nodes.get(curr_default_node.name).get("flags")
         assert r.get_default_node() != curr_default_node
         # Rollback to the old default node
         r.replace_default_node(curr_default_node)
 
+    async def test_address_remap(self, create_redis, master_host):
+        """Test that we can create a rediscluster object with
+        a host-port remapper and map connections through proxy objects
+        """
+
+        # we remap the first n nodes
+        offset = 1000
+        n = 6
+        hostname, master_port = master_host
+        ports = [master_port + i for i in range(n)]
+
+        def address_remap(address):
+            # remap first three nodes to our local proxy
+            # old = host, port
+            host, port = address
+            if int(port) in ports:
+                host, port = "127.0.0.1", int(port) + offset
+            # print(f"{old} {host, port}")
+            return host, port
+
+        # create the proxies
+        proxies = [
+            NodeProxy(("127.0.0.1", port + offset), (hostname, port)) for port in ports
+        ]
+        await asyncio.gather(*[p.start() for p in proxies])
+        try:
+            # create cluster:
+            r = await create_redis(
+                cls=RedisCluster, flushdb=False, address_remap=address_remap
+            )
+            try:
+                assert await r.ping() is True
+                assert await r.set("byte_string", b"giraffe")
+                assert await r.get("byte_string") == b"giraffe"
+            finally:
+                await r.close()
+        finally:
+            await asyncio.gather(*[p.aclose() for p in proxies])
+
+        # verify that the proxies were indeed used
+        n_used = sum((1 if p.n_connections else 0) for p in proxies)
+        assert n_used > 1
+
 
 class TestClusterRedisCommands:
     """
     Tests for RedisCluster unique commands
     """
 
     async def test_get_and_set(self, r: RedisCluster) -> None:
@@ -881,15 +960,15 @@
             reset_commands_processed = node_info["total_commands_processed"]
             assert reset_commands_processed < prior_commands_processed
 
     async def test_client_setname(self, r: RedisCluster) -> None:
         node = r.get_random_node()
         await r.client_setname("redis_py_test", target_nodes=node)
         client_name = await r.client_getname(target_nodes=node)
-        assert client_name == "redis_py_test"
+        assert_resp_response(r, client_name, "redis_py_test", b"redis_py_test")
 
     async def test_exists(self, r: RedisCluster) -> None:
         d = {"a": b"1", "b": b"2", "c": b"3", "d": b"4"}
         await r.mset_nonatomic(d)
         assert await r.exists(*d.keys()) == len(d)
 
     async def test_delete(self, r: RedisCluster) -> None:
@@ -923,14 +1002,21 @@
 
     @skip_if_redis_enterprise()
     async def test_cluster_myid(self, r: RedisCluster) -> None:
         node = r.get_random_node()
         myid = await r.cluster_myid(node)
         assert len(myid) == 40
 
+    @skip_if_server_version_lt("7.2.0")
+    @skip_if_redis_enterprise()
+    async def test_cluster_myshardid(self, r: RedisCluster) -> None:
+        node = r.get_random_node()
+        myshardid = await r.cluster_myshardid(node)
+        assert len(myshardid) == 40
+
     @skip_if_redis_enterprise()
     async def test_cluster_slots(self, r: RedisCluster) -> None:
         mock_all_nodes_resp(r, default_cluster_slots)
         cluster_slots = await r.cluster_slots()
         assert isinstance(cluster_slots, dict)
         assert len(default_cluster_slots) == len(cluster_slots)
         assert cluster_slots.get((0, 8191)) is not None
@@ -1353,15 +1439,15 @@
         assert reset_commands_processed < prior_commands_processed
 
     @skip_if_server_version_lt("6.2.0")
     async def test_client_trackinginfo(self, r: RedisCluster) -> None:
         node = r.get_primaries()[0]
         res = await r.client_trackinginfo(target_nodes=node)
         assert len(res) > 2
-        assert "prefixes" in res
+        assert "prefixes" in res or b"prefixes" in res
 
     @skip_if_server_version_lt("2.9.50")
     async def test_client_pause(self, r: RedisCluster) -> None:
         node = r.get_primaries()[0]
         assert await r.client_pause(1, target_nodes=node)
         assert await r.client_pause(timeout=1, target_nodes=node)
         with pytest.raises(RedisError):
@@ -1519,32 +1605,76 @@
         assert await r.get("{foo}a") == b"1"
         assert await r.get("{foo}b") == b"2"
 
     # LIST COMMANDS
     async def test_cluster_blpop(self, r: RedisCluster) -> None:
         await r.rpush("{foo}a", "1", "2")
         await r.rpush("{foo}b", "3", "4")
-        assert await r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"3")
-        assert await r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"4")
-        assert await r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"1")
-        assert await r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"2")
+        assert_resp_response(
+            r,
+            await r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"3"),
+            [b"{foo}b", b"3"],
+        )
+        assert_resp_response(
+            r,
+            await r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"4"),
+            [b"{foo}b", b"4"],
+        )
+        assert_resp_response(
+            r,
+            await r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"1"),
+            [b"{foo}a", b"1"],
+        )
+        assert_resp_response(
+            r,
+            await r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"2"),
+            [b"{foo}a", b"2"],
+        )
         assert await r.blpop(["{foo}b", "{foo}a"], timeout=1) is None
         await r.rpush("{foo}c", "1")
-        assert await r.blpop("{foo}c", timeout=1) == (b"{foo}c", b"1")
+        assert_resp_response(
+            r, await r.blpop("{foo}c", timeout=1), (b"{foo}c", b"1"), [b"{foo}c", b"1"]
+        )
 
     async def test_cluster_brpop(self, r: RedisCluster) -> None:
         await r.rpush("{foo}a", "1", "2")
         await r.rpush("{foo}b", "3", "4")
-        assert await r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"4")
-        assert await r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"3")
-        assert await r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"2")
-        assert await r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"1")
+        assert_resp_response(
+            r,
+            await r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"4"),
+            [b"{foo}b", b"4"],
+        )
+        assert_resp_response(
+            r,
+            await r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"3"),
+            [b"{foo}b", b"3"],
+        )
+        assert_resp_response(
+            r,
+            await r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"2"),
+            [b"{foo}a", b"2"],
+        )
+        assert_resp_response(
+            r,
+            await r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"1"),
+            [b"{foo}a", b"1"],
+        )
         assert await r.brpop(["{foo}b", "{foo}a"], timeout=1) is None
         await r.rpush("{foo}c", "1")
-        assert await r.brpop("{foo}c", timeout=1) == (b"{foo}c", b"1")
+        assert_resp_response(
+            r, await r.brpop("{foo}c", timeout=1), (b"{foo}c", b"1"), [b"{foo}c", b"1"]
+        )
 
     async def test_cluster_brpoplpush(self, r: RedisCluster) -> None:
         await r.rpush("{foo}a", "1", "2")
         await r.rpush("{foo}b", "3", "4")
         assert await r.brpoplpush("{foo}a", "{foo}b") == b"2"
         assert await r.brpoplpush("{foo}a", "{foo}b") == b"1"
         assert await r.brpoplpush("{foo}a", "{foo}b", timeout=1) is None
@@ -1721,65 +1851,83 @@
             [[b"a3", 20.0], [b"a1", 23.0]],
         )
 
     @skip_if_server_version_lt("4.9.0")
     async def test_cluster_bzpopmax(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2})
         await r.zadd("{foo}b", {"b1": 10, "b2": 20})
-        assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}b",
-            b"b2",
-            20,
-        )
-        assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}b",
-            b"b1",
-            10,
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b2", 20),
+            [b"{foo}b", b"b2", 20],
         )
-        assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}a",
-            b"a2",
-            2,
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b1", 10),
+            [b"{foo}b", b"b1", 10],
         )
-        assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}a",
-            b"a1",
-            1,
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a2", 2),
+            [b"{foo}a", b"a2", 2],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a1", 1),
+            [b"{foo}a", b"a1", 1],
         )
         assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) is None
         await r.zadd("{foo}c", {"c1": 100})
-        assert await r.bzpopmax("{foo}c", timeout=1) == (b"{foo}c", b"c1", 100)
+        assert_resp_response(
+            r,
+            await r.bzpopmax("{foo}c", timeout=1),
+            (b"{foo}c", b"c1", 100),
+            [b"{foo}c", b"c1", 100],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     async def test_cluster_bzpopmin(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2})
         await r.zadd("{foo}b", {"b1": 10, "b2": 20})
-        assert await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}b",
-            b"b1",
-            10,
-        )
-        assert await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}b",
-            b"b2",
-            20,
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b1", 10),
+            [b"b", b"b1", 10],
         )
-        assert await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}a",
-            b"a1",
-            1,
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b2", 20),
+            [b"b", b"b2", 20],
         )
-        assert await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (
-            b"{foo}a",
-            b"a2",
-            2,
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a1", 1),
+            [b"a", b"a1", 1],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a2", 2),
+            [b"a", b"a2", 2],
         )
         assert await r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) is None
         await r.zadd("{foo}c", {"c1": 100})
-        assert await r.bzpopmin("{foo}c", timeout=1) == (b"{foo}c", b"c1", 100)
+        assert_resp_response(
+            r,
+            await r.bzpopmin("{foo}c", timeout=1),
+            (b"{foo}c", b"c1", 100),
+            [b"{foo}c", b"c1", 100],
+        )
 
     @skip_if_server_version_lt("6.2.0")
     async def test_cluster_zrangestore(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         assert await r.zrangestore("{foo}b", "{foo}a", 0, 1)
         assert await r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         assert await r.zrangestore("{foo}b", "{foo}a", 1, 2)
@@ -2686,25 +2834,16 @@
     """
     Tests for SSL connections.
 
     This relies on the --redis-ssl-url for building the client and connecting to the
     appropriate port.
     """
 
-    ROOT = os.path.join(os.path.dirname(__file__), "../..")
-    CERT_DIR = os.path.abspath(os.path.join(ROOT, "dockers", "stunnel", "keys"))
-    if not os.path.isdir(CERT_DIR):  # github actions package validation case
-        CERT_DIR = os.path.abspath(
-            os.path.join(ROOT, "..", "dockers", "stunnel", "keys")
-        )
-        if not os.path.isdir(CERT_DIR):
-            raise IOError(f"No SSL certificates found. They should be in {CERT_DIR}")
-
-    SERVER_CERT = os.path.join(CERT_DIR, "server-cert.pem")
-    SERVER_KEY = os.path.join(CERT_DIR, "server-key.pem")
+    SERVER_CERT = get_ssl_filename("server-cert.pem")
+    SERVER_KEY = get_ssl_filename("server-key.pem")
 
     @pytest_asyncio.fixture()
     def create_client(self, request: FixtureRequest) -> Callable[..., RedisCluster]:
         ssl_url = request.config.option.redis_ssl_url
         ssl_host, ssl_port = urlparse(ssl_url)[1].split(":")
 
         async def _create_client(mocked: bool = True, **kwargs: Any) -> RedisCluster:
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_commands.py` & `redis-5.0.0rc2/tests/test_asyncio/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 """
 Tests async overrides of commands from their mixins
 """
+import asyncio
 import binascii
 import datetime
 import re
+import sys
 from string import ascii_letters
 
 import pytest
 import pytest_asyncio
 import redis
 from redis import exceptions
-from redis.client import EMPTY_RESPONSE, NEVER_DECODE, parse_info
+from redis._parsers.helpers import (
+    _RedisCallbacks,
+    _RedisCallbacksRESP2,
+    _RedisCallbacksRESP3,
+    parse_info,
+)
+from redis.client import EMPTY_RESPONSE, NEVER_DECODE
 from tests.conftest import (
     assert_resp_response,
     assert_resp_response_in,
     is_resp2_connection,
     skip_if_server_version_gte,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
 )
 
+if sys.version_info >= (3, 11, 3):
+    from asyncio import timeout as async_timeout
+else:
+    from async_timeout import timeout as async_timeout
+
 REDIS_6_VERSION = "5.9.0"
 
 
 @pytest_asyncio.fixture()
 async def r_teardown(r: redis.Redis):
     """
     A special fixture which removes the provided names from the database after use
@@ -69,21 +82,21 @@
 
 # RESPONSE CALLBACKS
 @pytest.mark.onlynoncluster
 class TestResponseCallbacks:
     """Tests for the response callback system"""
 
     async def test_response_callbacks(self, r: redis.Redis):
-        callbacks = redis.Redis.RESPONSE_CALLBACKS
+        callbacks = _RedisCallbacks
         if is_resp2_connection(r):
-            callbacks.update(redis.Redis.RESP2_RESPONSE_CALLBACKS)
+            callbacks.update(_RedisCallbacksRESP2)
         else:
-            callbacks.update(redis.Redis.RESP3_RESPONSE_CALLBACKS)
+            callbacks.update(_RedisCallbacksRESP3)
         assert r.response_callbacks == callbacks
-        assert id(r.response_callbacks) != id(redis.Redis.RESPONSE_CALLBACKS)
+        assert id(r.response_callbacks) != id(_RedisCallbacks)
         r.set_response_callback("GET", lambda x: "static")
         await r.set("a", "foo")
         assert await r.get("a") == "static"
 
     async def test_case_insensitive_command_names(self, r: redis.Redis):
         assert r.response_callbacks["ping"] == r.response_callbacks["PING"]
 
@@ -95,35 +108,35 @@
             await r.get("a")
 
     # SERVER INFORMATION
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_cat_no_category(self, r: redis.Redis):
         categories = await r.acl_cat()
         assert isinstance(categories, list)
-        assert "read" in categories
+        assert "read" in categories or b"read" in categories
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_cat_with_category(self, r: redis.Redis):
         commands = await r.acl_cat("read")
         assert isinstance(commands, list)
-        assert "get" in commands
+        assert "get" in commands or b"get" in commands
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_deluser(self, r_teardown):
         username = "redis-py-user"
         r = r_teardown(username)
 
         assert await r.acl_deluser(username) == 0
         assert await r.acl_setuser(username, enabled=False, reset=True)
         assert await r.acl_deluser(username) == 1
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_genpass(self, r: redis.Redis):
         password = await r.acl_genpass()
-        assert isinstance(password, str)
+        assert isinstance(password, (str, bytes))
 
     @skip_if_server_version_lt("7.0.0")
     async def test_acl_getuser_setuser(self, r_teardown):
         username = "redis-py-user"
         r = r_teardown(username)
         # test enabled=False
         assert await r.acl_setuser(username, enabled=False, reset=True)
@@ -296,15 +309,15 @@
         users = await r.acl_users()
         assert isinstance(users, list)
         assert len(users) > 0
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_whoami(self, r: redis.Redis):
         username = await r.acl_whoami()
-        assert isinstance(username, str)
+        assert isinstance(username, (str, bytes))
 
     @pytest.mark.onlynoncluster
     async def test_client_list(self, r: redis.Redis):
         clients = await r.client_list()
         assert isinstance(clients[0], dict)
         assert "addr" in clients[0]
 
@@ -334,15 +347,17 @@
     async def test_client_getname(self, r: redis.Redis):
         assert await r.client_getname() is None
 
     @skip_if_server_version_lt("2.6.9")
     @pytest.mark.onlynoncluster
     async def test_client_setname(self, r: redis.Redis):
         assert await r.client_setname("redis_py_test")
-        assert await r.client_getname() == "redis_py_test"
+        assert_resp_response(
+            r, await r.client_getname(), "redis_py_test", b"redis_py_test"
+        )
 
     @skip_if_server_version_lt("2.6.9")
     @pytest.mark.onlynoncluster
     async def test_client_kill(self, r: redis.Redis, r2):
         await r.client_setname("redis-py-c1")
         await r2.client_setname("redis-py-c2")
         clients = [
@@ -442,14 +457,36 @@
     @pytest.mark.onlynoncluster
     async def test_client_pause(self, r: redis.Redis):
         assert await r.client_pause(1)
         assert await r.client_pause(timeout=1)
         with pytest.raises(exceptions.RedisError):
             await r.client_pause(timeout="not an integer")
 
+    @skip_if_server_version_lt("7.2.0")
+    @pytest.mark.onlynoncluster
+    async def test_client_no_touch(self, r: redis.Redis):
+        assert await r.client_no_touch("ON") == b"OK"
+        assert await r.client_no_touch("OFF") == b"OK"
+        with pytest.raises(TypeError):
+            await r.client_no_touch()
+
+    @skip_if_server_version_lt("7.2.0")
+    @pytest.mark.onlycluster
+    async def test_waitaof(self, r):
+        # must return a list of 2 elements
+        assert len(await r.waitaof(0, 0, 0)) == 2
+        assert len(await r.waitaof(1, 0, 0)) == 2
+        assert len(await r.waitaof(1, 0, 1000)) == 2
+
+        # value is out of range, value must between 0 and 1
+        with pytest.raises(exceptions.ResponseError):
+            await r.waitaof(2, 0, 0)
+        with pytest.raises(exceptions.ResponseError):
+            await r.waitaof(-1, 0, 0)
+
     async def test_config_get(self, r: redis.Redis):
         data = await r.config_get()
         assert "maxmemory" in data
         assert data["maxmemory"].isdigit()
 
     @pytest.mark.onlynoncluster
     async def test_config_resetstat(self, r: redis.Redis):
@@ -1060,33 +1097,53 @@
         assert await r.type("a") == b"zset"
 
     # LIST COMMANDS
     @pytest.mark.onlynoncluster
     async def test_blpop(self, r: redis.Redis):
         await r.rpush("a", "1", "2")
         await r.rpush("b", "3", "4")
-        assert await r.blpop(["b", "a"], timeout=1) == (b"b", b"3")
-        assert await r.blpop(["b", "a"], timeout=1) == (b"b", b"4")
-        assert await r.blpop(["b", "a"], timeout=1) == (b"a", b"1")
-        assert await r.blpop(["b", "a"], timeout=1) == (b"a", b"2")
+        assert_resp_response(
+            r, await r.blpop(["b", "a"], timeout=1), (b"b", b"3"), [b"b", b"3"]
+        )
+        assert_resp_response(
+            r, await r.blpop(["b", "a"], timeout=1), (b"b", b"4"), [b"b", b"4"]
+        )
+        assert_resp_response(
+            r, await r.blpop(["b", "a"], timeout=1), (b"a", b"1"), [b"a", b"1"]
+        )
+        assert_resp_response(
+            r, await r.blpop(["b", "a"], timeout=1), (b"a", b"2"), [b"a", b"2"]
+        )
         assert await r.blpop(["b", "a"], timeout=1) is None
         await r.rpush("c", "1")
-        assert await r.blpop("c", timeout=1) == (b"c", b"1")
+        assert_resp_response(
+            r, await r.blpop("c", timeout=1), (b"c", b"1"), [b"c", b"1"]
+        )
 
     @pytest.mark.onlynoncluster
     async def test_brpop(self, r: redis.Redis):
         await r.rpush("a", "1", "2")
         await r.rpush("b", "3", "4")
-        assert await r.brpop(["b", "a"], timeout=1) == (b"b", b"4")
-        assert await r.brpop(["b", "a"], timeout=1) == (b"b", b"3")
-        assert await r.brpop(["b", "a"], timeout=1) == (b"a", b"2")
-        assert await r.brpop(["b", "a"], timeout=1) == (b"a", b"1")
+        assert_resp_response(
+            r, await r.brpop(["b", "a"], timeout=1), (b"b", b"4"), [b"b", b"4"]
+        )
+        assert_resp_response(
+            r, await r.brpop(["b", "a"], timeout=1), (b"b", b"3"), [b"b", b"3"]
+        )
+        assert_resp_response(
+            r, await r.brpop(["b", "a"], timeout=1), (b"a", b"2"), [b"a", b"2"]
+        )
+        assert_resp_response(
+            r, await r.brpop(["b", "a"], timeout=1), (b"a", b"1"), [b"a", b"1"]
+        )
         assert await r.brpop(["b", "a"], timeout=1) is None
         await r.rpush("c", "1")
-        assert await r.brpop("c", timeout=1) == (b"c", b"1")
+        assert_resp_response(
+            r, await r.brpop("c", timeout=1), (b"c", b"1"), [b"c", b"1"]
+        )
 
     @pytest.mark.onlynoncluster
     async def test_brpoplpush(self, r: redis.Redis):
         await r.rpush("a", "1", "2")
         await r.rpush("b", "3", "4")
         assert await r.brpoplpush("a", "b") == b"2"
         assert await r.brpoplpush("a", "b") == b"1"
@@ -1593,34 +1650,78 @@
         )
 
     @skip_if_server_version_lt("4.9.0")
     @pytest.mark.onlynoncluster
     async def test_bzpopmax(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2})
         await r.zadd("b", {"b1": 10, "b2": 20})
-        assert await r.bzpopmax(["b", "a"], timeout=1) == (b"b", b"b2", 20)
-        assert await r.bzpopmax(["b", "a"], timeout=1) == (b"b", b"b1", 10)
-        assert await r.bzpopmax(["b", "a"], timeout=1) == (b"a", b"a2", 2)
-        assert await r.bzpopmax(["b", "a"], timeout=1) == (b"a", b"a1", 1)
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["b", "a"], timeout=1),
+            (b"b", b"b2", 20),
+            [b"b", b"b2", 20],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["b", "a"], timeout=1),
+            (b"b", b"b1", 10),
+            [b"b", b"b1", 10],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["b", "a"], timeout=1),
+            (b"a", b"a2", 2),
+            [b"a", b"a2", 2],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmax(["b", "a"], timeout=1),
+            (b"a", b"a1", 1),
+            [b"a", b"a1", 1],
+        )
         assert await r.bzpopmax(["b", "a"], timeout=1) is None
         await r.zadd("c", {"c1": 100})
-        assert await r.bzpopmax("c", timeout=1) == (b"c", b"c1", 100)
+        assert_resp_response(
+            r, await r.bzpopmax("c", timeout=1), (b"c", b"c1", 100), [b"c", b"c1", 100]
+        )
 
     @skip_if_server_version_lt("4.9.0")
     @pytest.mark.onlynoncluster
     async def test_bzpopmin(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2})
         await r.zadd("b", {"b1": 10, "b2": 20})
-        assert await r.bzpopmin(["b", "a"], timeout=1) == (b"b", b"b1", 10)
-        assert await r.bzpopmin(["b", "a"], timeout=1) == (b"b", b"b2", 20)
-        assert await r.bzpopmin(["b", "a"], timeout=1) == (b"a", b"a1", 1)
-        assert await r.bzpopmin(["b", "a"], timeout=1) == (b"a", b"a2", 2)
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["b", "a"], timeout=1),
+            (b"b", b"b1", 10),
+            [b"b", b"b1", 10],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["b", "a"], timeout=1),
+            (b"b", b"b2", 20),
+            [b"b", b"b2", 20],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["b", "a"], timeout=1),
+            (b"a", b"a1", 1),
+            [b"a", b"a1", 1],
+        )
+        assert_resp_response(
+            r,
+            await r.bzpopmin(["b", "a"], timeout=1),
+            (b"a", b"a2", 2),
+            [b"a", b"a2", 2],
+        )
         assert await r.bzpopmin(["b", "a"], timeout=1) is None
         await r.zadd("c", {"c1": 100})
-        assert await r.bzpopmin("c", timeout=1) == (b"c", b"c1", 100)
+        assert_resp_response(
+            r, await r.bzpopmin("c", timeout=1), (b"c", b"c1", 100), [b"c", b"c1", 100]
+        )
 
     async def test_zrange(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert await r.zrange("a", 0, 1) == [b"a1", b"a2"]
         assert await r.zrange("a", 1, 2) == [b"a2", b"a3"]
 
         # withscores
@@ -1692,14 +1793,23 @@
 
     async def test_zrank(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert await r.zrank("a", "a1") == 0
         assert await r.zrank("a", "a2") == 1
         assert await r.zrank("a", "a6") is None
 
+    @skip_if_server_version_lt("7.2.0")
+    async def test_zrank_withscore(self, r: redis.Redis):
+        await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
+        assert await r.zrank("a", "a1") == 0
+        assert await r.rank("a", "a2") == 1
+        assert await r.zrank("a", "a6") is None
+        assert await r.zrank("a", "a3", withscore=True) == [2, "3"]
+        assert await r.zrank("a", "a6", withscore=True) is None
+
     async def test_zrem(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert await r.zrem("a", "a2") == 1
         assert await r.zrange("a", 0, -1) == [b"a1", b"a3"]
         assert await r.zrem("a", "b") == 0
         assert await r.zrange("a", 0, -1) == [b"a1", b"a3"]
 
@@ -1780,14 +1890,23 @@
 
     async def test_zrevrank(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert await r.zrevrank("a", "a1") == 4
         assert await r.zrevrank("a", "a2") == 3
         assert await r.zrevrank("a", "a6") is None
 
+    @skip_if_server_version_lt("7.2.0")
+    async def test_zrevrank_withscore(self, r: redis.Redis):
+        await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
+        assert await r.zrevrank("a", "a1") == 4
+        assert await r.zrevrank("a", "a2") == 3
+        assert await r.zrevrank("a", "a6") is None
+        assert await r.zrevrank("a", "a3", withscore=True) == [2, "3"]
+        assert await r.zrevrank("a", "a6", withscore=True) is None
+
     async def test_zscore(self, r: redis.Redis):
         await r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert await r.zscore("a", "a1") == 1.0
         assert await r.zscore("a", "a2") == 2.0
         assert await r.zscore("a", "a4") is None
 
     @pytest.mark.onlynoncluster
@@ -2281,34 +2400,43 @@
         values = (2.1909389952632, 41.433791470673, "place1") + (
             2.1873744593677,
             41.406342043777,
             "place2",
         )
 
         await r.geoadd("barcelona", values)
-        assert await r.geohash("barcelona", "place1", "place2", "place3") == [
-            "sp3e9yg3kd0",
-            "sp3e9cbc3t0",
-            None,
-        ]
+        assert_resp_response(
+            r,
+            await r.geohash("barcelona", "place1", "place2", "place3"),
+            ["sp3e9yg3kd0", "sp3e9cbc3t0", None],
+            [b"sp3e9yg3kd0", b"sp3e9cbc3t0", None],
+        )
 
     @skip_if_server_version_lt("3.2.0")
     async def test_geopos(self, r: redis.Redis):
         values = (2.1909389952632, 41.433791470673, "place1") + (
             2.1873744593677,
             41.406342043777,
             "place2",
         )
 
         await r.geoadd("barcelona", values)
         # redis uses 52 bits precision, hereby small errors may be introduced.
-        assert await r.geopos("barcelona", "place1", "place2") == [
-            (2.19093829393386841, 41.43379028184083523),
-            (2.18737632036209106, 41.40634178640635099),
-        ]
+        assert_resp_response(
+            r,
+            await r.geopos("barcelona", "place1", "place2"),
+            [
+                (2.19093829393386841, 41.43379028184083523),
+                (2.18737632036209106, 41.40634178640635099),
+            ],
+            [
+                [2.19093829393386841, 41.43379028184083523],
+                [2.18737632036209106, 41.40634178640635099],
+            ],
+        )
 
     @skip_if_server_version_lt("4.0.0")
     async def test_geopos_no_value(self, r: redis.Redis):
         assert await r.geopos("barcelona", "place1", "place2") == [None, None]
 
     @skip_if_server_version_lt("3.2.0")
     @skip_if_server_version_gte("4.0.0")
@@ -3075,14 +3203,45 @@
     @skip_if_server_version_lt("4.0.0")
     @pytest.mark.onlynoncluster
     async def test_module_list(self, r: redis.Redis):
         assert isinstance(await r.module_list(), list)
         for x in await r.module_list():
             assert isinstance(x, dict)
 
+    @pytest.mark.onlynoncluster
+    async def test_interrupted_command(self, r: redis.Redis):
+        """
+        Regression test for issue #1128:  An Un-handled BaseException
+        will leave the socket with un-read response to a previous
+        command.
+        """
+        ready = asyncio.Event()
+
+        async def helper():
+            with pytest.raises(asyncio.CancelledError):
+                # blocking pop
+                ready.set()
+                await r.brpop(["nonexist"])
+            # If the following is not done, further Timout operations will fail,
+            # because the timeout won't catch its Cancelled Error if the task
+            # has a pending cancel.  Python documentation probably should reflect this.
+            if sys.version_info >= (3, 11):
+                asyncio.current_task().uncancel()
+            # if all is well, we can continue.  The following should not hang.
+            await r.set("status", "down")
+
+        task = asyncio.create_task(helper())
+        await ready.wait()
+        await asyncio.sleep(0.01)
+        # the task is now sleeping, lets send it an exception
+        task.cancel()
+        # If all is well, the task should finish right away, otherwise fail with Timeout
+        async with async_timeout(1.0):
+            await task
+
 
 @pytest.mark.onlynoncluster
 class TestBinarySave:
     async def test_binary_get_set(self, r: redis.Redis):
         assert await r.set(" foo bar ", "123")
         assert await r.get(" foo bar ") == b"123"
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_connection.py` & `redis-5.0.0rc2/tests/test_asyncio/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
 import socket
 import types
 from unittest.mock import patch
 
 import pytest
 import redis
-from redis.asyncio import Redis
-from redis.asyncio.connection import Connection, UnixDomainSocketConnection
-from redis.asyncio.retry import Retry
-from redis.backoff import NoBackoff
-from redis.exceptions import ConnectionError, InvalidResponse, TimeoutError
-from redis.parsers import (
+from redis._parsers import (
     _AsyncHiredisParser,
     _AsyncRESP2Parser,
     _AsyncRESP3Parser,
     _AsyncRESPBase,
 )
+from redis.asyncio import Redis
+from redis.asyncio.connection import Connection, UnixDomainSocketConnection
+from redis.asyncio.retry import Retry
+from redis.backoff import NoBackoff
+from redis.exceptions import ConnectionError, InvalidResponse, TimeoutError
 from redis.utils import HIREDIS_AVAILABLE
 from tests.conftest import skip_if_server_version_lt
 
 from .compat import mock
 from .mocks import MockStream
 
 
@@ -39,35 +39,14 @@
     else:
         assert (
             str(cm.value) == f'Protocol error, got "{raw.decode()}" as reply type byte'
         )
     await r.connection.disconnect()
 
 
-async def test_asynckills():
-
-    for b in [True, False]:
-        r = Redis(single_connection_client=b)
-
-        await r.set("foo", "foo")
-        await r.set("bar", "bar")
-
-        t = asyncio.create_task(r.get("foo"))
-        await asyncio.sleep(1)
-        t.cancel()
-        try:
-            await t
-        except asyncio.CancelledError:
-            pytest.fail("connection left open with unread response")
-
-        assert await r.get("bar") == b"bar"
-        assert await r.ping()
-        assert await r.get("foo") == b"foo"
-
-
 @pytest.mark.onlynoncluster
 async def test_single_connection():
     """Test that concurrent requests on a single client are synchronised."""
     r = Redis(single_connection_client=True)
 
     init_call_count = 0
     command_call_count = 0
@@ -200,15 +179,15 @@
         b"*3\r\n$7\r\nmessage\r\n$8\r\nchannel1\r\n"
         b"$25\r\nhi\r\nthere\r\n+how\r\nare\r\nyou\r\n"
     )
 
     conn._parser._stream = MockStream(message, interrupt_every=2)
     for i in range(100):
         try:
-            response = await conn.read_response()
+            response = await conn.read_response(disconnect_on_error=False)
             break
         except MockStream.TestError:
             pass
 
     else:
         pytest.fail("didn't receive a response")
     assert response
@@ -289,7 +268,13 @@
         return reader, writer
 
     with patch.object(asyncio, "open_connection", open_connection):
         await conn.connect()
 
     vals = await asyncio.gather(do_read(), do_close())
     assert vals == [b"Hello, World!", None]
+
+
+@pytest.mark.onlynoncluster
+def test_create_single_connection_client_from_url():
+    client = Redis.from_url("redis://localhost:6379/0?", single_connection_client=True)
+    assert client.single_connection_client is True
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_connection_pool.py` & `redis-5.0.0rc2/tests/test_asyncio/test_connection_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,32 +131,32 @@
             connection_kwargs=connection_kwargs, connection_class=DummyConnection
         ) as pool:
             connection = await pool.get_connection("_")
             assert isinstance(connection, DummyConnection)
             assert connection.kwargs == connection_kwargs
 
     async def test_multiple_connections(self, master_host):
-        connection_kwargs = {"host": master_host}
+        connection_kwargs = {"host": master_host[0]}
         async with self.get_pool(connection_kwargs=connection_kwargs) as pool:
             c1 = await pool.get_connection("_")
             c2 = await pool.get_connection("_")
             assert c1 != c2
 
     async def test_max_connections(self, master_host):
-        connection_kwargs = {"host": master_host}
+        connection_kwargs = {"host": master_host[0]}
         async with self.get_pool(
             max_connections=2, connection_kwargs=connection_kwargs
         ) as pool:
             await pool.get_connection("_")
             await pool.get_connection("_")
             with pytest.raises(redis.ConnectionError):
                 await pool.get_connection("_")
 
     async def test_reuse_previously_released_connection(self, master_host):
-        connection_kwargs = {"host": master_host}
+        connection_kwargs = {"host": master_host[0]}
         async with self.get_pool(connection_kwargs=connection_kwargs) as pool:
             c1 = await pool.get_connection("_")
             await pool.release(c1)
             c2 = await pool.get_connection("_")
             assert c1 == c2
 
     async def test_repr_contains_db_info_tcp(self):
@@ -232,15 +232,15 @@
         async with self.get_pool(connection_kwargs=connection_kwargs) as pool:
             c1 = await pool.get_connection("_")
             c2 = await pool.get_connection("_")
             assert c1 != c2
 
     async def test_connection_pool_blocks_until_timeout(self, master_host):
         """When out of connections, block for timeout seconds, then raise"""
-        connection_kwargs = {"host": master_host}
+        connection_kwargs = {"host": master_host[0]}
         async with self.get_pool(
             max_connections=1, timeout=0.1, connection_kwargs=connection_kwargs
         ) as pool:
             c1 = await pool.get_connection("_")
 
             start = asyncio.get_running_loop().time()
             with pytest.raises(redis.ConnectionError):
@@ -267,15 +267,15 @@
 
             start = asyncio.get_running_loop().time()
             await asyncio.gather(target(), pool.get_connection("_"))
             stop = asyncio.get_running_loop().time()
             assert (stop - start) <= 0.2
 
     async def test_reuse_previously_released_connection(self, master_host):
-        connection_kwargs = {"host": master_host}
+        connection_kwargs = {"host": master_host[0]}
         async with self.get_pool(connection_kwargs=connection_kwargs) as pool:
             c1 = await pool.get_connection("_")
             await pool.release(c1)
             c2 = await pool.get_connection("_")
             assert c1 == c2
 
     def test_repr_contains_db_info_tcp(self):
@@ -603,18 +603,26 @@
         assert not pipe.connection
         assert len(pool._available_connections) == 1
         assert not pool._available_connections[0]._reader
 
     @skip_if_server_version_lt("2.8.8")
     @skip_if_redis_enterprise()
     async def test_read_only_error(self, r):
-        """READONLY errors get turned in ReadOnlyError exceptions"""
+        """READONLY errors get turned into ReadOnlyError exceptions"""
         with pytest.raises(redis.ReadOnlyError):
             await r.execute_command("DEBUG", "ERROR", "READONLY blah blah")
 
+    @skip_if_redis_enterprise()
+    async def test_oom_error(self, r):
+        """OOM errors get turned into OutOfMemoryError exceptions"""
+        with pytest.raises(redis.OutOfMemoryError):
+            # note: don't use the DEBUG OOM command since it's not the same
+            # as the db being full
+            await r.execute_command("DEBUG", "ERROR", "OOM blah blah")
+
     def test_connect_from_url_tcp(self):
         connection = redis.Redis.from_url("redis://localhost")
         pool = connection.connection_pool
 
         assert re.match("(.*)<(.*)<(.*)>>", repr(pool)).groups() == (
             "ConnectionPool",
             "Connection",
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_credentials.py` & `redis-5.0.0rc2/tests/test_asyncio/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_encoding.py` & `redis-5.0.0rc2/tests/test_asyncio/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_graph.py` & `redis-5.0.0rc2/tests/test_asyncio/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_json.py` & `redis-5.0.0rc2/tests/test_asyncio/test_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,49 @@
         decoded_r, await decoded_r.json().get("notascii", no_escape=True), res, [[res]]
     )
     assert 1 == await decoded_r.json().delete("notascii")
     assert await decoded_r.exists("notascii") == 0
 
 
 @pytest.mark.redismod
+@skip_ifmodversion_lt("2.6.0", "ReJSON")
+async def test_json_merge(decoded_r: redis.Redis):
+    # Test with root path $
+    assert await decoded_r.json().set(
+        "person_data",
+        "$",
+        {"person1": {"personal_data": {"name": "John"}}},
+    )
+    assert await decoded_r.json().merge(
+        "person_data", "$", {"person1": {"personal_data": {"hobbies": "reading"}}}
+    )
+    assert await decoded_r.json().get("person_data") == {
+        "person1": {"personal_data": {"name": "John", "hobbies": "reading"}}
+    }
+
+    # Test with root path path $.person1.personal_data
+    assert await decoded_r.json().merge(
+        "person_data", "$.person1.personal_data", {"country": "Israel"}
+    )
+    assert await decoded_r.json().get("person_data") == {
+        "person1": {
+            "personal_data": {"name": "John", "hobbies": "reading", "country": "Israel"}
+        }
+    }
+
+    # Test with null value to delete a value
+    assert await decoded_r.json().merge(
+        "person_data", "$.person1.personal_data", {"name": None}
+    )
+    assert await decoded_r.json().get("person_data") == {
+        "person1": {"personal_data": {"country": "Israel", "hobbies": "reading"}}
+    }
+
+
+@pytest.mark.redismod
 async def test_jsonsetexistentialmodifiersshouldsucceed(decoded_r: redis.Redis):
     obj = {"foo": "bar"}
     assert await decoded_r.json().set("obj", Path.root_path(), obj)
 
     # Test that flags prevent updates when conditions are unmet
     assert await decoded_r.json().set("obj", Path("foo"), "baz", nx=True) is None
     assert await decoded_r.json().set("obj", Path("qaz"), "baz", xx=True) is None
@@ -73,14 +108,25 @@
     await decoded_r.json().set("2", Path.root_path(), 2)
     assert await decoded_r.json().mget(["1"], Path.root_path()) == [1]
 
     assert await decoded_r.json().mget([1, 2], Path.root_path()) == [1, 2]
 
 
 @pytest.mark.redismod
+@skip_ifmodversion_lt("2.6.0", "ReJSON")
+async def test_mset(decoded_r: redis.Redis):
+    await decoded_r.json().mset(
+        [("1", Path.root_path(), 1), ("2", Path.root_path(), 2)]
+    )
+
+    assert await decoded_r.json().mget(["1"], Path.root_path()) == [1]
+    assert await decoded_r.json().mget(["1", "2"], Path.root_path()) == [1, 2]
+
+
+@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 async def test_clear(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 1 == await decoded_r.json().clear("arr", Path.root_path())
     assert_resp_response(decoded_r, await decoded_r.json().get("arr"), [], [[[]]])
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_lock.py` & `redis-5.0.0rc2/tests/test_asyncio/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_monitor.py` & `redis-5.0.0rc2/tests/test_asyncio/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_pipeline.py` & `redis-5.0.0rc2/tests/test_asyncio/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_pubsub.py` & `redis-5.0.0rc2/tests/test_asyncio/test_pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
 import functools
 import socket
 import sys
 from typing import Optional
 from unittest.mock import patch
 
-if sys.version_info.major >= 3 and sys.version_info.minor >= 11:
+# the functionality is available in 3.11.x but has a major issue before
+# 3.11.3. See https://github.com/redis/redis-py/issues/2633
+if sys.version_info >= (3, 11, 3):
     from asyncio import timeout as async_timeout
 else:
     from async_timeout import timeout as async_timeout
 
 import pytest
 import pytest_asyncio
 import redis.asyncio as redis
@@ -980,14 +982,17 @@
         # timeout waiting for another message which never arrives
         assert pubsub.connection.is_connected
         with pytest.raises(asyncio.TimeoutError):
             await get_msg_or_timeout()
         # the timeout on the read should not cause disconnect
         assert pubsub.connection.is_connected
 
+    @pytest.mark.skipif(
+        sys.version_info < (3, 8), reason="requires python 3.8 or higher"
+    )
     async def test_base_exception(self, r: redis.Redis):
         """
         Manually trigger a BaseException inside the parser's .read_response method
         and verify that it isn't caught
         """
         pubsub = r.pubsub()
         await pubsub.subscribe("foo")
@@ -1004,17 +1009,17 @@
                     return message
 
         # get subscribe message
         msg = await get_msg()
         assert msg is not None
         # timeout waiting for another message which never arrives
         assert pubsub.connection.is_connected
-        with patch("redis.parsers._AsyncRESP2Parser.read_response") as mock1, patch(
-            "redis.parsers._AsyncHiredisParser.read_response"
-        ) as mock2, patch("redis.parsers._AsyncRESP3Parser.read_response") as mock3:
+        with patch("redis._parsers._AsyncRESP2Parser.read_response") as mock1, patch(
+            "redis._parsers._AsyncHiredisParser.read_response"
+        ) as mock2, patch("redis._parsers._AsyncRESP3Parser.read_response") as mock3:
             mock1.side_effect = BaseException("boom")
             mock2.side_effect = BaseException("boom")
             mock3.side_effect = BaseException("boom")
 
             with pytest.raises(BaseException):
                 await get_msg()
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_retry.py` & `redis-5.0.0rc2/tests/test_asyncio/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_scripting.py` & `redis-5.0.0rc2/tests/test_asyncio/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_search.py` & `redis-5.0.0rc2/tests/test_asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_sentinel.py` & `redis-5.0.0rc2/tests/test_asyncio/test_sentinel.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SentinelConnectionPool,
     SlaveNotFoundError,
 )
 
 
 @pytest_asyncio.fixture(scope="module")
 def master_ip(master_host):
-    yield socket.gethostbyname(master_host)
+    yield socket.gethostbyname(master_host[0])
 
 
 class SentinelTestClient:
     def __init__(self, cluster, id):
         self.cluster = cluster
         self.id = id
```

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.0.0rc2/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/test_timeseries.py` & `redis-5.0.0rc2/tests/test_asyncio/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.0.0rc2/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/testdata/titles.csv` & `redis-5.0.0rc2/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.0.0rc2/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_bloom.py` & `redis-5.0.0rc2/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_cluster.py` & `redis-5.0.0rc2/tests/test_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import binascii
 import datetime
+import select
+import socket
+import socketserver
+import threading
 import warnings
 from queue import LifoQueue, Queue
 from time import sleep
 from unittest.mock import DEFAULT, Mock, call, patch
 
 import pytest
 from redis import Redis
+from redis._parsers import CommandsParser
 from redis.backoff import ExponentialBackoff, NoBackoff, default_backoff
 from redis.cluster import (
     PRIMARY,
     REDIS_CLUSTER_HASH_SLOTS,
     REPLICA,
     ClusterNode,
     NodesManager,
@@ -27,15 +32,14 @@
     MovedError,
     NoPermissionError,
     RedisClusterException,
     RedisError,
     ResponseError,
     TimeoutError,
 )
-from redis.parsers import CommandsParser
 from redis.retry import Retry
 from redis.utils import str_if_bytes
 from tests.test_pubsub import wait_for_message
 
 from .conftest import (
     _get_client,
     assert_resp_response,
@@ -49,14 +53,81 @@
 default_port = 7000
 default_cluster_slots = [
     [0, 8191, ["127.0.0.1", 7000, "node_0"], ["127.0.0.1", 7003, "node_3"]],
     [8192, 16383, ["127.0.0.1", 7001, "node_1"], ["127.0.0.1", 7002, "node_2"]],
 ]
 
 
+class ProxyRequestHandler(socketserver.BaseRequestHandler):
+    def recv(self, sock):
+        """A recv with a timeout"""
+        r = select.select([sock], [], [], 0.01)
+        if not r[0]:
+            return None
+        return sock.recv(1000)
+
+    def handle(self):
+        self.server.proxy.n_connections += 1
+        conn = socket.create_connection(self.server.proxy.redis_addr)
+        stop = False
+
+        def from_server():
+            # read from server and pass to client
+            while not stop:
+                data = self.recv(conn)
+                if data is None:
+                    continue
+                if not data:
+                    self.request.shutdown(socket.SHUT_WR)
+                    return
+                self.request.sendall(data)
+
+        thread = threading.Thread(target=from_server)
+        thread.start()
+        try:
+            while True:
+                # read from client and send to server
+                data = self.request.recv(1000)
+                if not data:
+                    return
+                conn.sendall(data)
+        finally:
+            conn.shutdown(socket.SHUT_WR)
+            stop = True  # for safety
+            thread.join()
+            conn.close()
+
+
+class NodeProxy:
+    """A class to proxy a node connection to a different port"""
+
+    def __init__(self, addr, redis_addr):
+        self.addr = addr
+        self.redis_addr = redis_addr
+        self.server = socketserver.ThreadingTCPServer(self.addr, ProxyRequestHandler)
+        self.server.proxy = self
+        self.server.socket_reuse_address = True
+        self.thread = None
+        self.n_connections = 0
+
+    def start(self):
+        # test that we can connect to redis
+        s = socket.create_connection(self.redis_addr, timeout=2)
+        s.close()
+        # Start a thread with the server -- that thread will then start one
+        # more thread for each request
+        self.thread = threading.Thread(target=self.server.serve_forever)
+        # Exit the server thread when the main thread terminates
+        self.thread.daemon = True
+        self.thread.start()
+
+    def close(self):
+        self.server.shutdown()
+
+
 @pytest.fixture()
 def slowlog(request, r):
     """
     Set the slowlog threshold to 0, and the
     max length to 128. This will force every
     command into the slowlog and allow us
     to test it
@@ -819,14 +890,59 @@
         # Mock connection error for the default node
         mock_node_resp_func(curr_default_node, raise_connection_error)
         # Test that the command succeed from a different node
         nodes = r.cluster_nodes()
         assert "myself" not in nodes.get(curr_default_node.name).get("flags")
         assert r.get_default_node() != curr_default_node
 
+    def test_address_remap(self, request, master_host):
+        """Test that we can create a rediscluster object with
+        a host-port remapper and map connections through proxy objects
+        """
+
+        # we remap the first n nodes
+        offset = 1000
+        n = 6
+        hostname, master_port = master_host
+        ports = [master_port + i for i in range(n)]
+
+        def address_remap(address):
+            # remap first three nodes to our local proxy
+            # old = host, port
+            host, port = address
+            if int(port) in ports:
+                host, port = "127.0.0.1", int(port) + offset
+            # print(f"{old} {host, port}")
+            return host, port
+
+        # create the proxies
+        proxies = [
+            NodeProxy(("127.0.0.1", port + offset), (hostname, port)) for port in ports
+        ]
+        for p in proxies:
+            p.start()
+        try:
+            # create cluster:
+            r = _get_client(
+                RedisCluster, request, flushdb=False, address_remap=address_remap
+            )
+            try:
+                assert r.ping() is True
+                assert r.set("byte_string", b"giraffe")
+                assert r.get("byte_string") == b"giraffe"
+            finally:
+                r.close()
+        finally:
+            for p in proxies:
+                p.close()
+
+        # verify that the proxies were indeed used
+        n_used = sum((1 if p.n_connections else 0) for p in proxies)
+        assert n_used > 1
+
 
 @pytest.mark.onlycluster
 class TestClusterRedisCommands:
     """
     Tests for RedisCluster unique commands
     """
 
@@ -880,15 +996,15 @@
             reset_commands_processed = node_info["total_commands_processed"]
             assert reset_commands_processed < prior_commands_processed
 
     def test_client_setname(self, r):
         node = r.get_random_node()
         r.client_setname("redis_py_test", target_nodes=node)
         client_name = r.client_getname(target_nodes=node)
-        assert client_name == "redis_py_test"
+        assert_resp_response(r, client_name, "redis_py_test", b"redis_py_test")
 
     def test_exists(self, r):
         d = {"a": b"1", "b": b"2", "c": b"3", "d": b"4"}
         r.mset_nonatomic(d)
         assert r.exists(*d.keys()) == len(d)
 
     def test_delete(self, r):
@@ -1042,14 +1158,21 @@
         ]
         for x in cluster_shards:
             assert list(x.keys()) == ["slots", "nodes"]
             for node in x["nodes"]:
                 for attribute in node.keys():
                     assert attribute in attributes
 
+    @skip_if_server_version_lt("7.2.0")
+    @skip_if_redis_enterprise()
+    def test_cluster_myshardid(self, r):
+        myshardid = r.cluster_myshardid()
+        assert isinstance(myshardid, str)
+        assert len(myshardid) > 0
+
     @skip_if_redis_enterprise()
     def test_cluster_addslots(self, r):
         node = r.get_random_node()
         mock_node_resp(node, "OK")
         assert r.cluster_addslots(node, 1, 2, 3) is True
 
     @skip_if_server_version_lt("7.0.0")
@@ -1468,15 +1591,15 @@
         assert reset_commands_processed < prior_commands_processed
 
     @skip_if_server_version_lt("6.2.0")
     def test_client_trackinginfo(self, r):
         node = r.get_primaries()[0]
         res = r.client_trackinginfo(target_nodes=node)
         assert len(res) > 2
-        assert "prefixes" in res
+        assert "prefixes" in res or b"prefixes" in res
 
     @skip_if_server_version_lt("2.9.50")
     def test_client_pause(self, r):
         node = r.get_primaries()[0]
         assert r.client_pause(1, target_nodes=node)
         assert r.client_pause(timeout=1, target_nodes=node)
         with pytest.raises(RedisError):
@@ -1630,32 +1753,76 @@
         assert r["{foo}a"] == b"1"
         assert r["{foo}b"] == b"2"
 
     # LIST COMMANDS
     def test_cluster_blpop(self, r):
         r.rpush("{foo}a", "1", "2")
         r.rpush("{foo}b", "3", "4")
-        assert r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"3")
-        assert r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"4")
-        assert r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"1")
-        assert r.blpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"2")
+        assert_resp_response(
+            r,
+            r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"3"),
+            [b"{foo}b", b"3"],
+        )
+        assert_resp_response(
+            r,
+            r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"4"),
+            [b"{foo}b", b"4"],
+        )
+        assert_resp_response(
+            r,
+            r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"1"),
+            [b"{foo}a", b"1"],
+        )
+        assert_resp_response(
+            r,
+            r.blpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"2"),
+            [b"{foo}a", b"2"],
+        )
         assert r.blpop(["{foo}b", "{foo}a"], timeout=1) is None
         r.rpush("{foo}c", "1")
-        assert r.blpop("{foo}c", timeout=1) == (b"{foo}c", b"1")
+        assert_resp_response(
+            r, r.blpop("{foo}c", timeout=1), (b"{foo}c", b"1"), [b"{foo}c", b"1"]
+        )
 
     def test_cluster_brpop(self, r):
         r.rpush("{foo}a", "1", "2")
         r.rpush("{foo}b", "3", "4")
-        assert r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"4")
-        assert r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"3")
-        assert r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"2")
-        assert r.brpop(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"1")
+        assert_resp_response(
+            r,
+            r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"4"),
+            [b"{foo}b", b"4"],
+        )
+        assert_resp_response(
+            r,
+            r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"3"),
+            [b"{foo}b", b"3"],
+        )
+        assert_resp_response(
+            r,
+            r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"2"),
+            [b"{foo}a", b"2"],
+        )
+        assert_resp_response(
+            r,
+            r.brpop(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"1"),
+            [b"{foo}a", b"1"],
+        )
         assert r.brpop(["{foo}b", "{foo}a"], timeout=1) is None
         r.rpush("{foo}c", "1")
-        assert r.brpop("{foo}c", timeout=1) == (b"{foo}c", b"1")
+        assert_resp_response(
+            r, r.brpop("{foo}c", timeout=1), (b"{foo}c", b"1"), [b"{foo}c", b"1"]
+        )
 
     def test_cluster_brpoplpush(self, r):
         r.rpush("{foo}a", "1", "2")
         r.rpush("{foo}b", "3", "4")
         assert r.brpoplpush("{foo}a", "{foo}b") == b"2"
         assert r.brpoplpush("{foo}a", "{foo}b") == b"1"
         assert r.brpoplpush("{foo}a", "{foo}b", timeout=1) is None
@@ -1829,33 +1996,83 @@
             [[b"a3", 20.0], [b"a1", 23.0]],
         )
 
     @skip_if_server_version_lt("4.9.0")
     def test_cluster_bzpopmax(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2})
         r.zadd("{foo}b", {"b1": 10, "b2": 20})
-        assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b2", 20)
-        assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b1", 10)
-        assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"a2", 2)
-        assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"a1", 1)
+        assert_resp_response(
+            r,
+            r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b2", 20),
+            [b"{foo}b", b"b2", 20],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b1", 10),
+            [b"{foo}b", b"b1", 10],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a2", 2),
+            [b"{foo}a", b"a2", 2],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmax(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a1", 1),
+            [b"{foo}a", b"a1", 1],
+        )
         assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) is None
         r.zadd("{foo}c", {"c1": 100})
-        assert r.bzpopmax("{foo}c", timeout=1) == (b"{foo}c", b"c1", 100)
+        assert_resp_response(
+            r,
+            r.bzpopmax("{foo}c", timeout=1),
+            (b"{foo}c", b"c1", 100),
+            [b"{foo}c", b"c1", 100],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     def test_cluster_bzpopmin(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2})
         r.zadd("{foo}b", {"b1": 10, "b2": 20})
-        assert r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b1", 10)
-        assert r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b2", 20)
-        assert r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"a1", 1)
-        assert r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}a", b"a2", 2)
+        assert_resp_response(
+            r,
+            r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b1", 10),
+            [b"b", b"b1", 10],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}b", b"b2", 20),
+            [b"b", b"b2", 20],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a1", 1),
+            [b"a", b"a1", 1],
+        )
+        assert_resp_response(
+            r,
+            r.bzpopmin(["{foo}b", "{foo}a"], timeout=1),
+            (b"{foo}a", b"a2", 2),
+            [b"a", b"a2", 2],
+        )
         assert r.bzpopmin(["{foo}b", "{foo}a"], timeout=1) is None
         r.zadd("{foo}c", {"c1": 100})
-        assert r.bzpopmin("{foo}c", timeout=1) == (b"{foo}c", b"c1", 100)
+        assert_resp_response(
+            r,
+            r.bzpopmin("{foo}c", timeout=1),
+            (b"{foo}c", b"c1", 100),
+            [b"{foo}c", b"c1", 100],
+        )
 
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zrangestore(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrangestore("{foo}b", "{foo}a", 0, 1)
         assert r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         assert r.zrangestore("{foo}b", "{foo}a", 1, 2)
```

### Comparing `redis-5.0.0rc1/tests/test_command_parser.py` & `redis-5.0.0rc2/tests/test_command_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import pytest
-from redis.parsers import CommandsParser
+from redis._parsers import CommandsParser
 
-from .conftest import skip_if_redis_enterprise, skip_if_server_version_lt
+from .conftest import (
+    assert_resp_response,
+    skip_if_redis_enterprise,
+    skip_if_server_version_lt,
+)
 
 
 class TestCommandsParser:
     def test_init_commands(self, r):
         commands_parser = CommandsParser(r)
         assert commands_parser.commands is not None
         assert "get" in commands_parser.commands
@@ -46,21 +50,48 @@
             b"KEYS",
             "key1",
             "key2",
             "key3",
         ]
         args7 = ["MIGRATE", "192.168.1.34", 6379, "key1", 0, 5000]
 
-        assert sorted(commands_parser.get_keys(r, *args1)) == ["key1", "key2"]
-        assert sorted(commands_parser.get_keys(r, *args2)) == ["mystream", "writers"]
-        assert sorted(commands_parser.get_keys(r, *args3)) == ["out", "zset1", "zset2"]
-        assert sorted(commands_parser.get_keys(r, *args4)) == ["Sicily", "out"]
-        assert sorted(commands_parser.get_keys(r, *args5)) == ["foo"]
-        assert sorted(commands_parser.get_keys(r, *args6)) == ["key1", "key2", "key3"]
-        assert sorted(commands_parser.get_keys(r, *args7)) == ["key1"]
+        assert_resp_response(
+            r,
+            sorted(commands_parser.get_keys(r, *args1)),
+            ["key1", "key2"],
+            [b"key1", b"key2"],
+        )
+        assert_resp_response(
+            r,
+            sorted(commands_parser.get_keys(r, *args2)),
+            ["mystream", "writers"],
+            [b"mystream", b"writers"],
+        )
+        assert_resp_response(
+            r,
+            sorted(commands_parser.get_keys(r, *args3)),
+            ["out", "zset1", "zset2"],
+            [b"out", b"zset1", b"zset2"],
+        )
+        assert_resp_response(
+            r,
+            sorted(commands_parser.get_keys(r, *args4)),
+            ["Sicily", "out"],
+            [b"Sicily", b"out"],
+        )
+        assert sorted(commands_parser.get_keys(r, *args5)) in [["foo"], [b"foo"]]
+        assert_resp_response(
+            r,
+            sorted(commands_parser.get_keys(r, *args6)),
+            ["key1", "key2", "key3"],
+            [b"key1", b"key2", b"key3"],
+        )
+        assert_resp_response(
+            r, sorted(commands_parser.get_keys(r, *args7)), ["key1"], [b"key1"]
+        )
 
     # A bug in redis<7.0 causes this to fail: https://github.com/redis/redis/issues/9493
     @skip_if_server_version_lt("7.0.0")
     def test_get_eval_keys_with_0_keys(self, r):
         commands_parser = CommandsParser(r)
         args = ["EVAL", "return {ARGV[1],ARGV[2]}", 0, "key1", "key2"]
         assert commands_parser.get_keys(r, *args) == []
```

### Comparing `redis-5.0.0rc1/tests/test_commands.py` & `redis-5.0.0rc2/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import binascii
 import datetime
 import re
+import threading
 import time
+from asyncio import CancelledError
 from string import ascii_letters
 from unittest import mock
+from unittest.mock import patch
 
 import pytest
 import redis
 from redis import exceptions
-from redis.client import EMPTY_RESPONSE, NEVER_DECODE, parse_info
+from redis._parsers.helpers import (
+    _RedisCallbacks,
+    _RedisCallbacksRESP2,
+    _RedisCallbacksRESP3,
+    parse_info,
+)
+from redis.client import EMPTY_RESPONSE, NEVER_DECODE
 
 from .conftest import (
     _get_client,
     assert_resp_response,
     assert_resp_response_in,
     is_resp2_connection,
     skip_if_redis_enterprise,
@@ -53,21 +62,21 @@
 
 # RESPONSE CALLBACKS
 @pytest.mark.onlynoncluster
 class TestResponseCallbacks:
     "Tests for the response callback system"
 
     def test_response_callbacks(self, r):
-        callbacks = redis.Redis.RESPONSE_CALLBACKS
+        callbacks = _RedisCallbacks
         if is_resp2_connection(r):
-            callbacks.update(redis.Redis.RESP2_RESPONSE_CALLBACKS)
+            callbacks.update(_RedisCallbacksRESP2)
         else:
-            callbacks.update(redis.Redis.RESP3_RESPONSE_CALLBACKS)
+            callbacks.update(_RedisCallbacksRESP3)
         assert r.response_callbacks == callbacks
-        assert id(r.response_callbacks) != id(redis.Redis.RESPONSE_CALLBACKS)
+        assert id(r.response_callbacks) != id(_RedisCallbacks)
         r.set_response_callback("GET", lambda x: "static")
         r["a"] = "foo"
         assert r["a"] == "static"
 
     def test_case_insensitive_command_names(self, r):
         assert r.response_callbacks["ping"] == r.response_callbacks["PING"]
 
@@ -129,21 +138,21 @@
             r["a"]
 
     # SERVER INFORMATION
     @skip_if_server_version_lt("6.0.0")
     def test_acl_cat_no_category(self, r):
         categories = r.acl_cat()
         assert isinstance(categories, list)
-        assert "read" in categories
+        assert "read" in categories or b"read" in categories
 
     @skip_if_server_version_lt("6.0.0")
     def test_acl_cat_with_category(self, r):
         commands = r.acl_cat("read")
         assert isinstance(commands, list)
-        assert "get" in commands
+        assert "get" in commands or b"get" in commands
 
     @skip_if_server_version_lt("7.0.0")
     @skip_if_redis_enterprise()
     def test_acl_dryrun(self, r, request):
         username = "redis-py-user"
 
         def teardown():
@@ -181,23 +190,23 @@
         assert r.acl_getuser(users[3]) is None
         assert r.acl_getuser(users[4]) is None
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     def test_acl_genpass(self, r):
         password = r.acl_genpass()
-        assert isinstance(password, str)
+        assert isinstance(password, (str, bytes))
 
         with pytest.raises(exceptions.DataError):
             r.acl_genpass("value")
             r.acl_genpass(-5)
             r.acl_genpass(5555)
 
         r.acl_genpass(555)
-        assert isinstance(password, str)
+        assert isinstance(password, (str, bytes))
 
     @skip_if_server_version_lt("7.0.0")
     @skip_if_redis_enterprise()
     def test_acl_getuser_setuser(self, r, request):
         r.flushall()
         username = "redis-py-user"
 
@@ -442,15 +451,15 @@
         users = r.acl_users()
         assert isinstance(users, list)
         assert len(users) > 0
 
     @skip_if_server_version_lt("6.0.0")
     def test_acl_whoami(self, r):
         username = r.acl_whoami()
-        assert isinstance(username, str)
+        assert isinstance(username, (str, bytes))
 
     @pytest.mark.onlynoncluster
     def test_client_list(self, r):
         clients = r.client_list()
         assert isinstance(clients[0], dict)
         assert "addr" in clients[0]
 
@@ -497,15 +506,15 @@
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.2.0")
     @skip_if_redis_enterprise()
     def test_client_trackinginfo(self, r):
         res = r.client_trackinginfo()
         assert len(res) > 2
-        assert "prefixes" in res
+        assert "prefixes" in res or b"prefixes" in res
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     def test_client_tracking(self, r, r2):
 
         # simple case
@@ -539,15 +548,15 @@
     def test_client_getname(self, r):
         assert r.client_getname() is None
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("2.6.9")
     def test_client_setname(self, r):
         assert r.client_setname("redis_py_test")
-        assert r.client_getname() == "redis_py_test"
+        assert_resp_response(r, r.client_getname(), "redis_py_test", b"redis_py_test")
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("2.6.9")
     def test_client_kill(self, r, r2):
         r.client_setname("redis-py-c1")
         r2.client_setname("redis-py-c2")
         clients = [
@@ -705,14 +714,36 @@
     @skip_if_server_version_lt("7.0.0")
     def test_client_no_evict(self, r):
         assert r.client_no_evict("ON")
         with pytest.raises(TypeError):
             r.client_no_evict()
 
     @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.2.0")
+    def test_client_no_touch(self, r):
+        assert r.client_no_touch("ON") == b"OK"
+        assert r.client_no_touch("OFF") == b"OK"
+        with pytest.raises(TypeError):
+            r.client_no_touch()
+
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.2.0")
+    def test_waitaof(self, r):
+        # must return a list of 2 elements
+        assert len(r.waitaof(0, 0, 0)) == 2
+        assert len(r.waitaof(1, 0, 0)) == 2
+        assert len(r.waitaof(1, 0, 1000)) == 2
+
+        # value is out of range, value must between 0 and 1
+        with pytest.raises(exceptions.ResponseError):
+            r.waitaof(2, 0, 0)
+        with pytest.raises(exceptions.ResponseError):
+            r.waitaof(-1, 0, 0)
+
+    @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("3.2.0")
     def test_client_reply(self, r, r_timeout):
         assert r_timeout.client_reply("ON") == b"OK"
         with pytest.raises(exceptions.RedisError):
             r_timeout.client_reply("OFF")
 
             r_timeout.client_reply("SKIP")
@@ -820,15 +851,15 @@
         lolwut = r.lolwut(5, 6, 7, 8).decode("utf-8")
         assert "Redis ver." in lolwut
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.2.0")
     @skip_if_redis_enterprise()
     def test_reset(self, r):
-        assert r.reset() == "RESET"
+        assert_resp_response(r, r.reset(), "RESET", b"RESET")
 
     def test_object(self, r):
         r["a"] = "foo"
         assert isinstance(r.object("refcount", "a"), int)
         assert isinstance(r.object("idletime", "a"), int)
         assert r.object("encoding", "a") in (b"raw", b"embstr")
         assert r.object("idletime", "invalid-key") is None
@@ -872,14 +903,16 @@
         # could be commands, before, between, or after, so just check that
         # the two we care about are in the appropriate order.
         assert commands.index(get_command) < commands.index(b"SLOWLOG RESET")
 
         # make sure other attributes are typed correctly
         assert isinstance(slowlog[0]["start_time"], int)
         assert isinstance(slowlog[0]["duration"], int)
+        assert isinstance(slowlog[0]["client_address"], bytes)
+        assert isinstance(slowlog[0]["client_name"], bytes)
 
         # Mock result if we didn't get slowlog complexity info.
         if "complexity" not in slowlog[0]:
             # monkey patch parse_response()
             COMPLEXITY_STATEMENT = "Complexity info: N:4712,M:3788"
             old_parse_response = r.parse_response
 
@@ -1785,33 +1818,49 @@
         assert r.type("a") == b"zset"
 
     # LIST COMMANDS
     @pytest.mark.onlynoncluster
     def test_blpop(self, r):
         r.rpush("a", "1", "2")
         r.rpush("b", "3", "4")
-        assert r.blpop(["b", "a"], timeout=1) == (b"b", b"3")
-        assert r.blpop(["b", "a"], timeout=1) == (b"b", b"4")
-        assert r.blpop(["b", "a"], timeout=1) == (b"a", b"1")
-        assert r.blpop(["b", "a"], timeout=1) == (b"a", b"2")
+        assert_resp_response(
+            r, r.blpop(["b", "a"], timeout=1), (b"b", b"3"), [b"b", b"3"]
+        )
+        assert_resp_response(
+            r, r.blpop(["b", "a"], timeout=1), (b"b", b"4"), [b"b", b"4"]
+        )
+        assert_resp_response(
+            r, r.blpop(["b", "a"], timeout=1), (b"a", b"1"), [b"a", b"1"]
+        )
+        assert_resp_response(
+            r, r.blpop(["b", "a"], timeout=1), (b"a", b"2"), [b"a", b"2"]
+        )
         assert r.blpop(["b", "a"], timeout=1) is None
         r.rpush("c", "1")
-        assert r.blpop("c", timeout=1) == (b"c", b"1")
+        assert_resp_response(r, r.blpop("c", timeout=1), (b"c", b"1"), [b"c", b"1"])
 
     @pytest.mark.onlynoncluster
     def test_brpop(self, r):
         r.rpush("a", "1", "2")
         r.rpush("b", "3", "4")
-        assert r.brpop(["b", "a"], timeout=1) == (b"b", b"4")
-        assert r.brpop(["b", "a"], timeout=1) == (b"b", b"3")
-        assert r.brpop(["b", "a"], timeout=1) == (b"a", b"2")
-        assert r.brpop(["b", "a"], timeout=1) == (b"a", b"1")
+        assert_resp_response(
+            r, r.brpop(["b", "a"], timeout=1), (b"b", b"4"), [b"b", b"4"]
+        )
+        assert_resp_response(
+            r, r.brpop(["b", "a"], timeout=1), (b"b", b"3"), [b"b", b"3"]
+        )
+        assert_resp_response(
+            r, r.brpop(["b", "a"], timeout=1), (b"a", b"2"), [b"a", b"2"]
+        )
+        assert_resp_response(
+            r, r.brpop(["b", "a"], timeout=1), (b"a", b"1"), [b"a", b"1"]
+        )
         assert r.brpop(["b", "a"], timeout=1) is None
         r.rpush("c", "1")
-        assert r.brpop("c", timeout=1) == (b"c", b"1")
+        assert_resp_response(r, r.brpop("c", timeout=1), (b"c", b"1"), [b"c", b"1"])
 
     @pytest.mark.onlynoncluster
     def test_brpoplpush(self, r):
         r.rpush("a", "1", "2")
         r.rpush("b", "3", "4")
         assert r.brpoplpush("a", "b") == b"2"
         assert r.brpoplpush("a", "b") == b"1"
@@ -2502,34 +2551,54 @@
         assert len(r.zrandmember("a", -10)) == 10
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("4.9.0")
     def test_bzpopmax(self, r):
         r.zadd("a", {"a1": 1, "a2": 2})
         r.zadd("b", {"b1": 10, "b2": 20})
-        assert r.bzpopmax(["b", "a"], timeout=1) == (b"b", b"b2", 20)
-        assert r.bzpopmax(["b", "a"], timeout=1) == (b"b", b"b1", 10)
-        assert r.bzpopmax(["b", "a"], timeout=1) == (b"a", b"a2", 2)
-        assert r.bzpopmax(["b", "a"], timeout=1) == (b"a", b"a1", 1)
+        assert_resp_response(
+            r, r.bzpopmax(["b", "a"], timeout=1), (b"b", b"b2", 20), [b"b", b"b2", 20]
+        )
+        assert_resp_response(
+            r, r.bzpopmax(["b", "a"], timeout=1), (b"b", b"b1", 10), [b"b", b"b1", 10]
+        )
+        assert_resp_response(
+            r, r.bzpopmax(["b", "a"], timeout=1), (b"a", b"a2", 2), [b"a", b"a2", 2]
+        )
+        assert_resp_response(
+            r, r.bzpopmax(["b", "a"], timeout=1), (b"a", b"a1", 1), [b"a", b"a1", 1]
+        )
         assert r.bzpopmax(["b", "a"], timeout=1) is None
         r.zadd("c", {"c1": 100})
-        assert r.bzpopmax("c", timeout=1) == (b"c", b"c1", 100)
+        assert_resp_response(
+            r, r.bzpopmax("c", timeout=1), (b"c", b"c1", 100), [b"c", b"c1", 100]
+        )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("4.9.0")
     def test_bzpopmin(self, r):
         r.zadd("a", {"a1": 1, "a2": 2})
         r.zadd("b", {"b1": 10, "b2": 20})
-        assert r.bzpopmin(["b", "a"], timeout=1) == (b"b", b"b1", 10)
-        assert r.bzpopmin(["b", "a"], timeout=1) == (b"b", b"b2", 20)
-        assert r.bzpopmin(["b", "a"], timeout=1) == (b"a", b"a1", 1)
-        assert r.bzpopmin(["b", "a"], timeout=1) == (b"a", b"a2", 2)
+        assert_resp_response(
+            r, r.bzpopmin(["b", "a"], timeout=1), (b"b", b"b1", 10), [b"b", b"b1", 10]
+        )
+        assert_resp_response(
+            r, r.bzpopmin(["b", "a"], timeout=1), (b"b", b"b2", 20), [b"b", b"b2", 20]
+        )
+        assert_resp_response(
+            r, r.bzpopmin(["b", "a"], timeout=1), (b"a", b"a1", 1), [b"a", b"a1", 1]
+        )
+        assert_resp_response(
+            r, r.bzpopmin(["b", "a"], timeout=1), (b"a", b"a2", 2), [b"a", b"a2", 2]
+        )
         assert r.bzpopmin(["b", "a"], timeout=1) is None
         r.zadd("c", {"c1": 100})
-        assert r.bzpopmin("c", timeout=1) == (b"c", b"c1", 100)
+        assert_resp_response(
+            r, r.bzpopmin("c", timeout=1), (b"c", b"c1", 100), [b"c", b"c1", 100]
+        )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     def test_zmpop(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert_resp_response(
             r,
@@ -2706,14 +2775,23 @@
 
     def test_zrank(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrank("a", "a1") == 0
         assert r.zrank("a", "a2") == 1
         assert r.zrank("a", "a6") is None
 
+    @skip_if_server_version_lt("7.2.0")
+    def test_zrank_withscore(self, r: redis.Redis):
+        r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
+        assert r.zrank("a", "a1") == 0
+        assert r.rank("a", "a2") == 1
+        assert r.zrank("a", "a6") is None
+        assert r.zrank("a", "a3", withscore=True) == [2, "3"]
+        assert r.zrank("a", "a6", withscore=True) is None
+
     def test_zrem(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrem("a", "a2") == 1
         assert r.zrange("a", 0, -1) == [b"a1", b"a3"]
         assert r.zrem("a", "b") == 0
         assert r.zrange("a", 0, -1) == [b"a1", b"a3"]
 
@@ -2792,14 +2870,23 @@
 
     def test_zrevrank(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrevrank("a", "a1") == 4
         assert r.zrevrank("a", "a2") == 3
         assert r.zrevrank("a", "a6") is None
 
+    @skip_if_server_version_lt("7.2.0")
+    def test_zrevrank_withscore(self, r):
+        r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
+        assert r.zrevrank("a", "a1") == 4
+        assert r.zrevrank("a", "a2") == 3
+        assert r.zrevrank("a", "a6") is None
+        assert r.zrevrank("a", "a3", withscore=True) == [2, "3"]
+        assert r.zrevrank("a", "a6", withscore=True) is None
+
     def test_zscore(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zscore("a", "a1") == 1.0
         assert r.zscore("a", "a2") == 2.0
         assert r.zscore("a", "a4") is None
 
     @pytest.mark.onlynoncluster
@@ -3399,34 +3486,43 @@
     def test_geohash(self, r):
         values = (2.1909389952632, 41.433791470673, "place1") + (
             2.1873744593677,
             41.406342043777,
             "place2",
         )
         r.geoadd("barcelona", values)
-        assert r.geohash("barcelona", "place1", "place2", "place3") == [
-            "sp3e9yg3kd0",
-            "sp3e9cbc3t0",
-            None,
-        ]
+        assert_resp_response(
+            r,
+            r.geohash("barcelona", "place1", "place2", "place3"),
+            ["sp3e9yg3kd0", "sp3e9cbc3t0", None],
+            [b"sp3e9yg3kd0", b"sp3e9cbc3t0", None],
+        )
 
     @skip_unless_arch_bits(64)
     @skip_if_server_version_lt("3.2.0")
     def test_geopos(self, r):
         values = (2.1909389952632, 41.433791470673, "place1") + (
             2.1873744593677,
             41.406342043777,
             "place2",
         )
         r.geoadd("barcelona", values)
         # redis uses 52 bits precision, hereby small errors may be introduced.
-        assert r.geopos("barcelona", "place1", "place2") == [
-            (2.19093829393386841, 41.43379028184083523),
-            (2.18737632036209106, 41.40634178640635099),
-        ]
+        assert_resp_response(
+            r,
+            r.geopos("barcelona", "place1", "place2"),
+            [
+                (2.19093829393386841, 41.43379028184083523),
+                (2.18737632036209106, 41.40634178640635099),
+            ],
+            [
+                [2.19093829393386841, 41.43379028184083523],
+                [2.18737632036209106, 41.40634178640635099],
+            ],
+        )
 
     @skip_if_server_version_lt("4.0.0")
     def test_geopos_no_value(self, r):
         assert r.geopos("barcelona", "place1", "place2") == [None, None]
 
     @skip_if_server_version_lt("3.2.0")
     @skip_if_server_version_gte("4.0.0")
@@ -3660,14 +3756,20 @@
             radius=1000,
             storedist=True,
         )
         # instead of save the geo score, the distance is saved.
         assert r.zscore("places_barcelona", "place1") == 88.05060698409301
 
     @skip_if_server_version_lt("3.2.0")
+    def test_georadius_Issue2609(self, r):
+        # test for issue #2609 (Geo search functions don't work with execute_command)
+        r.geoadd(name="my-key", values=[1, 2, "data"])
+        assert r.execute_command("GEORADIUS", "my-key", 1, 2, 400, "m") == [b"data"]
+
+    @skip_if_server_version_lt("3.2.0")
     def test_georadius(self, r):
         values = (2.1909389952632, 41.433791470673, "place1") + (
             2.1873744593677,
             41.406342043777,
             b"\x80place2",
         )
 
@@ -4777,28 +4879,30 @@
             r.command_list(category="list", pattern="l*")
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("2.8.13")
     @skip_if_redis_enterprise()
     def test_command_getkeys(self, r):
         res = r.command_getkeys("MSET", "a", "b", "c", "d", "e", "f")
-        assert res == ["a", "c", "e"]
+        assert_resp_response(r, res, ["a", "c", "e"], [b"a", b"c", b"e"])
         res = r.command_getkeys(
             "EVAL",
             '"not consulted"',
             "3",
             "key1",
             "key2",
             "key3",
             "arg1",
             "arg2",
             "arg3",
             "argN",
         )
-        assert res == ["key1", "key2", "key3"]
+        assert_resp_response(
+            r, res, ["key1", "key2", "key3"], [b"key1", b"key2", b"key3"]
+        )
 
     @skip_if_server_version_lt("2.8.13")
     def test_command(self, r):
         res = r.command()
         assert len(res) >= 100
         cmds = list(res.keys())
         assert "set" in cmds
@@ -4924,14 +5028,46 @@
     @skip_if_server_version_lt("2.8.0")
     @skip_if_redis_enterprise()
     def test_psync(self, r):
         r2 = redis.Redis(port=6380, decode_responses=False)
         res = r2.psync(r2.client_id(), 1)
         assert b"FULLRESYNC" in res
 
+    @pytest.mark.onlynoncluster
+    def test_interrupted_command(self, r: redis.Redis):
+        """
+        Regression test for issue #1128:  An Un-handled BaseException
+        will leave the socket with un-read response to a previous
+        command.
+        """
+
+        ok = False
+
+        def helper():
+            with pytest.raises(CancelledError):
+                # blocking pop
+                with patch.object(
+                    r.connection._parser, "read_response", side_effect=CancelledError
+                ):
+                    r.brpop(["nonexist"])
+            # if all is well, we can continue.
+            r.set("status", "down")  # should not hang
+            nonlocal ok
+            ok = True
+
+        thread = threading.Thread(target=helper)
+        thread.start()
+        thread.join(0.1)
+        try:
+            assert not thread.is_alive()
+            assert ok
+        finally:
+            # disconnect here so that fixture cleanup can proceed
+            r.connection.disconnect()
+
 
 @pytest.mark.onlynoncluster
 class TestBinarySave:
     def test_binary_get_set(self, r):
         assert r.set(" foo bar ", "123")
         assert r.get(" foo bar ") == b"123"
```

### Comparing `redis-5.0.0rc1/tests/test_connection.py` & `redis-5.0.0rc2/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import socket
 import types
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
 import redis
+from redis._parsers import _HiredisParser, _RESP2Parser, _RESP3Parser
 from redis.backoff import NoBackoff
 from redis.connection import Connection, SSLConnection, UnixDomainSocketConnection
 from redis.exceptions import ConnectionError, InvalidResponse, TimeoutError
-from redis.parsers import _HiredisParser, _RESP2Parser, _RESP3Parser
 from redis.retry import Retry
 from redis.utils import HIREDIS_AVAILABLE
 
 from .conftest import skip_if_server_version_lt
 from .mocks import MockSocket
 
 
@@ -152,15 +152,15 @@
 
     if isinstance(conn._parser, _RESP2Parser) or isinstance(conn._parser, _RESP3Parser):
         conn._parser._buffer._sock = mock_socket
     else:
         conn._parser._sock = mock_socket
     for i in range(100):
         try:
-            response = conn.read_response()
+            response = conn.read_response(disconnect_on_error=False)
             break
         except MockSocket.TestError:
             pass
 
     else:
         pytest.fail("didn't receive a response")
     assert response
@@ -197,7 +197,15 @@
         b"*10\r\n$4\r\nHSET\r\n$3\r\nfoo\r\n$3\r\nkey\r\n$6\r\nvalue1\r\n"
         b"$5\r\nkey_b\r\n$9\r\nbytes str\r\n$5\r\nkey_i\r\n$2\r\n67\r\n$5"
         b"\r\nkey_f\r\n$13\r\n3.14159265359\r\n"
     )
 
     actual = Class().pack_command(*cmd)[0]
     assert actual == expected, f"actual = {actual}, expected = {expected}"
+
+
+@pytest.mark.onlynoncluster
+def test_create_single_connection_client_from_url():
+    client = redis.Redis.from_url(
+        "redis://localhost:6379/0?", single_connection_client=True
+    )
+    assert client.connection is not None
```

### Comparing `redis-5.0.0rc1/tests/test_connection_pool.py` & `redis-5.0.0rc2/tests/test_connection_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,18 +524,25 @@
         assert not pipe.connection
         assert len(pool._available_connections) == 1
         assert not pool._available_connections[0]._sock
 
     @skip_if_server_version_lt("2.8.8")
     @skip_if_redis_enterprise()
     def test_read_only_error(self, r):
-        "READONLY errors get turned in ReadOnlyError exceptions"
+        "READONLY errors get turned into ReadOnlyError exceptions"
         with pytest.raises(redis.ReadOnlyError):
             r.execute_command("DEBUG", "ERROR", "READONLY blah blah")
 
+    def test_oom_error(self, r):
+        "OOM errors get turned into OutOfMemoryError exceptions"
+        with pytest.raises(redis.OutOfMemoryError):
+            # note: don't use the DEBUG OOM command since it's not the same
+            # as the db being full
+            r.execute_command("DEBUG", "ERROR", "OOM blah blah")
+
     def test_connect_from_url_tcp(self):
         connection = redis.Redis.from_url("redis://localhost")
         pool = connection.connection_pool
 
         assert re.match("(.*)<(.*)<(.*)>>", repr(pool)).groups() == (
             "ConnectionPool",
             "Connection",
```

### Comparing `redis-5.0.0rc1/tests/test_credentials.py` & `redis-5.0.0rc2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_encoding.py` & `redis-5.0.0rc2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_function.py` & `redis-5.0.0rc2/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_graph.py` & `redis-5.0.0rc2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_graph_utils/test_edge.py` & `redis-5.0.0rc2/tests/test_graph_utils/test_edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_graph_utils/test_node.py` & `redis-5.0.0rc2/tests/test_graph_utils/test_node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_graph_utils/test_path.py` & `redis-5.0.0rc2/tests/test_graph_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_helpers.py` & `redis-5.0.0rc2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_json.py` & `redis-5.0.0rc2/tests/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,47 @@
     assert_resp_response(client, client.json().get("foo"), "bar", [["bar"]])
     assert client.json().get("baz") is None
     assert 1 == client.json().delete("foo")
     assert client.exists("foo") == 0
 
 
 @pytest.mark.redismod
+@skip_ifmodversion_lt("2.6.0", "ReJSON")  # todo: update after the release
+def test_json_merge(client):
+    # Test with root path $
+    assert client.json().set(
+        "person_data",
+        "$",
+        {"person1": {"personal_data": {"name": "John"}}},
+    )
+    assert client.json().merge(
+        "person_data", "$", {"person1": {"personal_data": {"hobbies": "reading"}}}
+    )
+    assert client.json().get("person_data") == {
+        "person1": {"personal_data": {"name": "John", "hobbies": "reading"}}
+    }
+
+    # Test with root path path $.person1.personal_data
+    assert client.json().merge(
+        "person_data", "$.person1.personal_data", {"country": "Israel"}
+    )
+    assert client.json().get("person_data") == {
+        "person1": {
+            "personal_data": {"name": "John", "hobbies": "reading", "country": "Israel"}
+        }
+    }
+
+    # Test with null value to delete a value
+    assert client.json().merge("person_data", "$.person1.personal_data", {"name": None})
+    assert client.json().get("person_data") == {
+        "person1": {"personal_data": {"country": "Israel", "hobbies": "reading"}}
+    }
+
+
+@pytest.mark.redismod
 def test_nonascii_setgetdelete(client):
     assert client.json().set("notascii", Path.root_path(), "hyvää-élève")
     res = "hyvää-élève"
     assert_resp_response(
         client, client.json().get("notascii", no_escape=True), res, [[res]]
     )
     assert 1 == client.json().delete("notascii")
@@ -82,14 +115,23 @@
     client.json().set("2", Path.root_path(), 2)
     assert client.json().mget(["1"], Path.root_path()) == [1]
 
     assert client.json().mget([1, 2], Path.root_path()) == [1, 2]
 
 
 @pytest.mark.redismod
+@skip_ifmodversion_lt("2.6.0", "ReJSON")  # todo: update after the release
+def test_mset(client):
+    client.json().mset([("1", Path.root_path(), 1), ("2", Path.root_path(), 2)])
+
+    assert client.json().mget(["1"], Path.root_path()) == [1]
+    assert client.json().mget(["1", "2"], Path.root_path()) == [1, 2]
+
+
+@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 def test_clear(client):
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 1 == client.json().clear("arr", Path.root_path())
     assert_resp_response(client, client.json().get("arr"), [], [[[]]])
```

### Comparing `redis-5.0.0rc1/tests/test_lock.py` & `redis-5.0.0rc2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_monitor.py` & `redis-5.0.0rc2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_multiprocessing.py` & `redis-5.0.0rc2/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_pipeline.py` & `redis-5.0.0rc2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_pubsub.py` & `redis-5.0.0rc2/tests/test_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1139,17 +1139,17 @@
                     return message
 
         # get subscribe message
         msg = get_msg()
         assert msg is not None
         # timeout waiting for another message which never arrives
         assert is_connected()
-        with patch("redis.parsers._RESP2Parser.read_response") as mock1, patch(
-            "redis.parsers._HiredisParser.read_response"
-        ) as mock2, patch("redis.parsers._RESP3Parser.read_response") as mock3:
+        with patch("redis._parsers._RESP2Parser.read_response") as mock1, patch(
+            "redis._parsers._HiredisParser.read_response"
+        ) as mock2, patch("redis._parsers._RESP3Parser.read_response") as mock3:
             mock1.side_effect = BaseException("boom")
             mock2.side_effect = BaseException("boom")
             mock3.side_effect = BaseException("boom")
 
             with pytest.raises(BaseException):
                 get_msg()
```

### Comparing `redis-5.0.0rc1/tests/test_retry.py` & `redis-5.0.0rc2/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_scripting.py` & `redis-5.0.0rc2/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_search.py` & `redis-5.0.0rc2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/test_sentinel.py` & `redis-5.0.0rc2/tests/test_sentinel.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,23 @@
 @pytest.mark.onlynoncluster
 def test_discover_master_error(sentinel):
     with pytest.raises(MasterNotFoundError):
         sentinel.discover_master("xxx")
 
 
 @pytest.mark.onlynoncluster
+def test_dead_pool(sentinel):
+    master = sentinel.master_for("mymaster", db=9)
+    conn = master.connection_pool.get_connection("_")
+    conn.disconnect()
+    del master
+    conn.connect()
+
+
+@pytest.mark.onlynoncluster
 def test_discover_master_sentinel_down(cluster, sentinel, master_ip):
     # Put first sentinel 'foo' down
     cluster.nodes_down.add(("foo", 26379))
     address = sentinel.discover_master("mymaster")
     assert address == (master_ip, 6379)
     # 'bar' is now first sentinel
     assert sentinel.sentinels[0].id == ("bar", 26379)
```

### Comparing `redis-5.0.0rc1/tests/test_ssl.py` & `redis-5.0.0rc2/tests/test_ssl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-import os
 import socket
 import ssl
 from urllib.parse import urlparse
 
 import pytest
 import redis
 from redis.exceptions import ConnectionError, RedisError
 
 from .conftest import skip_if_cryptography, skip_if_nocryptography
+from .ssl_utils import get_ssl_filename
 
 
 @pytest.mark.ssl
 class TestSSL:
     """Tests for SSL connections
 
     This relies on the --redis-ssl-url purely for rebuilding the client
     and connecting to the appropriate port.
     """
 
-    ROOT = os.path.join(os.path.dirname(__file__), "..")
-    CERT_DIR = os.path.abspath(os.path.join(ROOT, "dockers", "stunnel", "keys"))
-    if not os.path.isdir(CERT_DIR):  # github actions package validation case
-        CERT_DIR = os.path.abspath(
-            os.path.join(ROOT, "..", "dockers", "stunnel", "keys")
-        )
-        if not os.path.isdir(CERT_DIR):
-            raise IOError(f"No SSL certificates found. They should be in {CERT_DIR}")
-
-    SERVER_CERT = os.path.join(CERT_DIR, "server-cert.pem")
-    SERVER_KEY = os.path.join(CERT_DIR, "server-key.pem")
+    SERVER_CERT = get_ssl_filename("server-cert.pem")
+    SERVER_KEY = get_ssl_filename("server-key.pem")
 
     def test_ssl_with_invalid_cert(self, request):
         ssl_url = request.config.option.redis_ssl_url
         sslclient = redis.from_url(ssl_url)
         with pytest.raises(ConnectionError) as e:
             sslclient.ping()
             assert "SSL: CERTIFICATE_VERIFY_FAILED" in str(e)
```

### Comparing `redis-5.0.0rc1/tests/test_timeseries.py` & `redis-5.0.0rc2/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/testdata/jsontestdata.py` & `redis-5.0.0rc2/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/testdata/titles.csv` & `redis-5.0.0rc2/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0rc1/tests/testdata/will_play_text.csv.bz2` & `redis-5.0.0rc2/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

