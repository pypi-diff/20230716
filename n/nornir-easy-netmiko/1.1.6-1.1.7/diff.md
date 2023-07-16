# Comparing `tmp/nornir_easy_netmiko-1.1.6.tar.gz` & `tmp/nornir_easy_netmiko-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_easy_netmiko-1.1.6.tar", max compression
+gzip compressed data, was "nornir_easy_netmiko-1.1.7.tar", max compression
```

## Comparing `nornir_easy_netmiko-1.1.6.tar` & `nornir_easy_netmiko-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,88 @@
--rw-r--r--   0        0        0      667 2023-07-11 13:12:50.179098 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/__init__.py
--rw-r--r--   0        0        0      170 2023-07-11 13:12:50.237110 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__init__.py
--rw-r--r--   0        0        0      315 2023-07-11 13:12:50.269117 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-07-11 13:13:51.455855 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-07-11 13:12:50.302125 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
--rw-r--r--   0        0        0     2425 2023-07-11 13:13:51.459856 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
--rw-r--r--   0        0        0     1666 2023-07-11 13:13:38.039628 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/netmiko.py
--rw-r--r--   0        0        0      958 2023-07-11 13:12:50.335132 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 13:12:50.352136 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2023-07-11 13:13:51.657900 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      634 2023-07-11 13:12:50.370140 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__init__.py
--rw-r--r--   0        0        0      746 2023-07-11 13:12:50.482165 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      846 2023-07-11 13:13:51.613890 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      953 2023-07-11 13:12:50.518173 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
--rw-r--r--   0        0        0     1326 2023-07-11 13:13:51.618891 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
--rw-r--r--   0        0        0     1372 2023-07-11 13:12:50.553180 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     1850 2023-07-11 13:13:51.623892 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
--rw-r--r--   0        0        0     1405 2023-07-11 13:12:50.584188 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-07-11 13:13:51.667902 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
--rw-r--r--   0        0        0     1240 2023-07-11 13:12:50.620195 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2023-07-11 13:13:51.627893 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-07-11 13:12:50.656204 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
--rw-r--r--   0        0        0     2206 2023-07-11 13:13:51.632894 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-07-11 13:12:50.693213 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
--rw-r--r--   0        0        0     3912 2023-07-11 13:13:51.662901 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
--rw-r--r--   0        0        0      683 2023-07-11 13:12:50.385143 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_commit.py
--rw-r--r--   0        0        0     1189 2023-07-11 13:12:50.400146 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
--rw-r--r--   0        0        0     1179 2023-07-11 13:12:50.416150 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_multiline.py
--rw-r--r--   0        0        0     1061 2023-07-11 13:12:50.431153 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_save_config.py
--rw-r--r--   0        0        0     1445 2023-07-11 13:12:50.446157 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_command.py
--rw-r--r--   0        0        0     2442 2023-07-11 13:12:50.461160 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_config.py
--rw-r--r--   0        0        0     1024 2023-07-11 13:13:47.427008 nornir_easy_netmiko-1.1.6/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.6/README.md
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      308 2023-07-16 03:04:23.135830 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/config
+-rw-r--r--   0        0        0       73 2023-07-16 03:04:19.670868 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/description
+-rw-r--r--   0        0        0       21 2023-07-16 03:04:23.127828 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/HEAD
+-rw-r--r--   0        0        0      478 2023-07-16 03:04:19.674869 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/applypatch-msg.sample
+-rw-r--r--   0        0        0      896 2023-07-16 03:04:19.677869 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/commit-msg.sample
+-rw-r--r--   0        0        0     4726 2023-07-16 03:04:19.681870 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/fsmonitor-watchman.sample
+-rw-r--r--   0        0        0      189 2023-07-16 03:04:19.684872 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/post-update.sample
+-rw-r--r--   0        0        0      424 2023-07-16 03:04:19.687872 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-applypatch.sample
+-rw-r--r--   0        0        0     1643 2023-07-16 03:04:19.691784 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-commit.sample
+-rw-r--r--   0        0        0      416 2023-07-16 03:04:19.693784 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-merge-commit.sample
+-rw-r--r--   0        0        0     1374 2023-07-16 03:04:19.697785 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-push.sample
+-rw-r--r--   0        0        0     4898 2023-07-16 03:04:19.703349 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-rebase.sample
+-rw-r--r--   0        0        0      544 2023-07-16 03:04:19.706350 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/pre-receive.sample
+-rw-r--r--   0        0        0     1492 2023-07-16 03:04:19.709351 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/prepare-commit-msg.sample
+-rw-r--r--   0        0        0     2783 2023-07-16 03:04:19.712351 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/push-to-checkout.sample
+-rw-r--r--   0        0        0     3650 2023-07-16 03:04:19.715352 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/hooks/update.sample
+-rw-r--r--   0        0        0     7775 2023-07-16 03:04:23.156835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/index
+-rw-r--r--   0        0        0      240 2023-07-16 03:04:19.718683 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/info/exclude
+-rw-r--r--   0        0        0      187 2023-07-16 03:04:23.131829 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/logs/HEAD
+-rw-r--r--   0        0        0      187 2023-07-16 03:04:23.131829 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      187 2023-07-16 03:04:23.127828 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0     4628 2023-07-16 03:04:23.101610 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/objects/pack/pack-be3d3a825c297fe6a3cc1d036097fe20be9cf0f7.idx
+-rw-r--r--   0        0        0    48085 2023-07-16 03:04:23.100832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/objects/pack/pack-be3d3a825c297fe6a3cc1d036097fe20be9cf0f7.pack
+-rw-r--r--   0        0        0      112 2023-07-16 03:04:23.122827 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/packed-refs
+-rw-r--r--   0        0        0       41 2023-07-16 03:04:23.131829 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/refs/heads/main
+-rw-r--r--   0        0        0       30 2023-07-16 03:04:23.127828 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0      946 2023-07-16 03:04:23.145832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/config/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0       90 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/config/groups.yaml
+-rw-r--r--   0        0        0      570 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/config/hosts.yaml
+-rw-r--r--   0        0        0      654 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/config/settings.py
+-rw-r--r--   0        0        0      313 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/main.py
+-rw-r--r--   0        0        0      909 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/manage.py
+-rw-r--r--   0        0        0    17059 2023-07-16 03:04:23.146832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir.log
+-rw-r--r--   0        0        0      686 2023-07-16 03:04:23.147832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/__init__.py
+-rw-r--r--   0        0        0      600 2023-07-16 03:04:23.147832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      722 2023-07-16 03:04:23.147832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      174 2023-07-16 03:04:23.147832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-16 03:04:23.147832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      341 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
+-rw-r--r--   0        0        0     2406 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
+-rw-r--r--   0        0        0     1729 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/netmiko.py
+-rw-r--r--   0        0        0     1153 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/errors/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-16 03:04:23.148832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      650 2023-07-16 03:04:23.149833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-16 03:04:23.149833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      836 2023-07-16 03:04:23.149833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      953 2023-07-16 03:04:23.149833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
+-rw-r--r--   0        0        0     1316 2023-07-16 03:04:23.149833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
+-rw-r--r--   0        0        0     1372 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     1840 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
+-rw-r--r--   0        0        0     1405 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
+-rw-r--r--   0        0        0     1852 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
+-rw-r--r--   0        0        0     1596 2023-07-16 03:04:23.150833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-07-16 03:04:23.151834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
+-rw-r--r--   0        0        0     1759 2023-07-16 03:04:23.151834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-07-16 03:04:23.151834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
+-rw-r--r--   0        0        0     2291 2023-07-16 03:04:23.151834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
+-rw-r--r--   0        0        0      704 2023-07-16 03:04:23.151834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_commit.py
+-rw-r--r--   0        0        0     1224 2023-07-16 03:04:23.152833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
+-rw-r--r--   0        0        0     1212 2023-07-16 03:04:23.152833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_multiline.py
+-rw-r--r--   0        0        0     1088 2023-07-16 03:04:23.152833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_save_config.py
+-rw-r--r--   0        0        0     1483 2023-07-16 03:04:23.152833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_send_command.py
+-rw-r--r--   0        0        0     2552 2023-07-16 03:04:23.152833 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_send_config.py
+-rw-r--r--   0        0        0     2303 2023-07-16 03:04:23.153834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/processor/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-16 03:04:23.153834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/processor/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2296 2023-07-16 03:04:23.153834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/processor.py
+-rw-r--r--   0        0        0       21 2023-07-16 03:04:23.144832 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 03:04:23.153834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/register.py
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.153834 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-12-06/test_host2(192.168.56.56).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-12-06/test_host3(192.168.56.57).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-12-06/test_host4(192.168.56.58).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-17-23/test_host2(192.168.56.56).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-17-23/test_host3(192.168.56.57).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-17-23/test_host4(192.168.56.58).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.154835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-19-57/test_host2(192.168.56.56).txt
+-rw-r--r--   0        0        0     6629 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-19-57/test_host3(192.168.56.57).txt
+-rw-r--r--   0        0        0     6616 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/2023-07-10_19-19-57/test_host4(192.168.56.58).txt
+-rw-r--r--   0        0        0      396 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/save/result.scv
+-rw-r--r--   0        0        0      647 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/settings.py
+-rw-r--r--   0        0        0      339 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/tasks/backup.py
+-rw-r--r--   0        0        0      347 2023-07-16 03:04:23.155835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/tasks/h3c_display_device.py
+-rw-r--r--   0        0        0      249 2023-07-16 03:04:23.156835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/tasks/save_config.py
+-rw-r--r--   0        0        0        0 2023-07-16 03:04:23.156835 nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/utils.py
+-rw-r--r--   0        0        0     1024 2023-07-16 03:09:13.408873 nornir_easy_netmiko-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.7/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.7/PKG-INFO
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8255ad64 (Tue Jul 11 13:13:38 2023 UTC)
-files sz: 1666
+moddate:  0x39098b64 (Thu Jun 15 12:51:05 2023 UTC)
+files sz: 1661
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -34,15 +34,15 @@
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('Config',))
                 38 IMPORT_NAME              6 (nornir.core.configuration)
                 40 IMPORT_FROM              7 (Config)
                 42 STORE_NAME               7 (Config)
                 44 POP_TOP
    
