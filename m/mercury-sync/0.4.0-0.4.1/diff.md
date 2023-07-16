# Comparing `tmp/mercury-sync-0.4.0.tar.gz` & `tmp/mercury-sync-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.4.0.tar", last modified: Fri Jul 14 20:02:14 2023, max compression
+gzip compressed data, was "mercury-sync-0.4.1.tar", last modified: Sun Jul 16 18:21:41 2023, max compression
```

## Comparing `mercury-sync-0.4.0.tar` & `mercury-sync-0.4.1.tar`

### file list

```diff
@@ -1,206 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.775679 mercury-sync-0.4.0/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/addresses/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/addresses/subnet_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/base/connection_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_http_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23338 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_multicast_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/root.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/dns_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/invalid_service_url_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/get_bits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/nameserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/random_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/query_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.799680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/a_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/aaaa_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/cname_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/domain_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/mx_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/naptr_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ns_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ptr_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/soa_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/srv_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/txt_record_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/unsupported_record_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.799680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/registrar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/dns_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/base_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/cache_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/memoizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/proxy_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/recursive_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/discovery/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/volume/backup_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/memory_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/monitor_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/registrar_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/endpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/middleware_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/middleware/base/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/bidirectional_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/unidirectional_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/compressor/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/gzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/zstandard_compressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/cors/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/cors_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/crsf/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/crsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/crsf/crsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_gzip_decompressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_zstandard_decompressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/gzip_decompressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/zstandard_decompressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_message_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/http_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/monitoring/monitor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/rate_limiting/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.823680 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/adaptive_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/base_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/cpu_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/leaky_bucket_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/resource_adaptive_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/sliding_window_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/token_bucket_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.823680 mercury-sync-0.4.0/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29917 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/plugin_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/service/socket/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/socket/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/connection/addresses/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/addresses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/addresses/subnet_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/connection/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/base/connection_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/mercury_sync_http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23338 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/udp/mercury_sync_udp_multicast_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/cache_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/cache_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/root.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/dns_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/invalid_service_url_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/exceptions/utils/get_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/nameservers/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/nameservers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/nameservers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/nameservers/nameserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/random/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/random/random_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/query_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.515785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/a_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/aaaa_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/cname_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/domain_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/mx_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/naptr_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/ns_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/ptr_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/record_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/soa_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/srv_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/txt_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/unsupported_record_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/registrar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/discovery/dns/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/request/dns_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/base_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/cache_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/memoizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/proxy_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/recursive_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/discovery/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/discovery/volume/backup_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/memory_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/monitor_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/registrar_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/endpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/middleware_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.519785 mercury-sync-0.4.1/mercury_sync/middleware/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/bidirectional_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/call_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/base/unidirectional_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/middleware/circuit_breaker/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/circuit_breaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/circuit_breaker/circuit_breaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/circuit_breaker/circuit_breaker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/middleware/compressor/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/compressor/gzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/compressor/zstandard_compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/middleware/cors/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/cors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/cors/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/cors/cors_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/middleware/crsf/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/crsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/crsf/crsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/bidirectional_gzip_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/bidirectional_zstandard_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/gzip_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/middleware/decompressor/zstandard_decompressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/dns_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/dns_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/dns_message_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/http_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/monitoring/monitor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/rate_limiting/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/adaptive_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/base_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/cpu_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/leaky_bucket_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/resource_adaptive_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/sliding_window_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/token_bucket_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.523785 mercury-sync-0.4.1/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30010 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/plugin_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/mercury_sync/service/socket/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/service/socket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:21:41.511785 mercury-sync-0.4.1/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-16 18:21:41.000000 mercury-sync-0.4.1/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-16 18:21:41.000000 mercury-sync-0.4.1/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:21:41.000000 mercury-sync-0.4.1/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 18:21:41.000000 mercury-sync-0.4.1/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-16 18:21:41.000000 mercury-sync-0.4.1/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 18:21:41.527785 mercury-sync-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-16 18:21:38.000000 mercury-sync-0.4.1/setup.py
```

### Comparing `mercury-sync-0.4.0/LICENSE` & `mercury-sync-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/PKG-INFO` & `mercury-sync-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.4.0/README.md` & `mercury-sync-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/addresses/subnet_range.py` & `mercury-sync-0.4.1/mercury_sync/connection/addresses/subnet_range.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_http_connection.py` & `mercury-sync-0.4.1/mercury_sync/connection/tcp/mercury_sync_http_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.4.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.4.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.4.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_multicast_connection.py` & `mercury-sync-0.4.1/mercury_sync/connection/udp/mercury_sync_udp_multicast_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.4.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_node.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/cache_node.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_value.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/cache/cache_value.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/nt.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/nt.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/root.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/config/root.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/nameserver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/nameservers/nameserver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/random_id_generator.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/random/random_id_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/__init__.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/a_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/a_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/aaaa_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/aaaa_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/cname_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/cname_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/domain_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/domain_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/mx_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/mx_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/naptr_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/naptr_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ns_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/ns_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ptr_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/ptr_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_types.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/record_types.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/soa_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/soa_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/srv_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/srv_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/txt_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/txt_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/unsupported_record_data.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/unsupported_record_data.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_domain_name.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_domain_name.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_domain_name.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_domain_name.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/host.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/host.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/url.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/core/url/url.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/registrar.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/registrar.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/request/dns_client.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/request/dns_client.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/base_resolver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/base_resolver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/cache_resolver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/cache_resolver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/memoizer.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/memoizer.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/proxy_resolver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/proxy_resolver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/recursive_resolver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/recursive_resolver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/resolver.py` & `mercury-sync-0.4.1/mercury_sync/discovery/dns/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.4.1/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/env/env.py` & `mercury-sync-0.4.1/mercury_sync/env/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
+    MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_REJECTION_SENSITIVITY: StrictFloat=0.1
+    MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_FAILURE_WINDOW: StrictStr='1m'
+    MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_FAILURE_THRESHOLD: Union[StrictInt, StrictFloat]=0.2
+    MERCURY_SYNC_HTTP_HANDLER_TIMEOUT: StrictStr='1m'
     MERCURY_SYNC_HTTP_RATE_LIMIT_STRATEGY: Literal[
         "none", 
         "global", 
         "endpoint", 
         "ip",
         "ip-endpoint",
         "custom"
@@ -51,15 +55,19 @@
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
     MERCURY_SYNC_MULTICAST_GROUP: IPvAnyAddress='224.1.1.1'
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
+            'MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_REJECTION_SENSITIVITY': float,
+            'MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_FAILURE_WINDOW': str,
+            'MERCURY_SYNC_HTTP_HANDLER_TIMEOUT': str,
             'MERCURY_SYNC_USE_UDP_MULTICAST': lambda value: True if value.lower() == 'true' else False,
+            'MERCURY_SYNC_HTTP_CIRCUIT_BREAKER_FAILURE_THRESHOLD': float,
             'MERCURY_SYNC_HTTP_CORS_ENABLED': lambda value: True if value.lower() == 'true' else False,
             'MERCURY_SYNC_HTTP_MEMORY_LIMIT': str,
             'MERCURY_SYNC_HTTP_RATE_LIMIT_BACKOFF_RATE': int,
             'MERCURY_SYNC_HTTP_RATE_LIMIT_BACKOFF': str,
             'MERCURY_SYNC_HTTP_CPU_LIMIT': float,
             'MERCURY_SYNC_HTTP_RATE_LIMIT_STRATEGY': str,
             'MERCURY_SYNC_HTTP_RATE_LIMIT_PERIOD': str,
```

### Comparing `mercury-sync-0.4.0/mercury_sync/env/load_env.py` & `mercury-sync-0.4.1/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/env/memory_parser.py` & `mercury-sync-0.4.1/mercury_sync/env/memory_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/env/monitor_env.py` & `mercury-sync-0.4.1/mercury_sync/env/monitor_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/env/registrar_env.py` & `mercury-sync-0.4.1/mercury_sync/env/registrar_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/env/time_parser.py` & `mercury-sync-0.4.1/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.4.1/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/hooks/endpoint_hook.py` & `mercury-sync-0.4.1/mercury_sync/hooks/endpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.4.1/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/base/bidirectional_wrapper.py` & `mercury-sync-0.4.1/mercury_sync/middleware/base/bidirectional_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-from mercury_sync.models.response import Response
 from mercury_sync.models.request import Request
 from pydantic import BaseModel
 from typing import (
     Callable, 
     Union, 
     Dict, 
     Optional,
```

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/base/middleware.py` & `mercury-sync-0.4.1/mercury_sync/middleware/base/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Dict, 
     Optional,
     List,
     Literal,
     Tuple
 )
 from .bidirectional_wrapper import BidirectionalWrapper
+from .call_wrapper import CallWrapper
 from .unidirectional_wrapper import UnidirectionalWrapper
 from .types import MiddlewareType
 
 
 class Middleware:
 
     def __init__(
@@ -40,17 +41,19 @@
         response_headers: Dict[str, str]={}
     ) -> None:
         
         self.name = name
         self.methods = methods
         self.response_headers = response_headers
         self.middleware_type = middleware_type
+        self.wraps = False
 
         self._wrapper_types = {
             MiddlewareType.BIDIRECTIONAL: BidirectionalWrapper,
+            MiddlewareType.CALL: CallWrapper,
             MiddlewareType.UNIDIRECTIONAL_BEFORE: UnidirectionalWrapper,
             MiddlewareType.UNIDIRECTIONAL_AFTER: UnidirectionalWrapper,
         }
 
     def __call__(self, request: Request) -> Tuple[
         Tuple[Response, int],
         bool
@@ -86,22 +89,28 @@
             middleware_type=self.middleware_type 
         )
 
         if isinstance(wrapper, BidirectionalWrapper):
             wrapper.pre = self.__pre__
             wrapper.post = self.__post__
 
-        elif isinstance(wrapper, UnidirectionalWrapper):
+        elif isinstance(wrapper, (CallWrapper, UnidirectionalWrapper)):
 
             wrapper.run = self.__run__
         
             self.response_headers.update(wrapper.response_headers)
+
+        wrapper.setup = self.__setup__
+        self.wraps = wrapper.wraps
         
         return wrapper
     
+    async def __setup__(self):
+        pass
+    
     async def __pre__(
         self, 
         request: Request,
         response: Response,
         status: int
     ) -> Tuple[
         Tuple[
```

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/base/types.py` & `mercury-sync-0.4.1/mercury_sync/middleware/base/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Tuple,
     Coroutine
 )
 
 
 class MiddlewareType(Enum):
     BIDIRECTIONAL='BIDIRECTIONAL'
+    CALL='CALL'
     UNIDIRECTIONAL_BEFORE='UNIDIRECTIONAL_BEFORE'
     UNIDIRECTIONAL_AFTER='UNIDIRECTIONAL_AFTER'
 
 
 RequestHandler = Callable[
     [Request],
     Coroutine[
@@ -46,14 +47,30 @@
         Tuple[
             Response,
             int
         ]
     ]
 ]
 
+CallHandler = Callable[
+    [
+        Request,
+        RequestHandler
+    ],
+    Coroutine[
+        Any, 
+        Any, 
+        Tuple[
+            Request,
+            Response, 
+            int
+        ]
+    ]
+]
+
 MiddlewareHandler = Callable[
     [
         Request,
         Response,
         int
     ],
     Coroutine[
@@ -63,14 +80,15 @@
             Tuple[Response, int],
             bool
         ]
     ]
 ]
 
 
