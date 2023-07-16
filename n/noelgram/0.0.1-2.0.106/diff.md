# Comparing `tmp/noelgram-0.0.1.tar.gz` & `tmp/noelgram-2.0.106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noelgram-0.0.1.tar", last modified: Sun Jul 16 03:12:37 2023, max compression
+gzip compressed data, was "noelgram-2.0.106.tar", last modified: Sun Jul 16 03:05:43 2023, max compression
```

## Comparing `noelgram-0.0.1.tar` & `noelgram-2.0.106.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.884765 noelgram-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-16 03:04:41.000000 noelgram-0.0.1/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-16 03:04:41.000000 noelgram-0.0.1/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      305 2023-07-16 03:04:41.000000 noelgram-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-16 03:04:41.000000 noelgram-0.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4332 2023-07-16 03:12:37.884765 noelgram-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 03:04:41.000000 noelgram-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.824764 noelgram-0.0.1/compiler/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.824764 noelgram-0.0.1/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22917 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/api/source/
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/source/auth_key.tl
--rw-r--r--   0 root         (0) root         (0)   168867 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/source/main_api.tl
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/api/template/
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/template/combinator.txt
--rw-r--r--   0 root         (0) root         (0)      547 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/api/template/type.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/docs/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19230 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/docs/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/docs/template/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/docs/template/page.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/errors/source/
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 root         (0) root         (0)    22642 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 root         (0) root         (0)     2000 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 root         (0) root         (0)     4219 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.828764 noelgram-0.0.1/compiler/errors/template/
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/template/class.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-16 03:04:41.000000 noelgram-0.0.1/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.832764 noelgram-0.0.1/noelgram/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-07-16 03:12:07.000000 noelgram-0.0.1/noelgram/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45007 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.832764 noelgram-0.0.1/noelgram/connection/
--rw-r--r--   0 root         (0) root         (0)      854 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2575 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.832764 noelgram-0.0.1/noelgram/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.832764 noelgram-0.0.1/noelgram/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.836764 noelgram-0.0.1/noelgram/crypto/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4059 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    13485 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    10308 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   209155 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.836764 noelgram-0.0.1/noelgram/enums/
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4203 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.836764 noelgram-0.0.1/noelgram/errors/
--rw-r--r--   0 root         (0) root         (0)     2646 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15602 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/file_id.py
--rw-r--r--   0 root         (0) root         (0)    24930 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.840764 noelgram-0.0.1/noelgram/handlers/
--rw-r--r--   0 root         (0) root         (0)     1475 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.840764 noelgram-0.0.1/noelgram/methods/
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.840764 noelgram-0.0.1/noelgram/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8565 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.840764 noelgram-0.0.1/noelgram/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1656 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.844764 noelgram-0.0.1/noelgram/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2042 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3264 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.848764 noelgram-0.0.1/noelgram/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     3440 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4014 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3206 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5219 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1715 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4523 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.848764 noelgram-0.0.1/noelgram/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1138 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.852764 noelgram-0.0.1/noelgram/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     1625 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.852764 noelgram-0.0.1/noelgram/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3515 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2336 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.860765 noelgram-0.0.1/noelgram/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     3922 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5182 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7751 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10551 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3918 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     4542 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     1951 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4756 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5292 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    13081 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    11465 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     5554 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    10979 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    21073 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     7292 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)     9789 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)     8213 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8714 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    12467 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)     9643 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     4068 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/messages/vote_poll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.860765 noelgram-0.0.1/noelgram/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.864765 noelgram-0.0.1/noelgram/methods/users/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.864765 noelgram-0.0.1/noelgram/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1254 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61915 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.864765 noelgram-0.0.1/noelgram/parser/
--rw-r--r--   0 root         (0) root         (0)      846 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8826 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     6152 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.864765 noelgram-0.0.1/noelgram/raw/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.864765 noelgram-0.0.1/noelgram/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/session/
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11925 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/session/internals/
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    14163 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/storage/
--rw-r--r--   0 root         (0) root         (0)      928 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     5932 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3982 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/types/
--rw-r--r--   0 root         (0) root         (0)     1109 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.868765 noelgram-0.0.1/noelgram/types/authorization/
--rw-r--r--   0 root         (0) root         (0)      938 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.872765 noelgram-0.0.1/noelgram/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     2840 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12847 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     7606 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     3370 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.876765 noelgram-0.0.1/noelgram/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3783 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7321 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5853 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4468 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4276 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5343 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5560 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.876765 noelgram-0.0.1/noelgram/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     3283 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.876765 noelgram-0.0.1/noelgram/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1000 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     2671 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.880765 noelgram-0.0.1/noelgram/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)   145825 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     4213 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     7069 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3773 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/object.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.884765 noelgram-0.0.1/noelgram/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32566 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)    20448 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5524 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4552 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9490 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     4443 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    12844 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    10495 2023-07-16 03:04:41.000000 noelgram-0.0.1/noelgram/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.832764 noelgram-0.0.1/noelgram.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-07-16 03:12:37.000000 noelgram-0.0.1/noelgram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18790 2023-07-16 03:12:37.000000 noelgram-0.0.1/noelgram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 03:12:37.000000 noelgram-0.0.1/noelgram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 03:05:43.000000 noelgram-0.0.1/noelgram.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-16 03:12:37.000000 noelgram-0.0.1/noelgram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 03:12:37.000000 noelgram-0.0.1/noelgram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-16 03:04:41.000000 noelgram-0.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 03:12:37.884765 noelgram-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3469 2023-07-16 03:04:41.000000 noelgram-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.884765 noelgram-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.884765 noelgram-0.0.1/tests/filters/
--rw-r--r--   0 root         (0) root         (0)     1202 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/filters/test_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:12:37.884765 noelgram-0.0.1/tests/parser/
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7282 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/parser/test_html.py
--rw-r--r--   0 root         (0) root         (0)     8352 2023-07-16 03:04:41.000000 noelgram-0.0.1/tests/test_file_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.633391 noelgram-2.0.106/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-16 03:04:41.000000 noelgram-2.0.106/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-16 03:04:41.000000 noelgram-2.0.106/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-16 03:04:41.000000 noelgram-2.0.106/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-16 03:04:41.000000 noelgram-2.0.106/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-07-16 03:05:43.633391 noelgram-2.0.106/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 03:04:41.000000 noelgram-2.0.106/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.573389 noelgram-2.0.106/compiler/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.573389 noelgram-2.0.106/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22917 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/api/source/
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/source/auth_key.tl
+-rw-r--r--   0 root         (0) root         (0)   168867 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/source/main_api.tl
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/api/template/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/template/combinator.txt
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/api/template/type.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/docs/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19230 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/docs/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/docs/template/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/docs/template/page.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/errors/source/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 root         (0) root         (0)    22642 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.577389 noelgram-2.0.106/compiler/errors/template/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/template/class.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-16 03:04:41.000000 noelgram-2.0.106/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram/
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45007 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram/connection/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram/crypto/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    13485 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    10308 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   209155 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.585389 noelgram-2.0.106/noelgram/enums/
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.585389 noelgram-2.0.106/noelgram/errors/
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15602 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    24930 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.585389 noelgram-2.0.106/noelgram/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.585389 noelgram-2.0.106/noelgram/methods/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.589389 noelgram-2.0.106/noelgram/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8565 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.589389 noelgram-2.0.106/noelgram/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.593389 noelgram-2.0.106/noelgram/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.597389 noelgram-2.0.106/noelgram/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4014 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5219 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4523 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.597389 noelgram-2.0.106/noelgram/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.597389 noelgram-2.0.106/noelgram/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.601390 noelgram-2.0.106/noelgram/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.609390 noelgram-2.0.106/noelgram/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5182 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7751 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10551 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4542 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4756 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    13081 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    11465 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    10979 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    21073 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     9789 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)     8213 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8714 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)     9643 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/messages/vote_poll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.609390 noelgram-2.0.106/noelgram/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.609390 noelgram-2.0.106/noelgram/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.613390 noelgram-2.0.106/noelgram/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61915 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.613390 noelgram-2.0.106/noelgram/parser/
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.613390 noelgram-2.0.106/noelgram/raw/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.613390 noelgram-2.0.106/noelgram/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.613390 noelgram-2.0.106/noelgram/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.617390 noelgram-2.0.106/noelgram/session/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11925 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.617390 noelgram-2.0.106/noelgram/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    14163 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.617390 noelgram-2.0.106/noelgram/storage/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.617390 noelgram-2.0.106/noelgram/types/
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.617390 noelgram-2.0.106/noelgram/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)      938 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.621390 noelgram-2.0.106/noelgram/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12847 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     7606 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.625390 noelgram-2.0.106/noelgram/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3783 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7321 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5343 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5560 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.625390 noelgram-2.0.106/noelgram/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.625390 noelgram-2.0.106/noelgram/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.629390 noelgram-2.0.106/noelgram/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)   145825 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4213 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6404 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/object.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.633391 noelgram-2.0.106/noelgram/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32566 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)    20448 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9490 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    12844 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    10495 2023-07-16 03:04:41.000000 noelgram-2.0.106/noelgram/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.581389 noelgram-2.0.106/noelgram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18790 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 03:05:43.000000 noelgram-2.0.106/noelgram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-16 03:04:41.000000 noelgram-2.0.106/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 03:05:43.633391 noelgram-2.0.106/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-07-16 03:04:41.000000 noelgram-2.0.106/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.633391 noelgram-2.0.106/tests/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.633391 noelgram-2.0.106/tests/filters/
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/filters/test_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 03:05:43.633391 noelgram-2.0.106/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7282 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/parser/test_html.py
+-rw-r--r--   0 root         (0) root         (0)     8352 2023-07-16 03:04:41.000000 noelgram-2.0.106/tests/test_file_id.py
```

### Comparing `noelgram-0.0.1/COPYING` & `noelgram-2.0.106/COPYING`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/COPYING.lesser` & `noelgram-2.0.106/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/NOTICE` & `noelgram-2.0.106/NOTICE`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/PKG-INFO` & `noelgram-2.0.106/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noelgram
-Version: 0.0.1
+Version: 2.0.106
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram
 Author: NOEL
 Author-email: ajual7832@gmail.com
 License: LGPLv3
 Download-URL: https://github.com/jokokendi/noelgram/releases/latest
 Project-URL: Tracker, https://github.com/jokokendi/noelgram/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noelgram Version: 0.0.1 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: noelgram Version: 2.0.106 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram Author: NOEL Author-email:
 ajual7832@gmail.com License: LGPLv3 Download-URL: https://github.com/jokokendi/
 noelgram/releases/latest Project-URL: Tracker, https://github.com/jokokendi/
 noelgram/issues Project-URL: Community, https://t.me/aruna_mutual Project-URL:
 Source, https://github.com/jokokendi/noelgram Keywords: telegram chat messenger
 mtproto api client library python Platform: UNKNOWN Classifier: Development