-     8          46 LOAD_CONST               4 ('easy_netmiko')
+     8          46 LOAD_CONST               4 ('netmiko')
                 48 STORE_NAME               8 (CONNECTION_NAME)
    
     11          50 LOAD_CONST               5 ('cisco_ios')
    
     12          52 LOAD_CONST               6 ('cisco_nxos')
    
     13          54 LOAD_CONST               6 ('cisco_nxos')
@@ -55,28 +55,28 @@
    
     10          62 LOAD_CONST              10 (('ios', 'nxos', 'nxos_ssh', 'eos', 'junos', 'iosxr'))
                 64 BUILD_CONST_KEY_MAP      6
                 66 STORE_NAME               9 (napalm_to_netmiko_map)
    
     20          68 PUSH_NULL
                 70 LOAD_BUILD_CLASS
-                72 LOAD_CONST              11 (<code object Netmiko, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 20>)
+                72 LOAD_CONST              11 (<code object Netmiko, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 20>)
                 74 MAKE_FUNCTION            0
                 76 LOAD_CONST              12 ('Netmiko')
                 78 PRECALL                  2
                 82 CALL                     2
                 92 STORE_NAME              10 (Netmiko)
                 94 LOAD_CONST              13 (None)
                 96 RETURN_VALUE
    consts
       0
       ('Any', 'Dict', 'Optional')
       ('ConnectHandler',)
       ('Config',)