+
 BidirectionalMiddlewareHandler = Callable[
     [
         Request,
         Response,
         int
     ],
     Coroutine[
```

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/base/unidirectional_wrapper.py` & `mercury-sync-0.4.1/mercury_sync/middleware/base/unidirectional_wrapper.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/compressor/gzip_compressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/compressor/gzip_compressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/compressor/zstandard_compressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/compressor/zstandard_compressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/cors/cors.py` & `mercury-sync-0.4.1/mercury_sync/middleware/cors/cors.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/cors/cors_headers.py` & `mercury-sync-0.4.1/mercury_sync/middleware/cors/cors_headers.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/crsf/crsf.py` & `mercury-sync-0.4.1/mercury_sync/middleware/crsf/crsf.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_gzip_decompressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/decompressor/bidirectional_gzip_decompressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_zstandard_decompressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/decompressor/bidirectional_zstandard_decompressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/decompressor/gzip_decompressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/decompressor/gzip_decompressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/middleware/decompressor/zstandard_decompressor.py` & `mercury-sync-0.4.1/mercury_sync/middleware/decompressor/zstandard_decompressor.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/dns_entry.py` & `mercury-sync-0.4.1/mercury_sync/models/dns_entry.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/dns_message.py` & `mercury-sync-0.4.1/mercury_sync/models/dns_message.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/healthcheck.py` & `mercury-sync-0.4.1/mercury_sync/models/healthcheck.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/http_message.py` & `mercury-sync-0.4.1/mercury_sync/models/http_message.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/http_request.py` & `mercury-sync-0.4.1/mercury_sync/models/http_request.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/limit.py` & `mercury-sync-0.4.1/mercury_sync/models/limit.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/request.py` & `mercury-sync-0.4.1/mercury_sync/models/request.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/response.py` & `mercury-sync-0.4.1/mercury_sync/models/response.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/models/service.py` & `mercury-sync-0.4.1/mercury_sync/models/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/monitoring/monitor_service.py` & `mercury-sync-0.4.1/mercury_sync/monitoring/monitor_service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/adaptive_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/adaptive_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/base_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/base_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/cpu_adaptive.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/cpu_adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         self._min_backoff = self._backoff
         self._max_fast_backoff = math.ceil(self._backoff * 10)
         self._max_backoff = math.ceil(self._max_fast_backoff * 10)
         self._last_check = self._loop.time()
         self._current_time = self._loop.time()
         self._previous_count = limit.max_requests
 
-
         self._history: List[float] = []
 
         self._max_queue = limit.max_requests
         self._sample_task: Union[asyncio.Task, None] = None
         self._running = False
         self._activate_limit = False
         self._process = psutil.Process(os.getpid())
```

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/leaky_bucket_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/leaky_bucket_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/resource_adaptive_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/resource_adaptive_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/sliding_window_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/sliding_window_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/token_bucket_limiter.py` & `mercury-sync-0.4.1/mercury_sync/rate_limiting/limiters/token_bucket_limiter.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/service/controller.py` & `mercury-sync-0.4.1/mercury_sync/service/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,17 @@
             )
 
     async def start_server(
       self,
       cert_path: Optional[str]=None,
       key_path: Optional[str]=None      
     ):
+        
+        for middleware in self.middleware:
+            await middleware.__setup__()
 
         pool: List[asyncio.Future] = []
 
         loop = asyncio.get_event_loop()
 
         if self.engine_type == "process":
             engine = ProcessPoolExecutor(
```

### Comparing `mercury-sync-0.4.0/mercury_sync/service/plugin_group.py` & `mercury-sync-0.4.1/mercury_sync/service/plugin_group.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/service/service.py` & `mercury-sync-0.4.1/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/service/socket/socket.py` & `mercury-sync-0.4.1/mercury_sync/service/socket/socket.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.4.1/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.4.1/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.4.0/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.4.1/mercury_sync.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.4.0/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.4.1/mercury_sync.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,21 @@
 mercury_sync/hooks/middleware_hook.py
 mercury_sync/hooks/server_hook.py
 mercury_sync/hooks/stream_hook.py
 mercury_sync/middleware/__init__.py
 mercury_sync/middleware/base/__init__.py
 mercury_sync/middleware/base/base_wrapper.py
 mercury_sync/middleware/base/bidirectional_wrapper.py
+mercury_sync/middleware/base/call_wrapper.py
 mercury_sync/middleware/base/middleware.py
 mercury_sync/middleware/base/types.py
 mercury_sync/middleware/base/unidirectional_wrapper.py
+mercury_sync/middleware/circuit_breaker/__init__.py
+mercury_sync/middleware/circuit_breaker/circuit_breaker.py
+mercury_sync/middleware/circuit_breaker/circuit_breaker_state.py
 mercury_sync/middleware/compressor/__init__.py
 mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py
 mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py
 mercury_sync/middleware/compressor/gzip_compressor.py
 mercury_sync/middleware/compressor/zstandard_compressor.py
 mercury_sync/middleware/cors/__init__.py
 mercury_sync/middleware/cors/cors.py
```

### Comparing `mercury-sync-0.4.0/setup.py` & `mercury-sync-0.4.1/setup.py`

 * *Files identical despite different names*