```

### Comparing `noelgram-0.0.1/README.md` & `noelgram-2.0.106/README.md`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/__init__.py` & `noelgram-2.0.106/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/__init__.py` & `noelgram-2.0.106/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/compiler.py` & `noelgram-2.0.106/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/source/auth_key.tl` & `noelgram-2.0.106/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/source/main_api.tl` & `noelgram-2.0.106/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/source/sys_msgs.tl` & `noelgram-2.0.106/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/template/combinator.txt` & `noelgram-2.0.106/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/api/template/type.txt` & `noelgram-2.0.106/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/docs/__init__.py` & `noelgram-2.0.106/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/docs/compiler.py` & `noelgram-2.0.106/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/__init__.py` & `noelgram-2.0.106/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/compiler.py` & `noelgram-2.0.106/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/sort.py` & `noelgram-2.0.106/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv` & `noelgram-2.0.106/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv` & `noelgram-2.0.106/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv` & `noelgram-2.0.106/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `noelgram-2.0.106/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `noelgram-2.0.106/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/__init__.py` & `noelgram-2.0.106/noelgram/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with noelgram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.0.1"
+__version__ = "2.0.106"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
-__copyright__ = "Copyright (C) 2017-present Noel <https://github.com/jokokendi>"
+__copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
     pass
```