-      'easy_netmiko'
+      'netmiko'
       'cisco_ios'
       'cisco_nxos'
       'arista_eos'
       'juniper_junos'
       'cisco_xr'
       ('ios', 'nxos', 'nxos_ssh', 'eos', 'junos', 'iosxr')
       code
@@ -152,20 +152,20 @@
                      138 BINARY_SUBSCR
          
           28         148 LOAD_CONST              10 ('return')
          
           37         150 LOAD_CONST               2 (None)
          
           28         152 BUILD_TUPLE             16
-                     154 LOAD_CONST              11 (<code object open, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 28>)
+                     154 LOAD_CONST              11 (<code object open, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 28>)
                      156 MAKE_FUNCTION            5 (defaults, annotations)
                      158 STORE_NAME              10 (open)
          
           62         160 LOAD_CONST              14 (('return', None))
-                     162 LOAD_CONST              12 (<code object close, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 62>)
+                     162 LOAD_CONST              12 (<code object close, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 62>)
                      164 MAKE_FUNCTION            4 (annotations)
                      166 STORE_NAME              11 (close)
                      168 LOAD_CONST               2 (None)
                      170 RETURN_VALUE
          consts
             'Netmiko'
             '\n    This plugin connects to the device using the Netmiko driver and sets the\n    relevant connection.\n    Inventory:\n        extras: maps to argument passed to ``ConnectHandler``.\n    '
@@ -285,15 +285,15 @@
                   'ssh_config_file'
                   'device_type'
                   ()
                names      ('ssh', 'config_file', 'AttributeError', 'napalm_to_netmiko_map', 'get', 'update', 'ConnectHandler', 'connection')
                varnames   ('self', 'hostname', 'username', 'password', 'port', 'platform', 'extras', 'configuration', 'parameters', 'connection')
                freevars   ()
                cellvars   ()
-               filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
+               filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
                name       'open'
                firstlineno 28
                lnotab
                   0x020b02010201020102fc0607020316fe020102ff0803120104ff080304
                   0236010a0208012a011801
             code
                argcount  : 1
@@ -315,33 +315,33 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('connection', 'disconnect')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
+               filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
                name       'close'
                firstlineno 62
                lnotab 0x0201
             (None, None)
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Optional', 'str', 'int', 'Dict', 'Any', 'Config', 'open', 'close')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
+         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
          name       'Netmiko'
          firstlineno 20
          lnotab
             0x0a01040e020102f804020efe02030efd02040efc02050efb02060efa02
             071ef902080ef8020902f70822
       'Netmiko'
       None
    names      ('typing', 'Any', 'Dict', 'Optional', 'netmiko', 'ConnectHandler', 'nornir.core.configuration', 'Config', 'CONNECTION_NAME', 'napalm_to_netmiko_map', 'Netmiko')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020114020c020c0304030201020102010201020102fa060a
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/netmiko.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/connections/netmiko.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Any, Dict, Optional
-
-from netmiko import ConnectHandler
-
-from nornir.core.configuration import Config
-
-
-CONNECTION_NAME = "easy_netmiko"
-
-napalm_to_netmiko_map = {
-    "ios": "cisco_ios",
-    "nxos": "cisco_nxos",
-    "nxos_ssh": "cisco_nxos",
-    "eos": "arista_eos",
-    "junos": "juniper_junos",
-    "iosxr": "cisco_xr",
-}
-
-
-class Netmiko:
-    """
-    This plugin connects to the device using the Netmiko driver and sets the
-    relevant connection.
-    Inventory:
-        extras: maps to argument passed to ``ConnectHandler``.
-    """
-
-    def open(
-        self,
-        hostname: Optional[str],
-        username: Optional[str],
-        password: Optional[str],
-        port: Optional[int],
-        platform: Optional[str],
-        extras: Optional[Dict[str, Any]] = None,
-        configuration: Optional[Config] = None,
-    ) -> None:
-        parameters = {
-            "host": hostname,
-            "username": username,
-            "password": password,
-            "port": port,
-        }
-
-        try:
-            parameters[
-                "ssh_config_file"
-            ] = configuration.ssh.config_file  # type: ignore
-        except AttributeError:
-            pass
-
-        if platform is not None:
-            # Look platform up in corresponding map, if no entry return the host.nos unmodified
-            platform = napalm_to_netmiko_map.get(platform, platform)
-            parameters["device_type"] = platform
-
-        extras = extras or {}
-        parameters.update(extras)
-        connection = ConnectHandler(**parameters)
-        self.connection = connection
-
-    def close(self) -> None:
-        self.connection.disconnect()
+from typing import Any, Dict, Optional
+
+from netmiko import ConnectHandler
+
+from nornir.core.configuration import Config
+
+
+CONNECTION_NAME = "easy_netmiko"
+
+napalm_to_netmiko_map = {
+    "ios": "cisco_ios",
+    "nxos": "cisco_nxos",
+    "nxos_ssh": "cisco_nxos",
+    "eos": "arista_eos",
+    "junos": "juniper_junos",
+    "iosxr": "cisco_xr",
+}
+
+
+class Netmiko:
+    """
+    This plugin connects to the device using the Netmiko driver and sets the
+    relevant connection.
+    Inventory:
+        extras: maps to argument passed to ``ConnectHandler``.
+    """
+
+    def open(
+        self,
+        hostname: Optional[str],
+        username: Optional[str],
+        password: Optional[str],
+        port: Optional[int],
+        platform: Optional[str],
+        extras: Optional[Dict[str, Any]] = None,
+        configuration: Optional[Config] = None,
+    ) -> None:
+        parameters = {
+            "host": hostname,
+            "username": username,
+            "password": password,
+            "port": port,
+        }
+
+        try:
+            parameters[
+                "ssh_config_file"
+            ] = configuration.ssh.config_file  # type: ignore
+        except AttributeError:
+            pass
+
+        if platform is not None:
+            # Look platform up in corresponding map, if no entry return the host.nos unmodified
+            platform = napalm_to_netmiko_map.get(platform, platform)
+            parameters["device_type"] = platform
+
+        extras = extras or {}
+        parameters.update(extras)
+        connection = ConnectHandler(**parameters)
+        self.connection = connection
+
+    def close(self) -> None:
+        self.connection.disconnect()
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__init__.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/errors/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from netmiko.exceptions import NetMikoAuthenticationException
+from netmiko.exceptions import NetMikoAuthenticationException, NetmikoTimeoutException
 from jinja2.exceptions import UndefinedError
 from nornir.core.task import Result
 from functools import wraps
 
 logger = logging.getLogger("nornir")
 
 def error_handle(func):