### Comparing `noelgram-0.0.1/noelgram/client.py` & `noelgram-2.0.106/noelgram/client.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/__init__.py` & `noelgram-2.0.106/noelgram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/connection.py` & `noelgram-2.0.106/noelgram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/__init__.py` & `noelgram-2.0.106/noelgram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/__init__.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_abridged.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_abridged_o.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_full.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate_o.py` & `noelgram-2.0.106/noelgram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/crypto/__init__.py` & `noelgram-2.0.106/noelgram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/crypto/aes.py` & `noelgram-2.0.106/noelgram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/crypto/mtproto.py` & `noelgram-2.0.106/noelgram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/crypto/prime.py` & `noelgram-2.0.106/noelgram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/crypto/rsa.py` & `noelgram-2.0.106/noelgram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/dispatcher.py` & `noelgram-2.0.106/noelgram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/emoji.py` & `noelgram-2.0.106/noelgram/emoji.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/__init__.py` & `noelgram-2.0.106/noelgram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/auto_name.py` & `noelgram-2.0.106/noelgram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/chat_action.py` & `noelgram-2.0.106/noelgram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/chat_event_action.py` & `noelgram-2.0.106/noelgram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/chat_member_status.py` & `noelgram-2.0.106/noelgram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/chat_members_filter.py` & `noelgram-2.0.106/noelgram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/chat_type.py` & `noelgram-2.0.106/noelgram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/message_entity_type.py` & `noelgram-2.0.106/noelgram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/message_media_type.py` & `noelgram-2.0.106/noelgram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/message_service_type.py` & `noelgram-2.0.106/noelgram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/messages_filter.py` & `noelgram-2.0.106/noelgram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/next_code_type.py` & `noelgram-2.0.106/noelgram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/parse_mode.py` & `noelgram-2.0.106/noelgram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/poll_type.py` & `noelgram-2.0.106/noelgram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/sent_code_type.py` & `noelgram-2.0.106/noelgram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/enums/user_status.py` & `noelgram-2.0.106/noelgram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/errors/__init__.py` & `noelgram-2.0.106/noelgram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/errors/rpc_error.py` & `noelgram-2.0.106/noelgram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/file_id.py` & `noelgram-2.0.106/noelgram/file_id.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/filters.py` & `noelgram-2.0.106/noelgram/filters.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/__init__.py` & `noelgram-2.0.106/noelgram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/callback_query_handler.py` & `noelgram-2.0.106/noelgram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/chat_join_request_handler.py` & `noelgram-2.0.106/noelgram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/chat_member_updated_handler.py` & `noelgram-2.0.106/noelgram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/chosen_inline_result_handler.py` & `noelgram-2.0.106/noelgram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/deleted_messages_handler.py` & `noelgram-2.0.106/noelgram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/disconnect_handler.py` & `noelgram-2.0.106/noelgram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/edited_message_handler.py` & `noelgram-2.0.106/noelgram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/handler.py` & `noelgram-2.0.106/noelgram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/inline_query_handler.py` & `noelgram-2.0.106/noelgram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/message_handler.py` & `noelgram-2.0.106/noelgram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/poll_handler.py` & `noelgram-2.0.106/noelgram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/raw_update_handler.py` & `noelgram-2.0.106/noelgram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/handlers/user_status_handler.py` & `noelgram-2.0.106/noelgram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/__init__.py` & `noelgram-2.0.106/noelgram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/advanced/__init__.py` & `noelgram-2.0.106/noelgram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/advanced/invoke.py` & `noelgram-2.0.106/noelgram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/advanced/resolve_peer.py` & `noelgram-2.0.106/noelgram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/advanced/save_file.py` & `noelgram-2.0.106/noelgram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/__init__.py` & `noelgram-2.0.106/noelgram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/accept_terms_of_service.py` & `noelgram-2.0.106/noelgram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/check_password.py` & `noelgram-2.0.106/noelgram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/connect.py` & `noelgram-2.0.106/noelgram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/disconnect.py` & `noelgram-2.0.106/noelgram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/get_password_hint.py` & `noelgram-2.0.106/noelgram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/initialize.py` & `noelgram-2.0.106/noelgram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/log_out.py` & `noelgram-2.0.106/noelgram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/recover_password.py` & `noelgram-2.0.106/noelgram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/resend_code.py` & `noelgram-2.0.106/noelgram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/send_code.py` & `noelgram-2.0.106/noelgram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/send_recovery_code.py` & `noelgram-2.0.106/noelgram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/sign_in.py` & `noelgram-2.0.106/noelgram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/sign_in_bot.py` & `noelgram-2.0.106/noelgram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/sign_up.py` & `noelgram-2.0.106/noelgram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/auth/terminate.py` & `noelgram-2.0.106/noelgram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/__init__.py` & `noelgram-2.0.106/noelgram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/answer_callback_query.py` & `noelgram-2.0.106/noelgram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/answer_inline_query.py` & `noelgram-2.0.106/noelgram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/answer_web_app_query.py` & `noelgram-2.0.106/noelgram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/delete_bot_commands.py` & `noelgram-2.0.106/noelgram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/get_bot_commands.py` & `noelgram-2.0.106/noelgram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/get_bot_default_privileges.py` & `noelgram-2.0.106/noelgram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/get_chat_menu_button.py` & `noelgram-2.0.106/noelgram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/get_game_high_scores.py` & `noelgram-2.0.106/noelgram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/get_inline_bot_results.py` & `noelgram-2.0.106/noelgram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/request_callback_answer.py` & `noelgram-2.0.106/noelgram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/send_game.py` & `noelgram-2.0.106/noelgram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/send_inline_bot_result.py` & `noelgram-2.0.106/noelgram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/set_bot_commands.py` & `noelgram-2.0.106/noelgram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/set_bot_default_privileges.py` & `noelgram-2.0.106/noelgram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/set_chat_menu_button.py` & `noelgram-2.0.106/noelgram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/bots/set_game_score.py` & `noelgram-2.0.106/noelgram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/__init__.py` & `noelgram-2.0.106/noelgram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/add_chat_members.py` & `noelgram-2.0.106/noelgram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/archive_chats.py` & `noelgram-2.0.106/noelgram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/ban_chat_member.py` & `noelgram-2.0.106/noelgram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/create_channel.py` & `noelgram-2.0.106/noelgram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/create_group.py` & `noelgram-2.0.106/noelgram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/create_supergroup.py` & `noelgram-2.0.106/noelgram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/delete_channel.py` & `noelgram-2.0.106/noelgram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/delete_chat_photo.py` & `noelgram-2.0.106/noelgram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/delete_supergroup.py` & `noelgram-2.0.106/noelgram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/delete_user_history.py` & `noelgram-2.0.106/noelgram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat_event_log.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat_member.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat_members.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat_members_count.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_chat_online_count.py` & `noelgram-2.0.106/noelgram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_dialogs.py` & `noelgram-2.0.106/noelgram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_dialogs_count.py` & `noelgram-2.0.106/noelgram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_nearby_chats.py` & `noelgram-2.0.106/noelgram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/get_send_as_chats.py` & `noelgram-2.0.106/noelgram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/join_chat.py` & `noelgram-2.0.106/noelgram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/leave_chat.py` & `noelgram-2.0.106/noelgram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/mark_chat_unread.py` & `noelgram-2.0.106/noelgram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/pin_chat_message.py` & `noelgram-2.0.106/noelgram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/promote_chat_member.py` & `noelgram-2.0.106/noelgram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/restrict_chat_member.py` & `noelgram-2.0.106/noelgram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_administrator_title.py` & `noelgram-2.0.106/noelgram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_description.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_permissions.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_photo.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_protected_content.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_title.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_chat_username.py` & `noelgram-2.0.106/noelgram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_send_as_chat.py` & `noelgram-2.0.106/noelgram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/set_slow_mode.py` & `noelgram-2.0.106/noelgram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/unarchive_chats.py` & `noelgram-2.0.106/noelgram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/unban_chat_member.py` & `noelgram-2.0.106/noelgram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/unpin_all_chat_messages.py` & `noelgram-2.0.106/noelgram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/chats/unpin_chat_message.py` & `noelgram-2.0.106/noelgram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/__init__.py` & `noelgram-2.0.106/noelgram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/add_contact.py` & `noelgram-2.0.106/noelgram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/delete_contacts.py` & `noelgram-2.0.106/noelgram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/get_contacts.py` & `noelgram-2.0.106/noelgram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/get_contacts_count.py` & `noelgram-2.0.106/noelgram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/contacts/import_contacts.py` & `noelgram-2.0.106/noelgram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/__init__.py` & `noelgram-2.0.106/noelgram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_callback_query.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_chat_join_request.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_chat_member_updated.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_chosen_inline_result.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_deleted_messages.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_disconnect.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_edited_message.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_inline_query.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_message.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_poll.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_raw_update.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/decorators/on_user_status.py` & `noelgram-2.0.106/noelgram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/__init__.py` & `noelgram-2.0.106/noelgram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/approve_all_chat_join_requests.py` & `noelgram-2.0.106/noelgram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/approve_chat_join_request.py` & `noelgram-2.0.106/noelgram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/create_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/decline_all_chat_join_requests.py` & `noelgram-2.0.106/noelgram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/decline_chat_join_request.py` & `noelgram-2.0.106/noelgram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/delete_chat_admin_invite_links.py` & `noelgram-2.0.106/noelgram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/delete_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/edit_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/export_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/get_chat_join_requests.py` & `noelgram-2.0.106/noelgram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/invite_links/revoke_chat_invite_link.py` & `noelgram-2.0.106/noelgram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/__init__.py` & `noelgram-2.0.106/noelgram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/copy_media_group.py` & `noelgram-2.0.106/noelgram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/copy_message.py` & `noelgram-2.0.106/noelgram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/delete_messages.py` & `noelgram-2.0.106/noelgram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/download_media.py` & `noelgram-2.0.106/noelgram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_inline_caption.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_inline_media.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_inline_reply_markup.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_inline_text.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_message_caption.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_message_media.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_message_reply_markup.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/edit_message_text.py` & `noelgram-2.0.106/noelgram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/forward_messages.py` & `noelgram-2.0.106/noelgram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_chat_history.py` & `noelgram-2.0.106/noelgram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_chat_history_count.py` & `noelgram-2.0.106/noelgram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_custom_emoji_stickers.py` & `noelgram-2.0.106/noelgram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_discussion_message.py` & `noelgram-2.0.106/noelgram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_discussion_replies.py` & `noelgram-2.0.106/noelgram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_discussion_replies_count.py` & `noelgram-2.0.106/noelgram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_media_group.py` & `noelgram-2.0.106/noelgram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/get_messages.py` & `noelgram-2.0.106/noelgram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/inline_session.py` & `noelgram-2.0.106/noelgram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/read_chat_history.py` & `noelgram-2.0.106/noelgram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/retract_vote.py` & `noelgram-2.0.106/noelgram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/search_global.py` & `noelgram-2.0.106/noelgram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/search_global_count.py` & `noelgram-2.0.106/noelgram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/search_messages.py` & `noelgram-2.0.106/noelgram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/search_messages_count.py` & `noelgram-2.0.106/noelgram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_animation.py` & `noelgram-2.0.106/noelgram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_audio.py` & `noelgram-2.0.106/noelgram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_cached_media.py` & `noelgram-2.0.106/noelgram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_chat_action.py` & `noelgram-2.0.106/noelgram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_contact.py` & `noelgram-2.0.106/noelgram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_dice.py` & `noelgram-2.0.106/noelgram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_document.py` & `noelgram-2.0.106/noelgram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_location.py` & `noelgram-2.0.106/noelgram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_media_group.py` & `noelgram-2.0.106/noelgram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_message.py` & `noelgram-2.0.106/noelgram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_photo.py` & `noelgram-2.0.106/noelgram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_poll.py` & `noelgram-2.0.106/noelgram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_reaction.py` & `noelgram-2.0.106/noelgram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_sticker.py` & `noelgram-2.0.106/noelgram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_venue.py` & `noelgram-2.0.106/noelgram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_video.py` & `noelgram-2.0.106/noelgram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_video_note.py` & `noelgram-2.0.106/noelgram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/send_voice.py` & `noelgram-2.0.106/noelgram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/stop_poll.py` & `noelgram-2.0.106/noelgram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/stream_media.py` & `noelgram-2.0.106/noelgram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/messages/vote_poll.py` & `noelgram-2.0.106/noelgram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/password/__init__.py` & `noelgram-2.0.106/noelgram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/password/change_cloud_password.py` & `noelgram-2.0.106/noelgram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/password/enable_cloud_password.py` & `noelgram-2.0.106/noelgram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/password/remove_cloud_password.py` & `noelgram-2.0.106/noelgram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/__init__.py` & `noelgram-2.0.106/noelgram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/block_user.py` & `noelgram-2.0.106/noelgram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/delete_profile_photos.py` & `noelgram-2.0.106/noelgram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_chat_photos.py` & `noelgram-2.0.106/noelgram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_chat_photos_count.py` & `noelgram-2.0.106/noelgram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_common_chats.py` & `noelgram-2.0.106/noelgram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_default_emoji_statuses.py` & `noelgram-2.0.106/noelgram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_me.py` & `noelgram-2.0.106/noelgram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/get_users.py` & `noelgram-2.0.106/noelgram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/set_emoji_status.py` & `noelgram-2.0.106/noelgram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/set_profile_photo.py` & `noelgram-2.0.106/noelgram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/set_username.py` & `noelgram-2.0.106/noelgram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/unblock_user.py` & `noelgram-2.0.106/noelgram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/users/update_profile.py` & `noelgram-2.0.106/noelgram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/__init__.py` & `noelgram-2.0.106/noelgram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/add_handler.py` & `noelgram-2.0.106/noelgram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/compose.py` & `noelgram-2.0.106/noelgram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/export_session_string.py` & `noelgram-2.0.106/noelgram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/idle.py` & `noelgram-2.0.106/noelgram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/remove_handler.py` & `noelgram-2.0.106/noelgram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/restart.py` & `noelgram-2.0.106/noelgram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/run.py` & `noelgram-2.0.106/noelgram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/start.py` & `noelgram-2.0.106/noelgram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/stop.py` & `noelgram-2.0.106/noelgram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/methods/utilities/stop_transmission.py` & `noelgram-2.0.106/noelgram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/mime_types.py` & `noelgram-2.0.106/noelgram/mime_types.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/parser/__init__.py` & `noelgram-2.0.106/noelgram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/parser/html.py` & `noelgram-2.0.106/noelgram/parser/html.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/parser/markdown.py` & `noelgram-2.0.106/noelgram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/parser/parser.py` & `noelgram-2.0.106/noelgram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/parser/utils.py` & `noelgram-2.0.106/noelgram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/__init__.py` & `noelgram-2.0.106/noelgram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/__init__.py` & `noelgram-2.0.106/noelgram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/future_salt.py` & `noelgram-2.0.106/noelgram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/future_salts.py` & `noelgram-2.0.106/noelgram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/gzip_packed.py` & `noelgram-2.0.106/noelgram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/list.py` & `noelgram-2.0.106/noelgram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/message.py` & `noelgram-2.0.106/noelgram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/msg_container.py` & `noelgram-2.0.106/noelgram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/__init__.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/bool.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/bytes.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/double.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/int.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/string.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/primitives/vector.py` & `noelgram-2.0.106/noelgram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/raw/core/tl_object.py` & `noelgram-2.0.106/noelgram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/__init__.py` & `noelgram-2.0.106/noelgram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/auth.py` & `noelgram-2.0.106/noelgram/session/auth.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/internals/__init__.py` & `noelgram-2.0.106/noelgram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/internals/data_center.py` & `noelgram-2.0.106/noelgram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/internals/msg_factory.py` & `noelgram-2.0.106/noelgram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/internals/msg_id.py` & `noelgram-2.0.106/noelgram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/internals/seq_no.py` & `noelgram-2.0.106/noelgram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/session/session.py` & `noelgram-2.0.106/noelgram/session/session.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/storage/__init__.py` & `noelgram-2.0.106/noelgram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/storage/file_storage.py` & `noelgram-2.0.106/noelgram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/storage/memory_storage.py` & `noelgram-2.0.106/noelgram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/storage/sqlite_storage.py` & `noelgram-2.0.106/noelgram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/storage/storage.py` & `noelgram-2.0.106/noelgram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/sync.py` & `noelgram-2.0.106/noelgram/sync.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/__init__.py` & `noelgram-2.0.106/noelgram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/authorization/__init__.py` & `noelgram-2.0.106/noelgram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/authorization/sent_code.py` & `noelgram-2.0.106/noelgram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/authorization/terms_of_service.py` & `noelgram-2.0.106/noelgram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/__init__.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_default.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/callback_game.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/callback_query.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/force_reply.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/game_high_score.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_button.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/keyboard_button.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/login_url.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_commands.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_default.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/menu_button_web_app.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/sent_web_app_message.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/bots_and_keyboards/web_app_info.py` & `noelgram-2.0.106/noelgram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/__init__.py` & `noelgram-2.0.106/noelgram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/chosen_inline_result.py` & `noelgram-2.0.106/noelgram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_animation.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_article.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_audio.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_animation.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_audio.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_document.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_photo.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_sticker.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_video.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_voice.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_contact.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_document.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_location.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_photo.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_venue.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_video.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/inline_mode/inline_query_result_voice.py` & `noelgram-2.0.106/noelgram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/__init__.py` & `noelgram-2.0.106/noelgram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media_animation.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media_audio.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media_document.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media_photo.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_media_video.py` & `noelgram-2.0.106/noelgram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_media/input_phone_contact.py` & `noelgram-2.0.106/noelgram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_message_content/__init__.py` & `noelgram-2.0.106/noelgram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_message_content/input_message_content.py` & `noelgram-2.0.106/noelgram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/input_message_content/input_text_message_content.py` & `noelgram-2.0.106/noelgram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/list.py` & `noelgram-2.0.106/noelgram/types/list.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/__init__.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/animation.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/audio.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/contact.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/dice.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/document.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/game.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/location.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/message.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/message_entity.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/message_reactions.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/photo.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/poll.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/poll_option.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/reaction.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/sticker.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/stripped_thumbnail.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/thumbnail.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/venue.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/video.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/video_note.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/voice.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/web_app_data.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/messages_and_media/web_page.py` & `noelgram-2.0.106/noelgram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/object.py` & `noelgram-2.0.106/noelgram/types/object.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/update.py` & `noelgram-2.0.106/noelgram/types/update.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/__init__.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_admin_with_invite_links.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_event.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_event_filter.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_invite_link.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_join_request.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_joiner.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_member.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_member_updated.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_permissions.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_photo.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_preview.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_privileges.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/chat_reactions.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/dialog.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/emoji_status.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/invite_link_importer.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/restriction.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/user.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_ended.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_members_invited.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_scheduled.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/types/user_and_chats/video_chat_started.py` & `noelgram-2.0.106/noelgram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram/utils.py` & `noelgram-2.0.106/noelgram/utils.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/noelgram.egg-info/PKG-INFO` & `noelgram-2.0.106/noelgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noelgram
-Version: 0.0.1
+Version: 2.0.106
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram
 Author: NOEL
 Author-email: ajual7832@gmail.com
 License: LGPLv3
 Download-URL: https://github.com/jokokendi/noelgram/releases/latest
 Project-URL: Tracker, https://github.com/jokokendi/noelgram/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noelgram Version: 0.0.1 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: noelgram Version: 2.0.106 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram Author: NOEL Author-email:
 ajual7832@gmail.com License: LGPLv3 Download-URL: https://github.com/jokokendi/
 noelgram/releases/latest Project-URL: Tracker, https://github.com/jokokendi/
 noelgram/issues Project-URL: Community, https://t.me/aruna_mutual Project-URL:
 Source, https://github.com/jokokendi/noelgram Keywords: telegram chat messenger
 mtproto api client library python Platform: UNKNOWN Classifier: Development
```

### Comparing `noelgram-0.0.1/noelgram.egg-info/SOURCES.txt` & `noelgram-2.0.106/noelgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/setup.py` & `noelgram-2.0.106/setup.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/__init__.py` & `noelgram-2.0.106/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/filters/__init__.py` & `noelgram-2.0.106/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/filters/test_command.py` & `noelgram-2.0.106/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/parser/__init__.py` & `noelgram-2.0.106/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/parser/test_html.py` & `noelgram-2.0.106/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `noelgram-0.0.1/tests/test_file_id.py` & `noelgram-2.0.106/tests/test_file_id.py`

 * *Files identical despite different names*