@@ -15,13 +15,16 @@
         try:
             result = func(*args, **kwargs)
             logger.info(f"{base_string} excute <{task}> success.")
             return result
         except NetMikoAuthenticationException as e:
             logger.warning(f"{base_string} user/password invaild.")
             return Result(host, exception=e, failed=True)
+        except NetmikoTimeoutException as e:
+            logger.warning(f"{base_string} connect timeout.")
+            return Result(host, exception=e, failed=True)
         except UndefinedError as e:
             logger.warning(f"{base_string} {e}")
             return Result(host, exception=e, failed=True)
     return wrapper
             
-                
+
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
+moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
 files sz: 634
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -68,11 +68,11 @@
       ('netmiko_multiline',)
       ('netmiko_commit', 'netmiko_file_transfer', 'netmiko_save_config', 'netmiko_send_command', 'netmiko_send_config', 'netmiko_multiline')
       None
    names      ('nornir_easy_netmiko.tasks.netmiko_commit', 'netmiko_commit', 'nornir_easy_netmiko.tasks.netmiko_file_transfer', 'netmiko_file_transfer', 'nornir_easy_netmiko.tasks.netmiko_save_config', 'netmiko_save_config', 'nornir_easy_netmiko.tasks.netmiko_send_command', 'netmiko_send_command', 'nornir_easy_netmiko.tasks.netmiko_send_config', 'netmiko_send_config', 'nornir_easy_netmiko.tasks.netmiko_multiline', 'netmiko_multiline', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\__init__.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c010c010c010c010c03
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
-files sz: 683
+moddate:  0x1e0d8b64 (Thu Jun 15 13:07:42 2023 UTC)
+files sz: 684
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -38,15 +38,15 @@
      6          42 LOAD_CONST               4 ('task')
                 44 LOAD_NAME                4 (Task)
                 46 LOAD_CONST               5 ('kwargs')
                 48 LOAD_NAME                1 (Any)
                 50 LOAD_CONST               6 ('return')
                 52 LOAD_NAME                3 (Result)
                 54 BUILD_TUPLE              6
-                56 LOAD_CONST               7 (<code object netmiko_commit, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_commit.py", line 6>)
+                56 LOAD_CONST               7 (<code object netmiko_commit, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_commit.py", line 6>)
                 58 MAKE_FUNCTION            4 (annotations)
                 60 STORE_NAME               7 (netmiko_commit)
                 62 LOAD_CONST               8 (None)
                 64 RETURN_VALUE
    consts
       0
       ('Any',)
@@ -118,20 +118,20 @@
             True
             ('host', 'result', 'changed')
             ()
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'commit', 'check_config_mode', 'exit_config_mode', 'Result')
          varnames   ('task', 'kwargs', 'conn', 'result')
          freevars   ()
          cellvars   ()
-         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
+         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
          name       'netmiko_commit'
          firstlineno 6
          lnotab 0x020b54011a0228012801
       None
    names      ('typing', 'Any', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'netmiko_commit')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0110010c03
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
+moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
 files sz: 1189
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
@@ -59,15 +59,15 @@
      8          68 LOAD_NAME                1 (Any)
    
      7          70 LOAD_CONST               9 ('return')
    
      9          72 LOAD_NAME                5 (Result)
    
      7          74 BUILD_TUPLE             10
-                76 LOAD_CONST              10 (<code object netmiko_file_transfer, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_file_transfer.py", line 7>)
+                76 LOAD_CONST              10 (<code object netmiko_file_transfer, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_file_transfer.py", line 7>)
                 78 MAKE_FUNCTION            4 (annotations)
                 80 STORE_NAME              10 (netmiko_file_transfer)
                 82 LOAD_CONST              11 (None)
                 84 RETURN_VALUE
    consts
       0
       ('Any',)
@@ -183,24 +183,24 @@
             'file_verified'
             'file_transferred'
             ('host', 'result', 'changed')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'setdefault', 'file_transfer', 'get', 'Result')
          varnames   ('task', 'source_file', 'dest_file', 'kwargs', 'net_connect', 'scp_result', 'file_valid')
          freevars   ()
          cellvars   ()
-         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
+         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
          name       'netmiko_file_transfer'
          firstlineno 7
          lnotab
             0x021154012c010c0102ff020104ff040102ff06032e01120220010c011c
             ff
       None
    names      ('typing', 'Any', 'netmiko', 'file_transfer', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'netmiko_file_transfer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c0110010c03020102ff020102ff020102ff020102ff02
       0202fe
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
+moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
 files sz: 1179
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
@@ -77,15 +77,15 @@
     11         118 LOAD_NAME                4 (Any)
    
      6         120 LOAD_CONST              10 ('return')
    
     12         122 LOAD_NAME                6 (Result)
    
      6         124 BUILD_TUPLE             12
-               126 LOAD_CONST              11 (<code object netmiko_multiline, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_multiline.py", line 6>)
+               126 LOAD_CONST              11 (<code object netmiko_multiline, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_multiline.py", line 6>)
                128 MAKE_FUNCTION            5 (defaults, annotations)
                130 STORE_NAME              12 (netmiko_multiline)
                132 LOAD_CONST              12 (None)
                134 RETURN_VALUE
    consts
       0
       ('Sequence', 'Union', 'List', 'Any')
@@ -171,23 +171,23 @@
          consts
             '\n    Execute Netmiko send_multiline method (or send_multiline_timing)\n\n    Arguments:\n        commands: List or list of lists (see Netmiko send_multiline)\n        use_timing: Set to True to switch to send_multiline_timing method.\n        enable: Set to True to force Netmiko .enable() call.\n        kwargs: Additional arguments to pass to send_multiline method.\n\n    Returns:\n        Result object with the following attributes set:\n          * result: String result showing you the output from commands\n    '
             ('host', 'result')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'enable', 'send_multiline_timing', 'send_multiline', 'Result')
          varnames   ('task', 'commands', 'use_timing', 'enable', 'kwargs', 'net_connect', 'result')
          freevars   ()
          cellvars   ()
-         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
+         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
          name       'netmiko_multiline'
          firstlineno 6
          lnotab 0x021454010401280104011e021c01
       None
       (False, False)
    names      ('typing', 'Sequence', 'Union', 'List', 'Any', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'bool', 'netmiko_multiline')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201180110010c06020102fc040102ff02022afe020302fd020402
       fc020502fb020602fa
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
+moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
 files sz: 1061
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
@@ -48,15 +48,15 @@
      6          48 LOAD_NAME                5 (str)
    
      5          50 LOAD_CONST               9 ('return')
    
      7          52 LOAD_NAME                1 (Result)
    
      5          54 BUILD_TUPLE             10
-                56 LOAD_CONST              10 (<code object netmiko_save_config, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_save_config.py", line 5>)
+                56 LOAD_CONST              10 (<code object netmiko_save_config, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_save_config.py", line 5>)
                 58 MAKE_FUNCTION            5 (defaults, annotations)
                 60 STORE_NAME               7 (netmiko_save_config)
                 62 LOAD_CONST              11 (None)
                 64 RETURN_VALUE
    consts
       0
       ('Result', 'Task')
@@ -135,23 +135,23 @@
             ('confirm', 'confirm_response')
             True
             ('host', 'result', 'changed')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'save_config', 'Result')
          varnames   ('task', 'cmd', 'confirm', 'confirm_response', 'conn', 'result')
          freevars   ()
          cellvars   ()
-         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
+         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
          name       'netmiko_save_config'
          firstlineno 5
          lnotab 0x020f54010401180106ff14042e01
       None
       ('', False, '')
    names      ('nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'bool', 'netmiko_save_config')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
+   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c0402ff040102ff020102ff020102ff020102ff020202
       fe
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_commit.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_commit.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Any
-from nornir.core.task import Result, Task
-from nornir_easy_netmiko.connections import CONNECTION_NAME
-
-
-def netmiko_commit(task: Task, **kwargs: Any) -> Result:
-    """
-    Execute Netmiko commit method
-
-    Arguments:
-        kwargs: Additional arguments to pass to method.
-
-    Returns:
-        :obj: `nornir.core.task.Result`:
-          * result (``str``): String showing the CLI output from the commit operation
-    """
-    conn = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    result = conn.commit(**kwargs)
-
-    if conn.check_config_mode():
-        conn.exit_config_mode()
+from typing import Any
+from nornir.core.task import Result, Task
+from nornir_easy_netmiko.connections import CONNECTION_NAME
+
+
+def netmiko_commit(task: Task, **kwargs: Any) -> Result:
+    """
+    Execute Netmiko commit method
+
+    Arguments:
+        kwargs: Additional arguments to pass to method.
+
+    Returns:
+        :obj: `nornir.core.task.Result`:
+          * result (``str``): String showing the CLI output from the commit operation
+    """
+    conn = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
+    result = conn.commit(**kwargs)
+
+    if conn.check_config_mode():
+        conn.exit_config_mode()
     return Result(host=task.host, result=result, changed=True)
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_multiline.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_multiline.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Sequence, Union, List, Any
-from nornir.core.task import Result, Task
-from nornir_easy_netmiko.connections import CONNECTION_NAME
-
-
-def netmiko_multiline(
-    task: Task,
-    commands: Sequence[Union[str, List[str]]],
-    use_timing: bool = False,
-    enable: bool = False,
-    **kwargs: Any
-) -> Result:
-    """
-    Execute Netmiko send_multiline method (or send_multiline_timing)
-
-    Arguments:
-        commands: List or list of lists (see Netmiko send_multiline)
-        use_timing: Set to True to switch to send_multiline_timing method.
-        enable: Set to True to force Netmiko .enable() call.
-        kwargs: Additional arguments to pass to send_multiline method.
-
-    Returns:
-        Result object with the following attributes set:
-          * result: String result showing you the output from commands
-    """
-    net_connect = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    if enable:
-        net_connect.enable()
-    if use_timing:
-        result = net_connect.send_multiline_timing(commands, **kwargs)
-    else:
-        result = net_connect.send_multiline(commands, **kwargs)
-    return Result(host=task.host, result=result)
+from typing import Sequence, Union, List, Any
+from nornir.core.task import Result, Task
+from nornir_easy_netmiko.connections import CONNECTION_NAME
+
+
+def netmiko_multiline(
+    task: Task,
+    commands: Sequence[Union[str, List[str]]],
+    use_timing: bool = False,
+    enable: bool = False,
+    **kwargs: Any
+) -> Result:
+    """
+    Execute Netmiko send_multiline method (or send_multiline_timing)
+
+    Arguments:
+        commands: List or list of lists (see Netmiko send_multiline)
+        use_timing: Set to True to switch to send_multiline_timing method.
+        enable: Set to True to force Netmiko .enable() call.
+        kwargs: Additional arguments to pass to send_multiline method.
+
+    Returns:
+        Result object with the following attributes set:
+          * result: String result showing you the output from commands
+    """
+    net_connect = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
+    if enable:
+        net_connect.enable()
+    if use_timing:
+        result = net_connect.send_multiline_timing(commands, **kwargs)
+    else:
+        result = net_connect.send_multiline(commands, **kwargs)
+    return Result(host=task.host, result=result)
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_save_config.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_save_config.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from nornir.core.task import Result, Task
-from nornir_easy_netmiko.connections import CONNECTION_NAME
-
-
-def netmiko_save_config(
-    task: Task, cmd: str = "", confirm: bool = False, confirm_response: str = ""
-) -> Result:
-    """
-    Execute Netmiko save_config method
-
-    Arguments:
-        cmd(str, optional): Command used to save the configuration.
-        confirm(bool, optional): Does device prompt for confirmation before executing save operation
-        confirm_response(str, optional): Response send to device when it prompts for confirmation
-
-    Returns:
-        :obj: `nornir.core.task.Result`:
-          * result (``str``): String showing the CLI output from the save operation
-    """
-    conn = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    if cmd:
-        result = conn.save_config(
-            cmd=cmd, confirm=confirm, confirm_response=confirm_response
-        )
-    else:
-        result = conn.save_config(confirm=confirm, confirm_response=confirm_response)
-    return Result(host=task.host, result=result, changed=True)
+from nornir.core.task import Result, Task
+from nornir_easy_netmiko.connections import CONNECTION_NAME
+
+
+def netmiko_save_config(
+    task: Task, cmd: str = "", confirm: bool = False, confirm_response: str = ""
+) -> Result:
+    """
+    Execute Netmiko save_config method
+
+    Arguments:
+        cmd(str, optional): Command used to save the configuration.
+        confirm(bool, optional): Does device prompt for confirmation before executing save operation
+        confirm_response(str, optional): Response send to device when it prompts for confirmation
+
+    Returns:
+        :obj: `nornir.core.task.Result`:
+          * result (``str``): String showing the CLI output from the save operation
+    """
+    conn = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
+    if cmd:
+        result = conn.save_config(
+            cmd=cmd, confirm=confirm, confirm_response=confirm_response
+        )
+    else:
+        result = conn.save_config(confirm=confirm, confirm_response=confirm_response)
+    return Result(host=task.host, result=result, changed=True)
```

### Comparing `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_command.py` & `nornir_easy_netmiko-1.1.7/nornir_easy_netmiko/nornir_easy_netmiko/tasks/netmiko_send_command.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Any
-from jinja2 import Template, StrictUndefined
-from nornir.core.task import Result, Task
-from nornir_easy_netmiko.connections import CONNECTION_NAME
-from nornir_easy_netmiko.errors import error_handle
-
-@error_handle
-def netmiko_send_command(
-    task: Task,
-    command_string: str,
-    use_timing: bool = False,
-    enable: bool = False,
-    **kwargs: Any
-) -> Result:
-    """
-    Execute Netmiko send_command method (or send_command_timing)
-
-    Arguments:
-        command_string: Command to execute on the remote network device.
-        use_timing: Set to True to switch to send_command_timing method.
-        enable: Set to True to force Netmiko .enable() call.
-        kwargs: Additional arguments to pass to send_command method.
-
-    Returns:
-        Result object with the following attributes set:
-          * result: Result of the show command (generally a string, but depends on use of TextFSM).
-    """
-    net_connect = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    # Render with jinja2
-    template = Template(command_string, undefined=StrictUndefined, trim_blocks=True)
-    command_string = template.render(task.host.dict())
-
-    if enable:
-        net_connect.enable()
-    if use_timing:
-        result = net_connect.send_command_timing(command_string, **kwargs)
-    else:
-        result = net_connect.send_command(command_string, **kwargs)
+from typing import Any
+from jinja2 import Template, StrictUndefined
+from nornir.core.task import Result, Task
+from nornir_easy_netmiko.connections import CONNECTION_NAME
+from nornir_easy_netmiko.errors import error_handle
+
+@error_handle
+def netmiko_send_command(
+    task: Task,
+    command_string: str,
+    use_timing: bool = False,
+    enable: bool = False,
+    **kwargs: Any
+) -> Result:
+    """
+    Execute Netmiko send_command method (or send_command_timing)
+
+    Arguments:
+        command_string: Command to execute on the remote network device.
+        use_timing: Set to True to switch to send_command_timing method.
+        enable: Set to True to force Netmiko .enable() call.
+        kwargs: Additional arguments to pass to send_command method.
+
+    Returns:
+        Result object with the following attributes set:
+          * result: Result of the show command (generally a string, but depends on use of TextFSM).
+    """
+    net_connect = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
+    # Render with jinja2
+    template = Template(command_string, undefined=StrictUndefined, trim_blocks=True)
+    command_string = template.render(task.host.dict())
+
+    if enable:
+        net_connect.enable()
+    if use_timing:
+        result = net_connect.send_command_timing(command_string, **kwargs)
+    else:
+        result = net_connect.send_command(command_string, **kwargs)
     return Result(host=task.host, result=result)
```

### Comparing `nornir_easy_netmiko-1.1.6/pyproject.toml` & `nornir_easy_netmiko-1.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_easy_netmiko"
-version = "1.1.6"
+version = "1.1.7"
 description = "Netmiko's plugins for Nornir. Support jinja2 and optimized exception."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ['Des1r3 <linzx@anonymous.com>']
 repository = "https://github.com/Des1r3/nornir_easy_netmiko"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `nornir_easy_netmiko-1.1.6/PKG-INFO` & `nornir_easy_netmiko-1.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-easy-netmiko
-Version: 1.1.6
+Version: 1.1.7
 Summary: Netmiko's plugins for Nornir. Support jinja2 and optimized exception.
 Home-page: https://github.com/Des1r3/nornir_easy_netmiko
 License: Apache-2.0
 Author: Des1r3
 Author-email: linzx@anonymous.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

