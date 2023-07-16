# Comparing `tmp/noelgram1-0.0.1.tar.gz` & `tmp/noelgram1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noelgram1-0.0.1.tar", last modified: Sun Jul 16 05:50:46 2023, max compression
+gzip compressed data, was "noelgram1-0.0.2.tar", last modified: Sun Jul 16 07:01:35 2023, max compression
```

## Comparing `noelgram1-0.0.1.tar` & `noelgram1-0.0.2.tar`

### file list

```diff
@@ -1,493 +1,495 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.847521 noelgram1-0.0.1/
--rw-rw-rw-   0        0        0    35821 2023-07-16 05:27:30.000000 noelgram1-0.0.1/COPYING
--rw-rw-rw-   0        0        0     7815 2023-07-16 05:27:30.000000 noelgram1-0.0.1/COPYING.lesser
--rw-rw-rw-   0        0        0      316 2023-07-16 05:27:30.000000 noelgram1-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      790 2023-07-16 05:27:30.000000 noelgram1-0.0.1/NOTICE
--rw-rw-rw-   0        0        0     4472 2023-07-16 05:50:46.846522 noelgram1-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2023-07-16 05:27:30.000000 noelgram1-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.707713 noelgram1-0.0.1/compiler/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.712712 noelgram1-0.0.1/compiler/api/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/__init__.py
--rw-rw-rw-   0        0        0    23054 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/compiler.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.719709 noelgram1-0.0.1/compiler/api/source/
--rw-rw-rw-   0        0        0     2273 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/source/auth_key.tl
--rw-rw-rw-   0        0        0   170923 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/source/main_api.tl
--rw-rw-rw-   0        0        0     3501 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/source/sys_msgs.tl
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.724703 noelgram1-0.0.1/compiler/api/template/
--rw-rw-rw-   0        0        0      778 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/template/combinator.txt
--rw-rw-rw-   0        0        0      658 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/api/template/type.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.728704 noelgram1-0.0.1/compiler/docs/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/docs/__init__.py
--rw-rw-rw-   0        0        0    19895 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/docs/compiler.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.734697 noelgram1-0.0.1/compiler/docs/template/
--rw-rw-rw-   0        0        0       78 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/docs/template/page.txt
--rw-rw-rw-   0        0        0       99 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/docs/template/toctree.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.741693 noelgram1-0.0.1/compiler/errors/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/__init__.py
--rw-rw-rw-   0        0        0     5059 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/compiler.py
--rw-rw-rw-   0        0        0     1298 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/sort.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.759682 noelgram1-0.0.1/compiler/errors/source/
--rw-rw-rw-   0        0        0      475 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/303_SEE_OTHER.tsv
--rw-rw-rw-   0        0        0    23001 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-rw-rw-   0        0        0      687 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-rw-rw-   0        0        0     2027 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv
--rw-rw-rw-   0        0        0     1189 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-rw-rw-   0        0        0      475 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/420_FLOOD.tsv
--rw-rw-rw-   0        0        0     4263 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-rw-rw-   0        0        0      157 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.764679 noelgram1-0.0.1/compiler/errors/template/
--rw-rw-rw-   0        0        0      190 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/template/class.txt
--rw-rw-rw-   0        0        0      127 2023-07-16 05:27:30.000000 noelgram1-0.0.1/compiler/errors/template/sub_class.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.787665 noelgram1-0.0.1/noelgram/
--rw-rw-rw-   0        0        0     1441 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/__init__.py
--rw-rw-rw-   0        0        0    43024 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/client.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.844638 noelgram1-0.0.1/noelgram/connection/
--rw-rw-rw-   0        0        0      873 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/__init__.py
--rw-rw-rw-   0        0        0     2614 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/connection.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.846629 noelgram1-0.0.1/noelgram/connection/transport/
--rw-rw-rw-   0        0        0      857 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.863618 noelgram1-0.0.1/noelgram/connection/transport/tcp/
--rw-rw-rw-   0        0        0     1068 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/__init__.py
--rw-rw-rw-   0        0        0     4212 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp.py
--rw-rw-rw-   0        0        0     1825 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_abridged.py
--rw-rw-rw-   0        0        0     2916 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_abridged_o.py
--rw-rw-rw-   0        0        0     1970 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_full.py
--rw-rw-rw-   0        0        0     1556 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate.py
--rw-rw-rw-   0        0        0     2532 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate_o.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.874612 noelgram1-0.0.1/noelgram/crypto/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/crypto/__init__.py
--rw-rw-rw-   0        0        0     4143 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/crypto/aes.py
--rw-rw-rw-   0        0        0     4118 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/crypto/mtproto.py
--rw-rw-rw-   0        0        0     2528 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/crypto/prime.py
--rw-rw-rw-   0        0        0    13696 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/crypto/rsa.py
--rw-rw-rw-   0        0        0    10313 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/dispatcher.py
--rw-rw-rw-   0        0        0   212040 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/emoji.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.911587 noelgram1-0.0.1/noelgram/enums/
--rw-rw-rw-   0        0        0     1785 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/auto_name.py
--rw-rw-rw-   0        0        0     2379 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/chat_action.py
--rw-rw-rw-   0        0        0     4330 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/chat_event_action.py
--rw-rw-rw-   0        0        0     1308 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/chat_member_status.py
--rw-rw-rw-   0        0        0     1488 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/chat_members_filter.py
--rw-rw-rw-   0        0        0     1278 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/chat_type.py
--rw-rw-rw-   0        0        0     2548 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/message_entity_type.py
--rw-rw-rw-   0        0        0     1669 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/message_media_type.py
--rw-rw-rw-   0        0        0     1973 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/message_service_type.py
--rw-rw-rw-   0        0        0     2481 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/messages_filter.py
--rw-rw-rw-   0        0        0     1560 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/next_code_type.py
--rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/parse_mode.py
--rw-rw-rw-   0        0        0     1078 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/poll_type.py
--rw-rw-rw-   0        0        0     1768 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/sent_code_type.py
--rw-rw-rw-   0        0        0     1342 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/enums/user_status.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.915585 noelgram1-0.0.1/noelgram/errors/
--rw-rw-rw-   0        0        0     2670 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/errors/__init__.py
--rw-rw-rw-   0        0        0     3418 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/errors/rpc_error.py
--rw-rw-rw-   0        0        0    15635 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/file_id.py
--rw-rw-rw-   0        0        0    25765 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.949564 noelgram1-0.0.1/noelgram/handlers/
--rw-rw-rw-   0        0        0     1505 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/__init__.py
--rw-rw-rw-   0        0        0     2075 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0     2060 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/chat_join_request_handler.py
--rw-rw-rw-   0        0        0     2095 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/chat_member_updated_handler.py
--rw-rw-rw-   0        0        0     2151 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/chosen_inline_result_handler.py
--rw-rw-rw-   0        0        0     2604 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/deleted_messages_handler.py
--rw-rw-rw-   0        0        0     1745 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/disconnect_handler.py
--rw-rw-rw-   0        0        0     2028 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/edited_message_handler.py
--rw-rw-rw-   0        0        0     1593 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/handler.py
--rw-rw-rw-   0        0        0     2033 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0     1984 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/message_handler.py
--rw-rw-rw-   0        0        0     1964 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/poll_handler.py
--rw-rw-rw-   0        0        0     3009 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/raw_update_handler.py
--rw-rw-rw-   0        0        0     2036 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/handlers/user_status_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.951562 noelgram1-0.0.1/noelgram/methods/
--rw-rw-rw-   0        0        0     1365 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.961557 noelgram1-0.0.1/noelgram/methods/advanced/
--rw-rw-rw-   0        0        0     1017 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/advanced/invoke.py
--rw-rw-rw-   0        0        0     4685 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/advanced/resolve_peer.py
--rw-rw-rw-   0        0        0     8647 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/advanced/save_file.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.997534 noelgram1-0.0.1/noelgram/methods/auth/
--rw-rw-rw-   0        0        0     1708 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     1512 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/accept_terms_of_service.py
--rw-rw-rw-   0        0        0     2002 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/check_password.py
--rw-rw-rw-   0        0        0     1800 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/connect.py
--rw-rw-rw-   0        0        0     1544 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/disconnect.py
--rw-rw-rw-   0        0        0     1345 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/get_password_hint.py
--rw-rw-rw-   0        0        0     1814 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/initialize.py
--rw-rw-rw-   0        0        0     1677 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/log_out.py
--rw-rw-rw-   0        0        0     1888 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/recover_password.py
--rw-rw-rw-   0        0        0     2214 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/resend_code.py
--rw-rw-rw-   0        0        0     2865 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/send_code.py
--rw-rw-rw-   0        0        0     1516 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/send_recovery_code.py
--rw-rw-rw-   0        0        0     3165 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/sign_in.py
--rw-rw-rw-   0        0        0     2802 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/sign_in_bot.py
--rw-rw-rw-   0        0        0     2428 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/sign_up.py
--rw-rw-rw-   0        0        0     2103 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/auth/terminate.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.042020 noelgram1-0.0.1/noelgram/methods/bots/
--rw-rw-rw-   0        0        0     2096 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/answer_callback_query.py
--rw-rw-rw-   0        0        0     5102 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/answer_inline_query.py
--rw-rw-rw-   0        0        0     2042 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/answer_web_app_query.py
--rw-rw-rw-   0        0        0     2422 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/delete_bot_commands.py
--rw-rw-rw-   0        0        0     2640 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/get_bot_commands.py
--rw-rw-rw-   0        0        0     2110 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/get_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2385 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/get_chat_menu_button.py
--rw-rw-rw-   0        0        0     2870 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/get_game_high_scores.py
--rw-rw-rw-   0        0        0     3457 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/get_inline_bot_results.py
--rw-rw-rw-   0        0        0     2924 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/request_callback_answer.py
--rw-rw-rw-   0        0        0     4056 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/send_game.py
--rw-rw-rw-   0        0        0     2901 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/send_inline_bot_result.py
--rw-rw-rw-   0        0        0     2783 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/set_bot_commands.py
--rw-rw-rw-   0        0        0     3267 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/set_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2104 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/set_chat_menu_button.py
--rw-rw-rw-   0        0        0     4046 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/bots/set_game_score.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.136961 noelgram1-0.0.1/noelgram/methods/chats/
--rw-rw-rw-   0        0        0     3540 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/__init__.py
--rw-rw-rw-   0        0        0     3454 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/add_chat_members.py
--rw-rw-rw-   0        0        0     2287 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/archive_chats.py
--rw-rw-rw-   0        0        0     4731 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/ban_chat_member.py
--rw-rw-rw-   0        0        0     1873 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/create_channel.py
--rw-rw-rw-   0        0        0     2348 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/create_group.py
--rw-rw-rw-   0        0        0     2015 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/create_supergroup.py
--rw-rw-rw-   0        0        0     1637 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/delete_channel.py
--rw-rw-rw-   0        0        0     2377 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/delete_chat_photo.py
--rw-rw-rw-   0        0        0     1655 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/delete_supergroup.py
--rw-rw-rw-   0        0        0     2024 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/delete_user_history.py
--rw-rw-rw-   0        0        0     3369 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat.py
--rw-rw-rw-   0        0        0     4141 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat_event_log.py
--rw-rw-rw-   0        0        0     3430 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat_member.py
--rw-rw-rw-   0        0        0     5440 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat_members.py
--rw-rw-rw-   0        0        0     2333 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat_members_count.py
--rw-rw-rw-   0        0        0     1774 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_chat_online_count.py
--rw-rw-rw-   0        0        0     3464 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_dialogs.py
--rw-rw-rw-   0        0        0     2159 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_dialogs_count.py
--rw-rw-rw-   0        0        0     2479 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_nearby_chats.py
--rw-rw-rw-   0        0        0     2201 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/get_send_as_chats.py
--rw-rw-rw-   0        0        0     2768 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/join_chat.py
--rw-rw-rw-   0        0        0     2682 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/leave_chat.py
--rw-rw-rw-   0        0        0     1575 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/mark_chat_unread.py
--rw-rw-rw-   0        0        0     3238 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/pin_chat_message.py
--rw-rw-rw-   0        0        0     3962 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/promote_chat_member.py
--rw-rw-rw-   0        0        0     4411 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/restrict_chat_member.py
--rw-rw-rw-   0        0        0     3221 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_administrator_title.py
--rw-rw-rw-   0        0        0     2313 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_description.py
--rw-rw-rw-   0        0        0     3502 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_permissions.py
--rw-rw-rw-   0        0        0     4722 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_photo.py
--rw-rw-rw-   0        0        0     1780 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_protected_content.py
--rw-rw-rw-   0        0        0     2650 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_title.py
--rw-rw-rw-   0        0        0     2364 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_chat_username.py
--rw-rw-rw-   0        0        0     2039 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_send_as_chat.py
--rw-rw-rw-   0        0        0     2146 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/set_slow_mode.py
--rw-rw-rw-   0        0        0     2301 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/unarchive_chats.py
--rw-rw-rw-   0        0        0     2369 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/unban_chat_member.py
--rw-rw-rw-   0        0        0     1995 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/unpin_all_chat_messages.py
--rw-rw-rw-   0        0        0     2200 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/chats/unpin_chat_message.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.150953 noelgram1-0.0.1/noelgram/methods/contacts/
--rw-rw-rw-   0        0        0     1187 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     2644 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/add_contact.py
--rw-rw-rw-   0        0        0     2514 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/delete_contacts.py
--rw-rw-rw-   0        0        0     1652 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0     1463 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/get_contacts_count.py
--rw-rw-rw-   0        0        0     1992 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/contacts/import_contacts.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.181933 noelgram1-0.0.1/noelgram/methods/decorators/
--rw-rw-rw-   0        0        0     1671 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0     2229 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_chat_join_request.py
--rw-rw-rw-   0        0        0     2250 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_chat_member_updated.py
--rw-rw-rw-   0        0        0     2278 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_chosen_inline_result.py
--rw-rw-rw-   0        0        0     2244 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_deleted_messages.py
--rw-rw-rw-   0        0        0     1596 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_disconnect.py
--rw-rw-rw-   0        0        0     2233 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_edited_message.py
--rw-rw-rw-   0        0        0     2228 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0     2199 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_message.py
--rw-rw-rw-   0        0        0     2181 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_poll.py
--rw-rw-rw-   0        0        0     1873 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_raw_update.py
--rw-rw-rw-   0        0        0     2213 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/decorators/on_user_status.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.226905 noelgram1-0.0.1/noelgram/methods/invite_links/
--rw-rw-rw-   0        0        0     2493 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/approve_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1981 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/approve_chat_join_request.py
--rw-rw-rw-   0        0        0     3456 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/create_chat_invite_link.py
--rw-rw-rw-   0        0        0     1950 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/decline_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1982 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/decline_chat_join_request.py
--rw-rw-rw-   0        0        0     2085 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     1803 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/delete_chat_invite_link.py
--rw-rw-rw-   0        0        0     3625 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/edit_chat_invite_link.py
--rw-rw-rw-   0        0        0     2647 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/export_chat_invite_link.py
--rw-rw-rw-   0        0        0     3666 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-rw-rw-   0        0        0     2053 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-rw-rw-   0        0        0     1981 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link.py
--rw-rw-rw-   0        0        0     3015 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-rw-rw-   0        0        0     1985 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-rw-rw-   0        0        0     3035 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_join_requests.py
--rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/invite_links/revoke_chat_invite_link.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.365820 noelgram1-0.0.1/noelgram/methods/messages/
--rw-rw-rw-   0        0        0     4040 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     6103 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/copy_media_group.py
--rw-rw-rw-   0        0        0     5300 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/copy_message.py
--rw-rw-rw-   0        0        0     3232 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     7717 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/download_media.py
--rw-rw-rw-   0        0        0     2336 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_inline_caption.py
--rw-rw-rw-   0        0        0    10619 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_inline_media.py
--rw-rw-rw-   0        0        0     2533 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_inline_reply_markup.py
--rw-rw-rw-   0        0        0     3203 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_inline_text.py
--rw-rw-rw-   0        0        0     3054 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_message_caption.py
--rw-rw-rw-   0        0        0    13309 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_message_media.py
--rw-rw-rw-   0        0        0     3053 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_message_reply_markup.py
--rw-rw-rw-   0        0        0     4004 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0     4674 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     4162 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_chat_history.py
--rw-rw-rw-   0        0        0     2461 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_chat_history_count.py
--rw-rw-rw-   0        0        0     2035 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_custom_emoji_stickers.py
--rw-rw-rw-   0        0        0     2294 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_discussion_message.py
--rw-rw-rw-   0        0        0     2894 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_discussion_replies.py
--rw-rw-rw-   0        0        0     2012 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_discussion_replies_count.py
--rw-rw-rw-   0        0        0     3019 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_media_group.py
--rw-rw-rw-   0        0        0     4860 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/get_messages.py
--rw-rw-rw-   0        0        0     2239 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/inline_session.py
--rw-rw-rw-   0        0        0     2600 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/read_chat_history.py
--rw-rw-rw-   0        0        0     2185 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/retract_vote.py
--rw-rw-rw-   0        0        0     4277 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/search_global.py
--rw-rw-rw-   0        0        0     2218 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/search_global_count.py
--rw-rw-rw-   0        0        0     5500 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/search_messages.py
--rw-rw-rw-   0        0        0     3287 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/search_messages_count.py
--rw-rw-rw-   0        0        0    12855 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_animation.py
--rw-rw-rw-   0        0        0    11360 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_audio.py
--rw-rw-rw-   0        0        0     5603 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_cached_media.py
--rw-rw-rw-   0        0        0     2897 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_chat_action.py
--rw-rw-rw-   0        0        0     4988 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_contact.py
--rw-rw-rw-   0        0        0     4957 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_dice.py
--rw-rw-rw-   0        0        0    10688 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     4689 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_location.py
--rw-rw-rw-   0        0        0    20323 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_media_group.py
--rw-rw-rw-   0        0        0     7442 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     9642 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     8252 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_poll.py
--rw-rw-rw-   0        0        0     2434 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_reaction.py
--rw-rw-rw-   0        0        0     8517 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     5534 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_venue.py
--rw-rw-rw-   0        0        0    12215 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     9515 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_video_note.py
--rw-rw-rw-   0        0        0     9632 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2896 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/stop_poll.py
--rw-rw-rw-   0        0        0     4043 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/stream_media.py
--rw-rw-rw-   0        0        0     2573 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/messages/vote_poll.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.379811 noelgram1-0.0.1/noelgram/methods/password/
--rw-rw-rw-   0        0        0     1117 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/password/__init__.py
--rw-rw-rw-   0        0        0     2879 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/password/change_cloud_password.py
--rw-rw-rw-   0        0        0     3094 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/password/enable_cloud_password.py
--rw-rw-rw-   0        0        0     2207 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/password/remove_cloud_password.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.412790 noelgram1-0.0.1/noelgram/methods/users/
--rw-rw-rw-   0        0        0     1708 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/__init__.py
--rw-rw-rw-   0        0        0     1825 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/block_user.py
--rw-rw-rw-   0        0        0     2300 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/delete_profile_photos.py
--rw-rw-rw-   0        0        0     4556 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_chat_photos.py
--rw-rw-rw-   0        0        0     2583 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_chat_photos_count.py
--rw-rw-rw-   0        0        0     2426 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_common_chats.py
--rw-rw-rw-   0        0        0     1711 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_default_emoji_statuses.py
--rw-rw-rw-   0        0        0     1614 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_me.py
--rw-rw-rw-   0        0        0     2633 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/get_users.py
--rw-rw-rw-   0        0        0     1940 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/set_emoji_status.py
--rw-rw-rw-   0        0        0     2793 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/set_profile_photo.py
--rw-rw-rw-   0        0        0     1933 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/set_username.py
--rw-rw-rw-   0        0        0     1835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/unblock_user.py
--rw-rw-rw-   0        0        0     2448 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/users/update_profile.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.439774 noelgram1-0.0.1/noelgram/methods/utilities/
--rw-rw-rw-   0        0        0     1292 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0     2310 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/compose.py
--rw-rw-rw-   0        0        0     1597 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/export_session_string.py
--rw-rw-rw-   0        0        0     2837 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/idle.py
--rw-rw-rw-   0        0        0     2273 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0     2366 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/restart.py
--rw-rw-rw-   0        0        0     2943 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/run.py
--rw-rw-rw-   0        0        0     2440 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/start.py
--rw-rw-rw-   0        0        0     2186 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/stop.py
--rw-rw-rw-   0        0        0     1753 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/methods/utilities/stop_transmission.py
--rw-rw-rw-   0        0        0    63796 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/mime_types.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.451767 noelgram1-0.0.1/noelgram/parser/
--rw-rw-rw-   0        0        0      865 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/parser/__init__.py
--rw-rw-rw-   0        0        0     8927 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/parser/html.py
--rw-rw-rw-   0        0        0     5943 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/parser/markdown.py
--rw-rw-rw-   0        0        0     2138 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/parser/parser.py
--rw-rw-rw-   0        0        0     1586 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/parser/utils.py
--rw-rw-rw-   0        0        0        0 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.454764 noelgram1-0.0.1/noelgram/raw/
--rw-rw-rw-   0        0        0     1066 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.472753 noelgram1-0.0.1/noelgram/raw/core/
--rw-rw-rw-   0        0        0     1343 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/__init__.py
--rw-rw-rw-   0        0        0     1745 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/future_salt.py
--rw-rw-rw-   0        0        0     1954 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/future_salts.py
--rw-rw-rw-   0        0        0     1876 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/gzip_packed.py
--rw-rw-rw-   0        0        0     1074 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/list.py
--rw-rw-rw-   0        0        0     1907 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/message.py
--rw-rw-rw-   0        0        0     1667 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/msg_container.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.492741 noelgram1-0.0.1/noelgram/raw/core/primitives/
--rw-rw-rw-   0        0        0     1036 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/bool.py
--rw-rw-rw-   0        0        0     1814 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/bytes.py
--rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/double.py
--rw-rw-rw-   0        0        0     1403 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/int.py
--rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/string.py
--rw-rw-rw-   0        0        0     2081 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/primitives/vector.py
--rw-rw-rw-   0        0        0     2577 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/raw/core/tl_object.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.499737 noelgram1-0.0.1/noelgram/session/
--rw-rw-rw-   0        0        0      891 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/__init__.py
--rw-rw-rw-   0        0        0    11727 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/auth.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.511730 noelgram1-0.0.1/noelgram/session/internals/
--rw-rw-rw-   0        0        0      938 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/internals/__init__.py
--rw-rw-rw-   0        0        0     2535 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/internals/data_center.py
--rw-rw-rw-   0        0        0     1412 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/internals/msg_factory.py
--rw-rw-rw-   0        0        0     1191 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/internals/msg_id.py
--rw-rw-rw-   0        0        0     1192 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/internals/seq_no.py
--rw-rw-rw-   0        0        0    13831 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/session/session.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.522722 noelgram1-0.0.1/noelgram/storage/
--rw-rw-rw-   0        0        0      949 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/storage/__init__.py
--rw-rw-rw-   0        0        0     2028 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/storage/file_storage.py
--rw-rw-rw-   0        0        0     2823 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/storage/memory_storage.py
--rw-rw-rw-   0        0        0     6446 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/storage/sqlite_storage.py
--rw-rw-rw-   0        0        0     2872 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/storage/storage.py
--rw-rw-rw-   0        0        0     3852 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/sync.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.532717 noelgram1-0.0.1/noelgram/types/
--rw-rw-rw-   0        0        0     1137 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.539712 noelgram1-0.0.1/noelgram/types/authorization/
--rw-rw-rw-   0        0        0      960 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/authorization/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/authorization/sent_code.py
--rw-rw-rw-   0        0        0     1986 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/authorization/terms_of_service.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.612666 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/
--rw-rw-rw-   0        0        0     2901 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command.py
--rw-rw-rw-   0        0        0     2861 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope.py
--rw-rw-rw-   0        0        0     1325 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-rw-rw-   0        0        0     1290 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-rw-rw-   0        0        0     1281 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-rw-rw-   0        0        0     1605 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-rw-rw-   0        0        0     1682 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-rw-rw-   0        0        0     1865 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-rw-rw-   0        0        0     1341 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-rw-rw-   0        0        0     1058 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/callback_game.py
--rw-rw-rw-   0        0        0    13110 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/callback_query.py
--rw-rw-rw-   0        0        0     2449 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/force_reply.py
--rw-rw-rw-   0        0        0     2286 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/game_high_score.py
--rw-rw-rw-   0        0        0     8328 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-rw-rw-   0        0        0     2536 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-rw-rw-   0        0        0     3609 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/keyboard_button.py
--rw-rw-rw-   0        0        0     3802 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/login_url.py
--rw-rw-rw-   0        0        0     1647 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button.py
--rw-rw-rw-   0        0        0     1241 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_commands.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_default.py
--rw-rw-rw-   0        0        0     1860 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_web_app.py
--rw-rw-rw-   0        0        0     4687 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-rw-rw-   0        0        0     1606 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/sent_web_app_message.py
--rw-rw-rw-   0        0        0     1350 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/bots_and_keyboards/web_app_info.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.671631 noelgram1-0.0.1/noelgram/types/inline_mode/
--rw-rw-rw-   0        0        0     2802 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/__init__.py
--rw-rw-rw-   0        0        0     3761 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/chosen_inline_result.py
--rw-rw-rw-   0        0        0     7479 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query.py
--rw-rw-rw-   0        0        0     2474 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result.py
--rw-rw-rw-   0        0        0     5931 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_animation.py
--rw-rw-rw-   0        0        0     3403 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_article.py
--rw-rw-rw-   0        0        0     4625 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_audio.py
--rw-rw-rw-   0        0        0     4353 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_animation.py
--rw-rw-rw-   0        0        0     4130 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_audio.py
--rw-rw-rw-   0        0        0     4501 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_document.py
--rw-rw-rw-   0        0        0     4423 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_photo.py
--rw-rw-rw-   0        0        0     3109 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-rw-rw-   0        0        0     4508 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_video.py
--rw-rw-rw-   0        0        0     4310 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_voice.py
--rw-rw-rw-   0        0        0     4246 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_contact.py
--rw-rw-rw-   0        0        0     5385 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_document.py
--rw-rw-rw-   0        0        0     4741 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_location.py
--rw-rw-rw-   0        0        0     5408 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     4885 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_venue.py
--rw-rw-rw-   0        0        0     5625 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_video.py
--rw-rw-rw-   0        0        0     4474 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_voice.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.690619 noelgram1-0.0.1/noelgram/types/input_media/
--rw-rw-rw-   0        0        0     1344 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media.py
--rw-rw-rw-   0        0        0     3513 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media_animation.py
--rw-rw-rw-   0        0        0     3364 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media_audio.py
--rw-rw-rw-   0        0        0     2836 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media_document.py
--rw-rw-rw-   0        0        0     2748 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media_photo.py
--rw-rw-rw-   0        0        0     3711 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_media_video.py
--rw-rw-rw-   0        0        0     1788 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_media/input_phone_contact.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.697614 noelgram1-0.0.1/noelgram/types/input_message_content/
--rw-rw-rw-   0        0        0     1030 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_message_content/__init__.py
--rw-rw-rw-   0        0        0     1453 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_message_content/input_message_content.py
--rw-rw-rw-   0        0        0     2706 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/input_message_content/input_text_message_content.py
--rw-rw-rw-   0        0        0     1123 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/list.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.754578 noelgram1-0.0.1/noelgram/types/messages_and_media/
--rw-rw-rw-   0        0        0     1883 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/__init__.py
--rw-rw-rw-   0        0        0     4165 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/animation.py
--rw-rw-rw-   0        0        0     4190 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/audio.py
--rw-rw-rw-   0        0        0     2278 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/contact.py
--rw-rw-rw-   0        0        0     1634 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/dice.py
--rw-rw-rw-   0        0        0     3507 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/document.py
--rw-rw-rw-   0        0        0     3143 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/game.py
--rw-rw-rw-   0        0        0     1715 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/location.py
--rw-rw-rw-   0        0        0   148109 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/message.py
--rw-rw-rw-   0        0        0     4476 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/message_entity.py
--rw-rw-rw-   0        0        0     1856 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/message_reactions.py
--rw-rw-rw-   0        0        0     4439 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/photo.py
--rw-rw-rw-   0        0        0     7240 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/poll.py
--rw-rw-rw-   0        0        0     1582 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/poll_option.py
--rw-rw-rw-   0        0        0     2703 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/reaction.py
--rw-rw-rw-   0        0        0     7115 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/sticker.py
--rw-rw-rw-   0        0        0     1478 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/stripped_thumbnail.py
--rw-rw-rw-   0        0        0     3866 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/thumbnail.py
--rw-rw-rw-   0        0        0     2365 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/venue.py
--rw-rw-rw-   0        0        0     4523 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/video.py
--rw-rw-rw-   0        0        0     3709 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/video_note.py
--rw-rw-rw-   0        0        0     3300 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/voice.py
--rw-rw-rw-   0        0        0     1616 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/web_app_data.py
--rw-rw-rw-   0        0        0     6538 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/messages_and_media/web_page.py
--rw-rw-rw-   0        0        0     3983 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/object.py
--rw-rw-rw-   0        0        0     1029 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/update.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.817540 noelgram1-0.0.1/noelgram/types/user_and_chats/
--rw-rw-rw-   0        0        0     2364 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/__init__.py
--rw-rw-rw-   0        0        0    33522 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat.py
--rw-rw-rw-   0        0        0     2299 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-rw-rw-   0        0        0    20324 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_event.py
--rw-rw-rw-   0        0        0     5689 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_event_filter.py
--rw-rw-rw-   0        0        0     4709 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_invite_link.py
--rw-rw-rw-   0        0        0     4384 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_join_request.py
--rw-rw-rw-   0        0        0     2646 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_joiner.py
--rw-rw-rw-   0        0        0     9671 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_member.py
--rw-rw-rw-   0        0        0     3776 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_member_updated.py
--rw-rw-rw-   0        0        0     4480 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_permissions.py
--rw-rw-rw-   0        0        0     4074 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_photo.py
--rw-rw-rw-   0        0        0     2671 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_preview.py
--rw-rw-rw-   0        0        0     5063 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_privileges.py
--rw-rw-rw-   0        0        0     2425 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/chat_reactions.py
--rw-rw-rw-   0        0        0     2761 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/dialog.py
--rw-rw-rw-   0        0        0     2499 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/emoji_status.py
--rw-rw-rw-   0        0        0     2012 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/invite_link_importer.py
--rw-rw-rw-   0        0        0     1713 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/restriction.py
--rw-rw-rw-   0        0        0    13235 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/user.py
--rw-rw-rw-   0        0        0     1387 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_ended.py
--rw-rw-rw-   0        0        0     1660 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_members_invited.py
--rw-rw-rw-   0        0        0     1574 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_scheduled.py
--rw-rw-rw-   0        0        0     1072 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_started.py
--rw-rw-rw-   0        0        0    10943 2023-07-16 05:27:30.000000 noelgram1-0.0.1/noelgram/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:45.839634 noelgram1-0.0.1/noelgram1.egg-info/
--rw-rw-rw-   0        0        0     4472 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18796 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 05:50:45.000000 noelgram1-0.0.1/noelgram1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2023-07-16 05:27:30.000000 noelgram1-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 05:50:46.848521 noelgram1-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3599 2023-07-16 05:50:30.000000 noelgram1-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.822536 noelgram1-0.0.1/tests/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.827534 noelgram1-0.0.1/tests/filters/
--rw-rw-rw-   0        0        0     1237 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/filters/__init__.py
--rw-rw-rw-   0        0        0     3520 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/filters/test_command.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:50:46.842524 noelgram1-0.0.1/tests/parser/
--rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/parser/__init__.py
--rw-rw-rw-   0        0        0     6411 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/parser/test_html.py
--rw-rw-rw-   0        0        0     8402 2023-07-16 05:27:30.000000 noelgram1-0.0.1/tests/test_file_id.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:35.075373 noelgram1-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-07-16 05:27:30.000000 noelgram1-0.0.2/COPYING
+-rw-rw-rw-   0        0        0     7815 2023-07-16 05:27:30.000000 noelgram1-0.0.2/COPYING.lesser
+-rw-rw-rw-   0        0        0      316 2023-07-16 05:27:30.000000 noelgram1-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      790 2023-07-16 05:27:30.000000 noelgram1-0.0.2/NOTICE
+-rw-rw-rw-   0        0        0     4472 2023-07-16 07:01:35.073376 noelgram1-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2547 2023-07-16 07:00:57.000000 noelgram1-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:31.891891 noelgram1-0.0.2/compiler/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:31.911879 noelgram1-0.0.2/compiler/api/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/__init__.py
+-rw-rw-rw-   0        0        0    23054 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/compiler.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:31.973840 noelgram1-0.0.2/compiler/api/source/
+-rw-rw-rw-   0        0        0     2273 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/source/auth_key.tl
+-rw-rw-rw-   0        0        0   170923 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/source/main_api.tl
+-rw-rw-rw-   0        0        0     3501 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/source/sys_msgs.tl
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:31.989831 noelgram1-0.0.2/compiler/api/template/
+-rw-rw-rw-   0        0        0      778 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/template/combinator.txt
+-rw-rw-rw-   0        0        0      658 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/api/template/type.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.009817 noelgram1-0.0.2/compiler/docs/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/docs/__init__.py
+-rw-rw-rw-   0        0        0    19895 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/docs/compiler.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.030804 noelgram1-0.0.2/compiler/docs/template/
+-rw-rw-rw-   0        0        0       78 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/docs/template/page.txt
+-rw-rw-rw-   0        0        0       99 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/docs/template/toctree.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.065782 noelgram1-0.0.2/compiler/errors/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/__init__.py
+-rw-rw-rw-   0        0        0     5059 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/compiler.py
+-rw-rw-rw-   0        0        0     1298 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/sort.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.104760 noelgram1-0.0.2/compiler/errors/source/
+-rw-rw-rw-   0        0        0      475 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-rw-rw-   0        0        0    23001 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-rw-rw-   0        0        0      687 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-rw-rw-   0        0        0     2027 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-rw-rw-   0        0        0     1189 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-rw-rw-   0        0        0      475 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/420_FLOOD.tsv
+-rw-rw-rw-   0        0        0     4263 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-rw-rw-   0        0        0      157 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.111756 noelgram1-0.0.2/compiler/errors/template/
+-rw-rw-rw-   0        0        0      190 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/template/class.txt
+-rw-rw-rw-   0        0        0      127 2023-07-16 05:27:30.000000 noelgram1-0.0.2/compiler/errors/template/sub_class.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.240674 noelgram1-0.0.2/noelgram/
+-rw-rw-rw-   0        0        0     1441 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/__init__.py
+-rw-rw-rw-   0        0        0    43024 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/client.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.310632 noelgram1-0.0.2/noelgram/connection/
+-rw-rw-rw-   0        0        0      873 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/__init__.py
+-rw-rw-rw-   0        0        0     2614 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/connection.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.314635 noelgram1-0.0.2/noelgram/connection/transport/
+-rw-rw-rw-   0        0        0      857 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.358601 noelgram1-0.0.2/noelgram/connection/transport/tcp/
+-rw-rw-rw-   0        0        0     1068 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/__init__.py
+-rw-rw-rw-   0        0        0     4212 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp.py
+-rw-rw-rw-   0        0        0     1825 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_abridged.py
+-rw-rw-rw-   0        0        0     2916 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_abridged_o.py
+-rw-rw-rw-   0        0        0     1970 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_full.py
+-rw-rw-rw-   0        0        0     1556 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_intermediate.py
+-rw-rw-rw-   0        0        0     2532 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_intermediate_o.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.393580 noelgram1-0.0.2/noelgram/crypto/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4143 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/crypto/aes.py
+-rw-rw-rw-   0        0        0     4118 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/crypto/mtproto.py
+-rw-rw-rw-   0        0        0     2528 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/crypto/prime.py
+-rw-rw-rw-   0        0        0    13696 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/crypto/rsa.py
+-rw-rw-rw-   0        0        0    10313 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/dispatcher.py
+-rw-rw-rw-   0        0        0   212040 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/emoji.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.539690 noelgram1-0.0.2/noelgram/enums/
+-rw-rw-rw-   0        0        0     1785 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/__init__.py
+-rw-rw-rw-   0        0        0     1029 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/auto_name.py
+-rw-rw-rw-   0        0        0     2379 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/chat_action.py
+-rw-rw-rw-   0        0        0     4330 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/chat_event_action.py
+-rw-rw-rw-   0        0        0     1308 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/chat_member_status.py
+-rw-rw-rw-   0        0        0     1488 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/chat_members_filter.py
+-rw-rw-rw-   0        0        0     1278 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/chat_type.py
+-rw-rw-rw-   0        0        0     2548 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/message_entity_type.py
+-rw-rw-rw-   0        0        0     1669 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/message_media_type.py
+-rw-rw-rw-   0        0        0     1973 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/message_service_type.py
+-rw-rw-rw-   0        0        0     2481 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/messages_filter.py
+-rw-rw-rw-   0        0        0     1560 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/next_code_type.py
+-rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/parse_mode.py
+-rw-rw-rw-   0        0        0     1078 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1768 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/sent_code_type.py
+-rw-rw-rw-   0        0        0     1342 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/enums/user_status.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.564675 noelgram1-0.0.2/noelgram/errors/
+-rw-rw-rw-   0        0        0     2670 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/errors/__init__.py
+-rw-rw-rw-   0        0        0     3418 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/errors/rpc_error.py
+-rw-rw-rw-   0        0        0    15635 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/file_id.py
+-rw-rw-rw-   0        0        0    25765 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.649623 noelgram1-0.0.2/noelgram/handlers/
+-rw-rw-rw-   0        0        0     1505 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2075 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0     2060 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/chat_join_request_handler.py
+-rw-rw-rw-   0        0        0     2095 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/chat_member_updated_handler.py
+-rw-rw-rw-   0        0        0     2151 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/chosen_inline_result_handler.py
+-rw-rw-rw-   0        0        0     2604 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/deleted_messages_handler.py
+-rw-rw-rw-   0        0        0     1745 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/disconnect_handler.py
+-rw-rw-rw-   0        0        0     2028 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/edited_message_handler.py
+-rw-rw-rw-   0        0        0     1593 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/handler.py
+-rw-rw-rw-   0        0        0     2033 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0     1984 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/message_handler.py
+-rw-rw-rw-   0        0        0     1964 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/poll_handler.py
+-rw-rw-rw-   0        0        0     3009 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/raw_update_handler.py
+-rw-rw-rw-   0        0        0     2036 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/handlers/user_status_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.653619 noelgram1-0.0.2/noelgram/methods/
+-rw-rw-rw-   0        0        0     1365 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.679602 noelgram1-0.0.2/noelgram/methods/advanced/
+-rw-rw-rw-   0        0        0     1017 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/advanced/invoke.py
+-rw-rw-rw-   0        0        0     4685 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/advanced/resolve_peer.py
+-rw-rw-rw-   0        0        0     8647 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/advanced/save_file.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.787537 noelgram1-0.0.2/noelgram/methods/auth/
+-rw-rw-rw-   0        0        0     1708 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     1512 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/accept_terms_of_service.py
+-rw-rw-rw-   0        0        0     2002 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/check_password.py
+-rw-rw-rw-   0        0        0     1800 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/connect.py
+-rw-rw-rw-   0        0        0     1544 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/disconnect.py
+-rw-rw-rw-   0        0        0     1345 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/get_password_hint.py
+-rw-rw-rw-   0        0        0     1814 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/initialize.py
+-rw-rw-rw-   0        0        0     1677 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/log_out.py
+-rw-rw-rw-   0        0        0     1888 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/recover_password.py
+-rw-rw-rw-   0        0        0     2214 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/resend_code.py
+-rw-rw-rw-   0        0        0     2865 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0     1516 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/send_recovery_code.py
+-rw-rw-rw-   0        0        0     3165 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/sign_in.py
+-rw-rw-rw-   0        0        0     2802 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/sign_in_bot.py
+-rw-rw-rw-   0        0        0     2428 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/sign_up.py
+-rw-rw-rw-   0        0        0     2103 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/auth/terminate.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.858491 noelgram1-0.0.2/noelgram/methods/bots/
+-rw-rw-rw-   0        0        0     2096 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/answer_callback_query.py
+-rw-rw-rw-   0        0        0     5102 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/answer_inline_query.py
+-rw-rw-rw-   0        0        0     2042 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/answer_web_app_query.py
+-rw-rw-rw-   0        0        0     2422 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/delete_bot_commands.py
+-rw-rw-rw-   0        0        0     2640 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/get_bot_commands.py
+-rw-rw-rw-   0        0        0     2110 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/get_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2385 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/get_chat_menu_button.py
+-rw-rw-rw-   0        0        0     2870 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/get_game_high_scores.py
+-rw-rw-rw-   0        0        0     3457 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/get_inline_bot_results.py
+-rw-rw-rw-   0        0        0     2924 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/request_callback_answer.py
+-rw-rw-rw-   0        0        0     4056 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/send_game.py
+-rw-rw-rw-   0        0        0     2901 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/send_inline_bot_result.py
+-rw-rw-rw-   0        0        0     2783 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/set_bot_commands.py
+-rw-rw-rw-   0        0        0     3267 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/set_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2104 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/set_chat_menu_button.py
+-rw-rw-rw-   0        0        0     4046 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/bots/set_game_score.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.150314 noelgram1-0.0.2/noelgram/methods/chats/
+-rw-rw-rw-   0        0        0     3540 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0     3454 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/add_chat_members.py
+-rw-rw-rw-   0        0        0     2287 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/archive_chats.py
+-rw-rw-rw-   0        0        0     4731 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0     1873 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/create_channel.py
+-rw-rw-rw-   0        0        0     2348 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/create_group.py
+-rw-rw-rw-   0        0        0     2015 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/create_supergroup.py
+-rw-rw-rw-   0        0        0     1637 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/delete_channel.py
+-rw-rw-rw-   0        0        0     2377 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/delete_chat_photo.py
+-rw-rw-rw-   0        0        0     1655 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/delete_supergroup.py
+-rw-rw-rw-   0        0        0     2024 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/delete_user_history.py
+-rw-rw-rw-   0        0        0     3369 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0     4141 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat_event_log.py
+-rw-rw-rw-   0        0        0     3430 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat_member.py
+-rw-rw-rw-   0        0        0     5440 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat_members.py
+-rw-rw-rw-   0        0        0     2333 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat_members_count.py
+-rw-rw-rw-   0        0        0     1774 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_chat_online_count.py
+-rw-rw-rw-   0        0        0     3464 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_dialogs.py
+-rw-rw-rw-   0        0        0     2159 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_dialogs_count.py
+-rw-rw-rw-   0        0        0     2479 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_nearby_chats.py
+-rw-rw-rw-   0        0        0     2201 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/get_send_as_chats.py
+-rw-rw-rw-   0        0        0     2768 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/join_chat.py
+-rw-rw-rw-   0        0        0     2682 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0     1575 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/mark_chat_unread.py
+-rw-rw-rw-   0        0        0     3238 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/pin_chat_message.py
+-rw-rw-rw-   0        0        0     3962 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0     4411 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/restrict_chat_member.py
+-rw-rw-rw-   0        0        0     3221 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_administrator_title.py
+-rw-rw-rw-   0        0        0     2313 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_description.py
+-rw-rw-rw-   0        0        0     3502 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_permissions.py
+-rw-rw-rw-   0        0        0     4722 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0     1780 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_protected_content.py
+-rw-rw-rw-   0        0        0     2650 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_title.py
+-rw-rw-rw-   0        0        0     2364 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_chat_username.py
+-rw-rw-rw-   0        0        0     2039 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_send_as_chat.py
+-rw-rw-rw-   0        0        0     2146 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/set_slow_mode.py
+-rw-rw-rw-   0        0        0     2301 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/unarchive_chats.py
+-rw-rw-rw-   0        0        0     2369 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/unban_chat_member.py
+-rw-rw-rw-   0        0        0     1995 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/unpin_all_chat_messages.py
+-rw-rw-rw-   0        0        0     2200 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/chats/unpin_chat_message.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.182292 noelgram1-0.0.2/noelgram/methods/contacts/
+-rw-rw-rw-   0        0        0     1187 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     2644 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/add_contact.py
+-rw-rw-rw-   0        0        0     2514 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/delete_contacts.py
+-rw-rw-rw-   0        0        0     1652 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0     1463 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/get_contacts_count.py
+-rw-rw-rw-   0        0        0     1992 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/contacts/import_contacts.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.275234 noelgram1-0.0.2/noelgram/methods/decorators/
+-rw-rw-rw-   0        0        0     1671 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0     2229 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_chat_join_request.py
+-rw-rw-rw-   0        0        0     2250 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_chat_member_updated.py
+-rw-rw-rw-   0        0        0     2278 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_chosen_inline_result.py
+-rw-rw-rw-   0        0        0     2244 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_deleted_messages.py
+-rw-rw-rw-   0        0        0     1596 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_disconnect.py
+-rw-rw-rw-   0        0        0     2233 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_edited_message.py
+-rw-rw-rw-   0        0        0     2228 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0     2199 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_message.py
+-rw-rw-rw-   0        0        0     2181 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_poll.py
+-rw-rw-rw-   0        0        0     1873 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_raw_update.py
+-rw-rw-rw-   0        0        0     2213 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/decorators/on_user_status.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.361180 noelgram1-0.0.2/noelgram/methods/invite_links/
+-rw-rw-rw-   0        0        0     2493 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1981 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/approve_chat_join_request.py
+-rw-rw-rw-   0        0        0     3456 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/create_chat_invite_link.py
+-rw-rw-rw-   0        0        0     1950 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1982 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/decline_chat_join_request.py
+-rw-rw-rw-   0        0        0     2085 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     1803 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/delete_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3625 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/edit_chat_invite_link.py
+-rw-rw-rw-   0        0        0     2647 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/export_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3666 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-rw-rw-   0        0        0     2053 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-rw-rw-   0        0        0     1981 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3015 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-rw-rw-   0        0        0     1985 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-rw-rw-   0        0        0     3035 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_join_requests.py
+-rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/invite_links/revoke_chat_invite_link.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.845880 noelgram1-0.0.2/noelgram/methods/messages/
+-rw-rw-rw-   0        0        0     4193 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     6103 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/copy_media_group.py
+-rw-rw-rw-   0        0        0     5300 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0     3232 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     7717 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/download_media.py
+-rw-rw-rw-   0        0        0     2336 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_inline_caption.py
+-rw-rw-rw-   0        0        0    10619 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_inline_media.py
+-rw-rw-rw-   0        0        0     2533 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_inline_reply_markup.py
+-rw-rw-rw-   0        0        0     3203 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_inline_text.py
+-rw-rw-rw-   0        0        0     3054 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_message_caption.py
+-rw-rw-rw-   0        0        0    13309 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_message_media.py
+-rw-rw-rw-   0        0        0     3053 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_message_reply_markup.py
+-rw-rw-rw-   0        0        0     4004 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0     4674 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     4162 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_chat_history.py
+-rw-rw-rw-   0        0        0     2461 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_chat_history_count.py
+-rw-rw-rw-   0        0        0     2035 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_custom_emoji_stickers.py
+-rw-rw-rw-   0        0        0     2294 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_discussion_message.py
+-rw-rw-rw-   0        0        0     2894 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_discussion_replies.py
+-rw-rw-rw-   0        0        0     2012 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_discussion_replies_count.py
+-rw-rw-rw-   0        0        0     3019 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_media_group.py
+-rw-rw-rw-   0        0        0     4860 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/get_messages.py
+-rw-rw-rw-   0        0        0     2239 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/inline_session.py
+-rw-rw-rw-   0        0        0     2600 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/read_chat_history.py
+-rw-rw-rw-   0        0        0     2185 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/retract_vote.py
+-rw-rw-rw-   0        0        0     4277 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/search_global.py
+-rw-rw-rw-   0        0        0     2218 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/search_global_count.py
+-rw-rw-rw-   0        0        0     5500 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/search_messages.py
+-rw-rw-rw-   0        0        0     3287 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/search_messages_count.py
+-rw-rw-rw-   0        0        0    12855 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_animation.py
+-rw-rw-rw-   0        0        0    11360 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_audio.py
+-rw-rw-rw-   0        0        0     5603 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_cached_media.py
+-rw-rw-rw-   0        0        0     2897 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_chat_action.py
+-rw-rw-rw-   0        0        0     4988 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_contact.py
+-rw-rw-rw-   0        0        0     4957 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_dice.py
+-rw-rw-rw-   0        0        0    10688 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     4689 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_location.py
+-rw-rw-rw-   0        0        0    20323 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_media_group.py
+-rw-rw-rw-   0        0        0     7442 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     9642 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     8252 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_poll.py
+-rw-rw-rw-   0        0        0     2434 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_reaction.py
+-rw-rw-rw-   0        0        0     8517 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     5534 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_venue.py
+-rw-rw-rw-   0        0        0    12215 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     9515 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_video_note.py
+-rw-rw-rw-   0        0        0     9632 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2896 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/stop_poll.py
+-rw-rw-rw-   0        0        0     4043 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/stream_media.py
+-rw-rw-rw-   0        0        0     2573 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/messages/vote_poll.py
+-rw-rw-rw-   0        0        0     2901 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/methods/messages/wait_for_callback_query.py
+-rw-rw-rw-   0        0        0     2822 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/methods/messages/wait_for_message.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.872863 noelgram1-0.0.2/noelgram/methods/password/
+-rw-rw-rw-   0        0        0     1117 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/password/__init__.py
+-rw-rw-rw-   0        0        0     2879 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/password/change_cloud_password.py
+-rw-rw-rw-   0        0        0     3094 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/password/enable_cloud_password.py
+-rw-rw-rw-   0        0        0     2207 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/password/remove_cloud_password.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:33.946260 noelgram1-0.0.2/noelgram/methods/users/
+-rw-rw-rw-   0        0        0     1708 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/__init__.py
+-rw-rw-rw-   0        0        0     1825 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/block_user.py
+-rw-rw-rw-   0        0        0     2300 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/delete_profile_photos.py
+-rw-rw-rw-   0        0        0     4556 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_chat_photos.py
+-rw-rw-rw-   0        0        0     2583 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_chat_photos_count.py
+-rw-rw-rw-   0        0        0     2426 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_common_chats.py
+-rw-rw-rw-   0        0        0     1711 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_default_emoji_statuses.py
+-rw-rw-rw-   0        0        0     1614 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_me.py
+-rw-rw-rw-   0        0        0     2633 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/get_users.py
+-rw-rw-rw-   0        0        0     1940 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/set_emoji_status.py
+-rw-rw-rw-   0        0        0     2793 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/set_profile_photo.py
+-rw-rw-rw-   0        0        0     1933 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/set_username.py
+-rw-rw-rw-   0        0        0     1835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/unblock_user.py
+-rw-rw-rw-   0        0        0     2448 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/users/update_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.022268 noelgram1-0.0.2/noelgram/methods/utilities/
+-rw-rw-rw-   0        0        0     1292 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0     2310 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/compose.py
+-rw-rw-rw-   0        0        0     1597 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/export_session_string.py
+-rw-rw-rw-   0        0        0     2837 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/idle.py
+-rw-rw-rw-   0        0        0     2273 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0     2366 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/restart.py
+-rw-rw-rw-   0        0        0     2943 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     2440 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     2186 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/stop.py
+-rw-rw-rw-   0        0        0     1753 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/methods/utilities/stop_transmission.py
+-rw-rw-rw-   0        0        0    63796 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/mime_types.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.053254 noelgram1-0.0.2/noelgram/parser/
+-rw-rw-rw-   0        0        0      865 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/parser/__init__.py
+-rw-rw-rw-   0        0        0     8927 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/parser/html.py
+-rw-rw-rw-   0        0        0     5943 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/parser/markdown.py
+-rw-rw-rw-   0        0        0     2138 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/parser/parser.py
+-rw-rw-rw-   0        0        0     1586 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/parser/utils.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.057250 noelgram1-0.0.2/noelgram/raw/
+-rw-rw-rw-   0        0        0     1066 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.102223 noelgram1-0.0.2/noelgram/raw/core/
+-rw-rw-rw-   0        0        0     1343 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/__init__.py
+-rw-rw-rw-   0        0        0     1745 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/future_salt.py
+-rw-rw-rw-   0        0        0     1954 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/future_salts.py
+-rw-rw-rw-   0        0        0     1876 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/gzip_packed.py
+-rw-rw-rw-   0        0        0     1074 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/list.py
+-rw-rw-rw-   0        0        0     1907 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/message.py
+-rw-rw-rw-   0        0        0     1667 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/msg_container.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.129208 noelgram1-0.0.2/noelgram/raw/core/primitives/
+-rw-rw-rw-   0        0        0     1036 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/bool.py
+-rw-rw-rw-   0        0        0     1814 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/bytes.py
+-rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/double.py
+-rw-rw-rw-   0        0        0     1403 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/int.py
+-rw-rw-rw-   0        0        0     1225 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/string.py
+-rw-rw-rw-   0        0        0     2081 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/primitives/vector.py
+-rw-rw-rw-   0        0        0     2577 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/raw/core/tl_object.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.163185 noelgram1-0.0.2/noelgram/session/
+-rw-rw-rw-   0        0        0      891 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/__init__.py
+-rw-rw-rw-   0        0        0    11727 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/auth.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.193167 noelgram1-0.0.2/noelgram/session/internals/
+-rw-rw-rw-   0        0        0      938 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/internals/__init__.py
+-rw-rw-rw-   0        0        0     2535 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/internals/data_center.py
+-rw-rw-rw-   0        0        0     1412 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/internals/msg_factory.py
+-rw-rw-rw-   0        0        0     1191 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/internals/msg_id.py
+-rw-rw-rw-   0        0        0     1192 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/internals/seq_no.py
+-rw-rw-rw-   0        0        0    13831 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/session/session.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.243647 noelgram1-0.0.2/noelgram/storage/
+-rw-rw-rw-   0        0        0      949 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/storage/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/storage/file_storage.py
+-rw-rw-rw-   0        0        0     2823 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/storage/memory_storage.py
+-rw-rw-rw-   0        0        0     6446 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/storage/sqlite_storage.py
+-rw-rw-rw-   0        0        0     2872 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/storage/storage.py
+-rw-rw-rw-   0        0        0     3852 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/sync.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.258642 noelgram1-0.0.2/noelgram/types/
+-rw-rw-rw-   0        0        0     1137 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.270634 noelgram1-0.0.2/noelgram/types/authorization/
+-rw-rw-rw-   0        0        0      960 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/authorization/__init__.py
+-rw-rw-rw-   0        0        0     2350 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/authorization/sent_code.py
+-rw-rw-rw-   0        0        0     1986 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/authorization/terms_of_service.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.410547 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/
+-rw-rw-rw-   0        0        0     2901 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command.py
+-rw-rw-rw-   0        0        0     2861 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope.py
+-rw-rw-rw-   0        0        0     1325 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-rw-rw-   0        0        0     1290 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-rw-rw-   0        0        0     1281 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-rw-rw-   0        0        0     1605 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-rw-rw-   0        0        0     1682 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-rw-rw-   0        0        0     1865 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-rw-rw-   0        0        0     1341 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-rw-rw-   0        0        0     1058 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/callback_game.py
+-rw-rw-rw-   0        0        0    13110 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/callback_query.py
+-rw-rw-rw-   0        0        0     2449 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/force_reply.py
+-rw-rw-rw-   0        0        0     2286 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/game_high_score.py
+-rw-rw-rw-   0        0        0     8328 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0     2536 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0     3609 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/keyboard_button.py
+-rw-rw-rw-   0        0        0     3802 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/login_url.py
+-rw-rw-rw-   0        0        0     1647 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button.py
+-rw-rw-rw-   0        0        0     1241 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_commands.py
+-rw-rw-rw-   0        0        0     1244 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_default.py
+-rw-rw-rw-   0        0        0     1860 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-rw-rw-   0        0        0     4687 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0     2397 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     1606 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-rw-rw-   0        0        0     1350 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/bots_and_keyboards/web_app_info.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.534471 noelgram1-0.0.2/noelgram/types/inline_mode/
+-rw-rw-rw-   0        0        0     2802 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/__init__.py
+-rw-rw-rw-   0        0        0     3761 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/chosen_inline_result.py
+-rw-rw-rw-   0        0        0     7479 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query.py
+-rw-rw-rw-   0        0        0     2474 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result.py
+-rw-rw-rw-   0        0        0     5931 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_animation.py
+-rw-rw-rw-   0        0        0     3403 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     4625 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_audio.py
+-rw-rw-rw-   0        0        0     4353 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-rw-rw-   0        0        0     4130 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-rw-rw-   0        0        0     4501 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_document.py
+-rw-rw-rw-   0        0        0     4423 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-rw-rw-   0        0        0     3109 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-rw-rw-   0        0        0     4508 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_video.py
+-rw-rw-rw-   0        0        0     4310 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-rw-rw-   0        0        0     4246 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_contact.py
+-rw-rw-rw-   0        0        0     5385 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     4741 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_location.py
+-rw-rw-rw-   0        0        0     5408 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     4885 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_venue.py
+-rw-rw-rw-   0        0        0     5625 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_video.py
+-rw-rw-rw-   0        0        0     4474 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_voice.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.596432 noelgram1-0.0.2/noelgram/types/input_media/
+-rw-rw-rw-   0        0        0     1344 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media.py
+-rw-rw-rw-   0        0        0     3513 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media_animation.py
+-rw-rw-rw-   0        0        0     3364 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media_audio.py
+-rw-rw-rw-   0        0        0     2836 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media_document.py
+-rw-rw-rw-   0        0        0     2748 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media_photo.py
+-rw-rw-rw-   0        0        0     3711 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_media_video.py
+-rw-rw-rw-   0        0        0     1788 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_media/input_phone_contact.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.608424 noelgram1-0.0.2/noelgram/types/input_message_content/
+-rw-rw-rw-   0        0        0     1030 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_message_content/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_message_content/input_message_content.py
+-rw-rw-rw-   0        0        0     2706 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/input_message_content/input_text_message_content.py
+-rw-rw-rw-   0        0        0     1123 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/list.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:34.799543 noelgram1-0.0.2/noelgram/types/messages_and_media/
+-rw-rw-rw-   0        0        0     1883 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/__init__.py
+-rw-rw-rw-   0        0        0     4165 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/animation.py
+-rw-rw-rw-   0        0        0     4190 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/audio.py
+-rw-rw-rw-   0        0        0     2278 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/contact.py
+-rw-rw-rw-   0        0        0     1634 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/dice.py
+-rw-rw-rw-   0        0        0     3507 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/document.py
+-rw-rw-rw-   0        0        0     3143 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/game.py
+-rw-rw-rw-   0        0        0     1715 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/location.py
+-rw-rw-rw-   0        0        0   151898 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/message.py
+-rw-rw-rw-   0        0        0     4476 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/message_entity.py
+-rw-rw-rw-   0        0        0     1856 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/message_reactions.py
+-rw-rw-rw-   0        0        0     4439 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/photo.py
+-rw-rw-rw-   0        0        0     7240 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/poll.py
+-rw-rw-rw-   0        0        0     1582 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/poll_option.py
+-rw-rw-rw-   0        0        0     2703 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/reaction.py
+-rw-rw-rw-   0        0        0     7115 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/sticker.py
+-rw-rw-rw-   0        0        0     1478 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/stripped_thumbnail.py
+-rw-rw-rw-   0        0        0     3866 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/thumbnail.py
+-rw-rw-rw-   0        0        0     2365 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/venue.py
+-rw-rw-rw-   0        0        0     4523 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/video.py
+-rw-rw-rw-   0        0        0     3709 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/video_note.py
+-rw-rw-rw-   0        0        0     3300 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/voice.py
+-rw-rw-rw-   0        0        0     1616 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/web_app_data.py
+-rw-rw-rw-   0        0        0     6538 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/messages_and_media/web_page.py
+-rw-rw-rw-   0        0        0     3983 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/object.py
+-rw-rw-rw-   0        0        0     1029 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/update.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:35.025404 noelgram1-0.0.2/noelgram/types/user_and_chats/
+-rw-rw-rw-   0        0        0     2364 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/__init__.py
+-rw-rw-rw-   0        0        0    33812 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat.py
+-rw-rw-rw-   0        0        0     2299 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-rw-rw-   0        0        0    20324 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_event.py
+-rw-rw-rw-   0        0        0     5689 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_event_filter.py
+-rw-rw-rw-   0        0        0     4709 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_invite_link.py
+-rw-rw-rw-   0        0        0     4384 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_join_request.py
+-rw-rw-rw-   0        0        0     2646 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_joiner.py
+-rw-rw-rw-   0        0        0     9671 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_member.py
+-rw-rw-rw-   0        0        0     3776 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_member_updated.py
+-rw-rw-rw-   0        0        0     4480 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_permissions.py
+-rw-rw-rw-   0        0        0     4074 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_photo.py
+-rw-rw-rw-   0        0        0     2671 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_preview.py
+-rw-rw-rw-   0        0        0     5063 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_privileges.py
+-rw-rw-rw-   0        0        0     2425 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/chat_reactions.py
+-rw-rw-rw-   0        0        0     2761 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/dialog.py
+-rw-rw-rw-   0        0        0     2499 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/emoji_status.py
+-rw-rw-rw-   0        0        0     2012 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/invite_link_importer.py
+-rw-rw-rw-   0        0        0     1713 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/restriction.py
+-rw-rw-rw-   0        0        0    13525 2023-07-16 07:00:57.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/user.py
+-rw-rw-rw-   0        0        0     1387 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_ended.py
+-rw-rw-rw-   0        0        0     1660 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_members_invited.py
+-rw-rw-rw-   0        0        0     1574 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_scheduled.py
+-rw-rw-rw-   0        0        0     1072 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_started.py
+-rw-rw-rw-   0        0        0    10943 2023-07-16 05:27:30.000000 noelgram1-0.0.2/noelgram/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:32.303635 noelgram1-0.0.2/noelgram1.egg-info/
+-rw-rw-rw-   0        0        0     4472 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18895 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 07:01:31.000000 noelgram1-0.0.2/noelgram1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2023-07-16 05:27:30.000000 noelgram1-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 07:01:35.075373 noelgram1-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3599 2023-07-16 05:50:30.000000 noelgram1-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:35.043392 noelgram1-0.0.2/tests/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:35.052388 noelgram1-0.0.2/tests/filters/
+-rw-rw-rw-   0        0        0     1237 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/filters/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/filters/test_command.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:01:35.070381 noelgram1-0.0.2/tests/parser/
+-rw-rw-rw-   0        0        0      835 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/parser/__init__.py
+-rw-rw-rw-   0        0        0     6411 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/parser/test_html.py
+-rw-rw-rw-   0        0        0     8402 2023-07-16 05:27:30.000000 noelgram1-0.0.2/tests/test_file_id.py
```

### Comparing `noelgram1-0.0.1/COPYING` & `noelgram1-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/COPYING.lesser` & `noelgram1-0.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/NOTICE` & `noelgram1-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/PKG-INFO` & `noelgram1-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noelgram1
-Version: 0.0.1
+Version: 0.0.2
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram
 Download-URL: https://github.com/noelgram/noelgram/releases/latest
 Author: Dan
 Author-email: dan@noelgram.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/noelgram/noelgram/issues
@@ -36,16 +36,16 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
-    <a href="https://github.com/noelgram/noelgram">
-        <img src="https://docs.noelgram.org/_static/noelgram.png" alt="Noelgram" width="128">
+    <a href="https://github.com/pyrogram/pyrogram">
+        <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="Noelgram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br>
     <a href="https://noelgram.org">
         Homepage
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noelgram1 Version: 0.0.1 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: noelgram1 Version: 0.0.2 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram Download-URL: https://github.com/
 noelgram/noelgram/releases/latest Author: Dan Author-email: dan@noelgram.org
 License: LGPLv3 Project-URL: Tracker, https://github.com/noelgram/noelgram/
 issues Project-URL: Community, https://t.me/noelgram Project-URL: Source,
 https://github.com/noelgram/noelgram Project-URL: Documentation, https://
 docs.noelgram.org Keywords: telegram chat messenger mtproto api client library
```

### Comparing `noelgram1-0.0.1/README.md` & `noelgram1-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
-    <a href="https://github.com/noelgram/noelgram">
-        <img src="https://docs.noelgram.org/_static/noelgram.png" alt="Noelgram" width="128">
+    <a href="https://github.com/pyrogram/pyrogram">
+        <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="Noelgram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br>
     <a href="https://noelgram.org">
         Homepage
     </a>
```

### Comparing `noelgram1-0.0.1/compiler/__init__.py` & `noelgram1-0.0.2/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/__init__.py` & `noelgram1-0.0.2/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/compiler.py` & `noelgram1-0.0.2/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/source/auth_key.tl` & `noelgram1-0.0.2/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/source/main_api.tl` & `noelgram1-0.0.2/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/source/sys_msgs.tl` & `noelgram1-0.0.2/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/template/combinator.txt` & `noelgram1-0.0.2/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/api/template/type.txt` & `noelgram1-0.0.2/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/docs/__init__.py` & `noelgram1-0.0.2/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/docs/compiler.py` & `noelgram1-0.0.2/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/__init__.py` & `noelgram1-0.0.2/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/compiler.py` & `noelgram1-0.0.2/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/sort.py` & `noelgram1-0.0.2/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv` & `noelgram1-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv` & `noelgram1-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv` & `noelgram1-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `noelgram1-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `noelgram1-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/__init__.py` & `noelgram1-0.0.2/noelgram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Noelgram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `noelgram1-0.0.1/noelgram/client.py` & `noelgram1-0.0.2/noelgram/client.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/__init__.py` & `noelgram1-0.0.2/noelgram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/connection.py` & `noelgram1-0.0.2/noelgram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/__init__.py` & `noelgram1-0.0.2/noelgram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/__init__.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_abridged.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_abridged_o.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_full.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/connection/transport/tcp/tcp_intermediate_o.py` & `noelgram1-0.0.2/noelgram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/crypto/__init__.py` & `noelgram1-0.0.2/noelgram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/crypto/aes.py` & `noelgram1-0.0.2/noelgram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/crypto/mtproto.py` & `noelgram1-0.0.2/noelgram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/crypto/prime.py` & `noelgram1-0.0.2/noelgram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/crypto/rsa.py` & `noelgram1-0.0.2/noelgram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/dispatcher.py` & `noelgram1-0.0.2/noelgram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/emoji.py` & `noelgram1-0.0.2/noelgram/emoji.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/__init__.py` & `noelgram1-0.0.2/noelgram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/auto_name.py` & `noelgram1-0.0.2/noelgram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/chat_action.py` & `noelgram1-0.0.2/noelgram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/chat_event_action.py` & `noelgram1-0.0.2/noelgram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/chat_member_status.py` & `noelgram1-0.0.2/noelgram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/chat_members_filter.py` & `noelgram1-0.0.2/noelgram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/chat_type.py` & `noelgram1-0.0.2/noelgram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/message_entity_type.py` & `noelgram1-0.0.2/noelgram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/message_media_type.py` & `noelgram1-0.0.2/noelgram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/message_service_type.py` & `noelgram1-0.0.2/noelgram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/messages_filter.py` & `noelgram1-0.0.2/noelgram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/next_code_type.py` & `noelgram1-0.0.2/noelgram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/parse_mode.py` & `noelgram1-0.0.2/noelgram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/poll_type.py` & `noelgram1-0.0.2/noelgram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/sent_code_type.py` & `noelgram1-0.0.2/noelgram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/enums/user_status.py` & `noelgram1-0.0.2/noelgram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/errors/__init__.py` & `noelgram1-0.0.2/noelgram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/errors/rpc_error.py` & `noelgram1-0.0.2/noelgram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/file_id.py` & `noelgram1-0.0.2/noelgram/file_id.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/filters.py` & `noelgram1-0.0.2/noelgram/filters.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/__init__.py` & `noelgram1-0.0.2/noelgram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/callback_query_handler.py` & `noelgram1-0.0.2/noelgram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/chat_join_request_handler.py` & `noelgram1-0.0.2/noelgram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/chat_member_updated_handler.py` & `noelgram1-0.0.2/noelgram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/chosen_inline_result_handler.py` & `noelgram1-0.0.2/noelgram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/deleted_messages_handler.py` & `noelgram1-0.0.2/noelgram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/disconnect_handler.py` & `noelgram1-0.0.2/noelgram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/edited_message_handler.py` & `noelgram1-0.0.2/noelgram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/handler.py` & `noelgram1-0.0.2/noelgram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/inline_query_handler.py` & `noelgram1-0.0.2/noelgram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/message_handler.py` & `noelgram1-0.0.2/noelgram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/poll_handler.py` & `noelgram1-0.0.2/noelgram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/raw_update_handler.py` & `noelgram1-0.0.2/noelgram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/handlers/user_status_handler.py` & `noelgram1-0.0.2/noelgram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/__init__.py` & `noelgram1-0.0.2/noelgram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/advanced/__init__.py` & `noelgram1-0.0.2/noelgram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/advanced/invoke.py` & `noelgram1-0.0.2/noelgram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/advanced/resolve_peer.py` & `noelgram1-0.0.2/noelgram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/advanced/save_file.py` & `noelgram1-0.0.2/noelgram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/__init__.py` & `noelgram1-0.0.2/noelgram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/accept_terms_of_service.py` & `noelgram1-0.0.2/noelgram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/check_password.py` & `noelgram1-0.0.2/noelgram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/connect.py` & `noelgram1-0.0.2/noelgram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/disconnect.py` & `noelgram1-0.0.2/noelgram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/get_password_hint.py` & `noelgram1-0.0.2/noelgram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/initialize.py` & `noelgram1-0.0.2/noelgram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/log_out.py` & `noelgram1-0.0.2/noelgram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/recover_password.py` & `noelgram1-0.0.2/noelgram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/resend_code.py` & `noelgram1-0.0.2/noelgram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/send_code.py` & `noelgram1-0.0.2/noelgram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/send_recovery_code.py` & `noelgram1-0.0.2/noelgram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/sign_in.py` & `noelgram1-0.0.2/noelgram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/sign_in_bot.py` & `noelgram1-0.0.2/noelgram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/sign_up.py` & `noelgram1-0.0.2/noelgram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/auth/terminate.py` & `noelgram1-0.0.2/noelgram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/__init__.py` & `noelgram1-0.0.2/noelgram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/answer_callback_query.py` & `noelgram1-0.0.2/noelgram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/answer_inline_query.py` & `noelgram1-0.0.2/noelgram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/answer_web_app_query.py` & `noelgram1-0.0.2/noelgram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/delete_bot_commands.py` & `noelgram1-0.0.2/noelgram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/get_bot_commands.py` & `noelgram1-0.0.2/noelgram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/get_bot_default_privileges.py` & `noelgram1-0.0.2/noelgram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/get_chat_menu_button.py` & `noelgram1-0.0.2/noelgram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/get_game_high_scores.py` & `noelgram1-0.0.2/noelgram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/get_inline_bot_results.py` & `noelgram1-0.0.2/noelgram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/request_callback_answer.py` & `noelgram1-0.0.2/noelgram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/send_game.py` & `noelgram1-0.0.2/noelgram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/send_inline_bot_result.py` & `noelgram1-0.0.2/noelgram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/set_bot_commands.py` & `noelgram1-0.0.2/noelgram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/set_bot_default_privileges.py` & `noelgram1-0.0.2/noelgram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/set_chat_menu_button.py` & `noelgram1-0.0.2/noelgram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/bots/set_game_score.py` & `noelgram1-0.0.2/noelgram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/__init__.py` & `noelgram1-0.0.2/noelgram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/add_chat_members.py` & `noelgram1-0.0.2/noelgram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/archive_chats.py` & `noelgram1-0.0.2/noelgram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/ban_chat_member.py` & `noelgram1-0.0.2/noelgram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/create_channel.py` & `noelgram1-0.0.2/noelgram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/create_group.py` & `noelgram1-0.0.2/noelgram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/create_supergroup.py` & `noelgram1-0.0.2/noelgram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/delete_channel.py` & `noelgram1-0.0.2/noelgram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/delete_chat_photo.py` & `noelgram1-0.0.2/noelgram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/delete_supergroup.py` & `noelgram1-0.0.2/noelgram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/delete_user_history.py` & `noelgram1-0.0.2/noelgram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat_event_log.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat_member.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat_members.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat_members_count.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_chat_online_count.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_dialogs.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_dialogs_count.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_nearby_chats.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/get_send_as_chats.py` & `noelgram1-0.0.2/noelgram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/join_chat.py` & `noelgram1-0.0.2/noelgram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/leave_chat.py` & `noelgram1-0.0.2/noelgram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/mark_chat_unread.py` & `noelgram1-0.0.2/noelgram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/pin_chat_message.py` & `noelgram1-0.0.2/noelgram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/promote_chat_member.py` & `noelgram1-0.0.2/noelgram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/restrict_chat_member.py` & `noelgram1-0.0.2/noelgram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_administrator_title.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_description.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_permissions.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_photo.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_protected_content.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_title.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_chat_username.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_send_as_chat.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/set_slow_mode.py` & `noelgram1-0.0.2/noelgram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/unarchive_chats.py` & `noelgram1-0.0.2/noelgram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/unban_chat_member.py` & `noelgram1-0.0.2/noelgram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/unpin_all_chat_messages.py` & `noelgram1-0.0.2/noelgram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/chats/unpin_chat_message.py` & `noelgram1-0.0.2/noelgram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/__init__.py` & `noelgram1-0.0.2/noelgram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/add_contact.py` & `noelgram1-0.0.2/noelgram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/delete_contacts.py` & `noelgram1-0.0.2/noelgram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/get_contacts.py` & `noelgram1-0.0.2/noelgram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/get_contacts_count.py` & `noelgram1-0.0.2/noelgram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/contacts/import_contacts.py` & `noelgram1-0.0.2/noelgram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/__init__.py` & `noelgram1-0.0.2/noelgram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_callback_query.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_chat_join_request.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_chat_member_updated.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_chosen_inline_result.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_deleted_messages.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_disconnect.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_edited_message.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_inline_query.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_message.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_poll.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_raw_update.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/decorators/on_user_status.py` & `noelgram1-0.0.2/noelgram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/__init__.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/approve_all_chat_join_requests.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/approve_chat_join_request.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/create_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/decline_all_chat_join_requests.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/decline_chat_join_request.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/delete_chat_admin_invite_links.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/delete_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/edit_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/export_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/get_chat_join_requests.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/invite_links/revoke_chat_invite_link.py` & `noelgram1-0.0.2/noelgram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/__init__.py` & `noelgram1-0.0.2/noelgram/methods/messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 from .send_venue import SendVenue
 from .send_video import SendVideo
 from .send_video_note import SendVideoNote
 from .send_voice import SendVoice
 from .stop_poll import StopPoll
 from .stream_media import StreamMedia
 from .vote_poll import VotePoll
+from .wait_for_callback_query import WaitForCallbackQuery
+from .wait_for_message import WaitForMessage
 
 
 class Messages(
     DeleteMessages,
     EditMessageCaption,
     EditMessageReplyMarkup,
     EditMessageMedia,
@@ -110,10 +112,12 @@
     SearchMessagesCount,
     SearchGlobalCount,
     GetDiscussionMessage,
     SendReaction,
     GetDiscussionReplies,
     GetDiscussionRepliesCount,
     StreamMedia,
-    GetCustomEmojiStickers
+    GetCustomEmojiStickers,
+    WaitForCallbackQuery,
+    WaitForMessage
 ):
     pass
```

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/copy_media_group.py` & `noelgram1-0.0.2/noelgram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/copy_message.py` & `noelgram1-0.0.2/noelgram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/delete_messages.py` & `noelgram1-0.0.2/noelgram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/download_media.py` & `noelgram1-0.0.2/noelgram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_inline_caption.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_inline_media.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_inline_reply_markup.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_inline_text.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_message_caption.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_message_media.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_message_reply_markup.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/edit_message_text.py` & `noelgram1-0.0.2/noelgram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/forward_messages.py` & `noelgram1-0.0.2/noelgram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_chat_history.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_chat_history_count.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_custom_emoji_stickers.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_discussion_message.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_discussion_replies.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_discussion_replies_count.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_media_group.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/get_messages.py` & `noelgram1-0.0.2/noelgram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/inline_session.py` & `noelgram1-0.0.2/noelgram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/read_chat_history.py` & `noelgram1-0.0.2/noelgram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/retract_vote.py` & `noelgram1-0.0.2/noelgram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/search_global.py` & `noelgram1-0.0.2/noelgram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/search_global_count.py` & `noelgram1-0.0.2/noelgram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/search_messages.py` & `noelgram1-0.0.2/noelgram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/search_messages_count.py` & `noelgram1-0.0.2/noelgram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_animation.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_audio.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_cached_media.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_chat_action.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_contact.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_dice.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_document.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_location.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_media_group.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_message.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_photo.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_poll.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_reaction.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_sticker.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_venue.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_video.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_video_note.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/send_voice.py` & `noelgram1-0.0.2/noelgram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/stop_poll.py` & `noelgram1-0.0.2/noelgram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/stream_media.py` & `noelgram1-0.0.2/noelgram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/messages/vote_poll.py` & `noelgram1-0.0.2/noelgram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/password/__init__.py` & `noelgram1-0.0.2/noelgram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/password/change_cloud_password.py` & `noelgram1-0.0.2/noelgram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/password/enable_cloud_password.py` & `noelgram1-0.0.2/noelgram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/password/remove_cloud_password.py` & `noelgram1-0.0.2/noelgram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/__init__.py` & `noelgram1-0.0.2/noelgram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/block_user.py` & `noelgram1-0.0.2/noelgram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/delete_profile_photos.py` & `noelgram1-0.0.2/noelgram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_chat_photos.py` & `noelgram1-0.0.2/noelgram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_chat_photos_count.py` & `noelgram1-0.0.2/noelgram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_common_chats.py` & `noelgram1-0.0.2/noelgram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_default_emoji_statuses.py` & `noelgram1-0.0.2/noelgram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_me.py` & `noelgram1-0.0.2/noelgram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/get_users.py` & `noelgram1-0.0.2/noelgram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/set_emoji_status.py` & `noelgram1-0.0.2/noelgram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/set_profile_photo.py` & `noelgram1-0.0.2/noelgram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/set_username.py` & `noelgram1-0.0.2/noelgram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/unblock_user.py` & `noelgram1-0.0.2/noelgram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/users/update_profile.py` & `noelgram1-0.0.2/noelgram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/__init__.py` & `noelgram1-0.0.2/noelgram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/add_handler.py` & `noelgram1-0.0.2/noelgram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/compose.py` & `noelgram1-0.0.2/noelgram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/export_session_string.py` & `noelgram1-0.0.2/noelgram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/idle.py` & `noelgram1-0.0.2/noelgram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/remove_handler.py` & `noelgram1-0.0.2/noelgram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/restart.py` & `noelgram1-0.0.2/noelgram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/run.py` & `noelgram1-0.0.2/noelgram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/start.py` & `noelgram1-0.0.2/noelgram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/stop.py` & `noelgram1-0.0.2/noelgram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/methods/utilities/stop_transmission.py` & `noelgram1-0.0.2/noelgram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/mime_types.py` & `noelgram1-0.0.2/noelgram/mime_types.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/parser/__init__.py` & `noelgram1-0.0.2/noelgram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/parser/html.py` & `noelgram1-0.0.2/noelgram/parser/html.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/parser/markdown.py` & `noelgram1-0.0.2/noelgram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/parser/parser.py` & `noelgram1-0.0.2/noelgram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/parser/utils.py` & `noelgram1-0.0.2/noelgram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/__init__.py` & `noelgram1-0.0.2/noelgram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/__init__.py` & `noelgram1-0.0.2/noelgram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/future_salt.py` & `noelgram1-0.0.2/noelgram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/future_salts.py` & `noelgram1-0.0.2/noelgram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/gzip_packed.py` & `noelgram1-0.0.2/noelgram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/list.py` & `noelgram1-0.0.2/noelgram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/message.py` & `noelgram1-0.0.2/noelgram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/msg_container.py` & `noelgram1-0.0.2/noelgram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/__init__.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/bool.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/bytes.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/double.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/int.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/string.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/primitives/vector.py` & `noelgram1-0.0.2/noelgram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/raw/core/tl_object.py` & `noelgram1-0.0.2/noelgram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/__init__.py` & `noelgram1-0.0.2/noelgram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/auth.py` & `noelgram1-0.0.2/noelgram/session/auth.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/internals/__init__.py` & `noelgram1-0.0.2/noelgram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/internals/data_center.py` & `noelgram1-0.0.2/noelgram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/internals/msg_factory.py` & `noelgram1-0.0.2/noelgram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/internals/msg_id.py` & `noelgram1-0.0.2/noelgram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/internals/seq_no.py` & `noelgram1-0.0.2/noelgram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/session/session.py` & `noelgram1-0.0.2/noelgram/session/session.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/storage/__init__.py` & `noelgram1-0.0.2/noelgram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/storage/file_storage.py` & `noelgram1-0.0.2/noelgram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/storage/memory_storage.py` & `noelgram1-0.0.2/noelgram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/storage/sqlite_storage.py` & `noelgram1-0.0.2/noelgram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/storage/storage.py` & `noelgram1-0.0.2/noelgram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/sync.py` & `noelgram1-0.0.2/noelgram/sync.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/__init__.py` & `noelgram1-0.0.2/noelgram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/authorization/__init__.py` & `noelgram1-0.0.2/noelgram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/authorization/sent_code.py` & `noelgram1-0.0.2/noelgram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/authorization/terms_of_service.py` & `noelgram1-0.0.2/noelgram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/__init__.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/bot_command_scope_default.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/callback_game.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/callback_query.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/force_reply.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/game_high_score.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_button.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/keyboard_button.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/login_url.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_commands.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_default.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/menu_button_web_app.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/sent_web_app_message.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/bots_and_keyboards/web_app_info.py` & `noelgram1-0.0.2/noelgram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/__init__.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/chosen_inline_result.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_animation.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_article.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_audio.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_animation.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_audio.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_document.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_photo.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_sticker.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_video.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_cached_voice.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_contact.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_document.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_location.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_photo.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_venue.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_video.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/inline_mode/inline_query_result_voice.py` & `noelgram1-0.0.2/noelgram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/__init__.py` & `noelgram1-0.0.2/noelgram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media_animation.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media_audio.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media_document.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media_photo.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_media_video.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_media/input_phone_contact.py` & `noelgram1-0.0.2/noelgram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_message_content/__init__.py` & `noelgram1-0.0.2/noelgram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_message_content/input_message_content.py` & `noelgram1-0.0.2/noelgram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/input_message_content/input_text_message_content.py` & `noelgram1-0.0.2/noelgram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/list.py` & `noelgram1-0.0.2/noelgram/types/list.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/__init__.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/animation.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/audio.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/contact.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/dice.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/document.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/game.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/location.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/message.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -9250,8 +9250,245 @@
 00024210: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
 00024220: 662e 5f63 6c69 656e 742e 756e 7069 6e5f  f._client.unpin_
 00024230: 6368 6174 5f6d 6573 7361 6765 280d 0a20  chat_message(.. 
 00024240: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
 00024250: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
 00024260: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
 00024270: 7373 6167 655f 6964 3d73 656c 662e 6964  ssage_id=self.id
-00024280: 0d0a 2020 2020 2020 2020 290d 0a         ..        )..
+00024280: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00024290: 2020 2061 7379 6e63 2064 6566 2061 736b     async def ask
+000242a0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+000242b0: 0d0a 2020 2020 2020 2020 7465 7874 3a20  ..        text: 
+000242c0: 7374 722c 0d0a 2020 2020 2020 2020 7175  str,..        qu
+000242d0: 6f74 653a 2062 6f6f 6c20 3d20 4e6f 6e65  ote: bool = None
+000242e0: 2c0d 0a20 2020 2020 2020 2070 6172 7365  ,..        parse
+000242f0: 5f6d 6f64 653a 204f 7074 696f 6e61 6c5b  _mode: Optional[
+00024300: 2265 6e75 6d73 2e50 6172 7365 4d6f 6465  "enums.ParseMode
+00024310: 225d 203d 204e 6f6e 652c 0d0a 2020 2020  "] = None,..    
+00024320: 2020 2020 656e 7469 7469 6573 3a20 4c69      entities: Li
+00024330: 7374 5b22 7479 7065 732e 4d65 7373 6167  st["types.Messag
+00024340: 6545 6e74 6974 7922 5d20 3d20 4e6f 6e65  eEntity"] = None
+00024350: 2c0d 0a20 2020 2020 2020 2064 6973 6162  ,..        disab
+00024360: 6c65 5f77 6562 5f70 6167 655f 7072 6576  le_web_page_prev
+00024370: 6965 773a 2062 6f6f 6c20 3d20 4e6f 6e65  iew: bool = None
+00024380: 2c0d 0a20 2020 2020 2020 2064 6973 6162  ,..        disab
+00024390: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3a  le_notification:
+000243a0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20   bool = None,.. 
+000243b0: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
+000243c0: 6d65 7373 6167 655f 6964 3a20 696e 7420  message_id: int 
+000243d0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+000243e0: 2072 6570 6c79 5f6d 6172 6b75 703d 4e6f   reply_markup=No
+000243f0: 6e65 2c0d 0a20 2020 2020 2020 2066 696c  ne,..        fil
+00024400: 7465 7273 3d4e 6f6e 652c 0d0a 2020 2020  ters=None,..    
+00024410: 2020 2020 7469 6d65 6f75 743a 2069 6e74      timeout: int
+00024420: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
+00024430: 3e20 224d 6573 7361 6765 223a 0d0a 2020  > "Message":..  
+00024440: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+00024450: 6574 686f 6420 2a61 736b 2a20 6f66 203a  ethod *ask* of :
+00024460: 6f62 6a3a 607e 6e6f 656c 6772 616d 2e74  obj:`~noelgram.t
+00024470: 7970 6573 2e4d 6573 7361 6765 602e 0d0a  ypes.Message`...
+00024480: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00024490: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+000244a0: 6375 7420 666f 723a 0d0a 2020 2020 2020  cut for:..      
+000244b0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+000244c0: 3a20 7079 7468 6f6e 0d0a 2020 2020 2020  : python..      
+000244d0: 2020 2020 2020 636c 6965 6e74 2e73 656e        client.sen
+000244e0: 645f 6d65 7373 6167 6528 6368 6174 5f69  d_message(chat_i
+000244f0: 642c 2022 5768 6174 2069 7320 796f 7572  d, "What is your
+00024500: 206e 616d 653f 2229 0d0a 2020 2020 2020   name?")..      
+00024510: 2020 2020 2020 636c 6965 6e74 2e77 6169        client.wai
+00024520: 745f 666f 725f 6d65 7373 6167 6528 6368  t_for_message(ch
+00024530: 6174 5f69 6429 0d0a 2020 2020 2020 2020  at_id)..        
+00024540: 2020 2020 0d0a 2020 2020 2020 2020 4578      ..        Ex
+00024550: 616d 706c 653a 0d0a 2020 2020 2020 2020  ample:..        
+00024560: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00024570: 6b3a 3a20 7079 7468 6f6e 0d0a 2020 2020  k:: python..    
+00024580: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+00024590: 6167 652e 6173 6b28 2257 6861 7420 6973  age.ask("What is
+000245a0: 2079 6f75 7220 6e61 6d65 3f22 290d 0a20   your name?").. 
+000245b0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000245c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000245d0: 7465 7874 2028 6060 7374 7260 6029 3a0d  text (``str``):.
+000245e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000245f0: 2054 6578 7420 6f66 2074 6865 206d 6573   Text of the mes
+00024600: 7361 6765 2074 6f20 6265 2073 656e 742e  sage to be sent.
+00024610: 0d0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
+00024620: 6f74 6520 2860 6062 6f6f 6c60 602c 202a  ote (``bool``, *
+00024630: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00024640: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+00024650: 6060 5472 7565 6060 2c20 7468 6520 6d65  ``True``, the me
+00024660: 7373 6167 6520 7769 6c6c 2062 6520 7365  ssage will be se
+00024670: 6e74 2061 7320 6120 7265 706c 7920 746f  nt as a reply to
+00024680: 2074 6869 7320 6d65 7373 6167 652e 0d0a   this message...
+00024690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246a0: 4966 202a 7265 706c 795f 746f 5f6d 6573  If *reply_to_mes
+000246b0: 7361 6765 5f69 642a 2069 7320 7061 7373  sage_id* is pass
+000246c0: 6564 2c20 7468 6973 2070 6172 616d 6574  ed, this paramet
+000246d0: 6572 2077 696c 6c20 6265 2069 676e 6f72  er will be ignor
+000246e0: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
+000246f0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00024700: 2060 6054 7275 6560 6020 696e 2067 726f   ``True`` in gro
+00024710: 7570 2063 6861 7473 2061 6e64 2060 6046  up chats and ``F
+00024720: 616c 7365 6060 2069 6e20 7072 6976 6174  alse`` in privat
+00024730: 6520 6368 6174 732e 0d0a 2020 2020 2020  e chats...      
+00024740: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
+00024750: 2028 3a6f 626a 3a60 7e6e 6f65 6c67 7261   (:obj:`~noelgra
+00024760: 6d2e 656e 756d 732e 5061 7273 654d 6f64  m.enums.ParseMod
+00024770: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
+00024780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024790: 2020 4279 2064 6566 6175 6c74 2c20 7465    By default, te
+000247a0: 7874 7320 6172 6520 7061 7273 6564 2075  xts are parsed u
+000247b0: 7369 6e67 2062 6f74 6820 4d61 726b 646f  sing both Markdo
+000247c0: 776e 2061 6e64 2048 544d 4c20 7374 796c  wn and HTML styl
+000247d0: 6573 2e0d 0a20 2020 2020 2020 2020 2020  es...           
+000247e0: 2020 2020 2059 6f75 2063 616e 2063 6f6d       You can com
+000247f0: 6269 6e65 2062 6f74 6820 7379 6e74 6178  bine both syntax
+00024800: 6573 2074 6f67 6574 6865 722e 0d0a 2020  es together...  
+00024810: 2020 2020 2020 2020 2020 656e 7469 7469            entiti
+00024820: 6573 2028 4c69 7374 206f 6620 3a6f 626a  es (List of :obj
+00024830: 3a60 7e6e 6f65 6c67 7261 6d2e 7479 7065  :`~noelgram.type
+00024840: 732e 4d65 7373 6167 6545 6e74 6974 7960  s.MessageEntity`
+00024850: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00024860: 2020 2020 4c69 7374 206f 6620 7370 6563      List of spec
+00024870: 6961 6c20 656e 7469 7469 6573 2074 6861  ial entities tha
+00024880: 7420 6170 7065 6172 2069 6e20 6d65 7373  t appear in mess
+00024890: 6167 6520 7465 7874 2c20 7768 6963 6820  age text, which 
+000248a0: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
+000248b0: 2069 6e73 7465 6164 206f 6620 2a70 6172   instead of *par
+000248c0: 7365 5f6d 6f64 652a 2e0d 0a20 2020 2020  se_mode*...     
+000248d0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+000248e0: 6562 5f70 6167 655f 7072 6576 6965 7720  eb_page_preview 
+000248f0: 2860 6062 6f6f 6c60 602c 202a 6f70 7469  (``bool``, *opti
+00024900: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+00024910: 2020 2020 2020 2020 2044 6973 6162 6c65           Disable
+00024920: 7320 6c69 6e6b 2070 7265 7669 6577 7320  s link previews 
+00024930: 666f 7220 6c69 6e6b 7320 696e 2074 6869  for links in thi
+00024940: 7320 6d65 7373 6167 652e 0d0a 2020 2020  s message...    
+00024950: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00024960: 6e6f 7469 6669 6361 7469 6f6e 2028 6060  notification (``
+00024970: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+00024980: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+00024990: 2020 2020 2020 5365 6e64 7320 7468 6520        Sends the 
+000249a0: 6d65 7373 6167 6520 7369 6c65 6e74 6c79  message silently
+000249b0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000249c0: 2020 2055 7365 7273 2077 696c 6c20 7265     Users will re
+000249d0: 6365 6976 6520 6120 6e6f 7469 6669 6361  ceive a notifica
+000249e0: 7469 6f6e 2077 6974 6820 6e6f 2073 6f75  tion with no sou
+000249f0: 6e64 2e0d 0a20 2020 2020 2020 2020 2020  nd...           
+00024a00: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00024a10: 655f 6964 2028 6060 696e 7460 602c 202a  e_id (``int``, *
+00024a20: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00024a30: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+00024a40: 7468 6520 6d65 7373 6167 6520 6973 2061  the message is a
+00024a50: 2072 6570 6c79 2c20 4944 206f 6620 7468   reply, ID of th
+00024a60: 6520 6f72 6967 696e 616c 206d 6573 7361  e original messa
+00024a70: 6765 2e0d 0a20 2020 2020 2020 2020 2020  ge...           
+00024a80: 2072 6570 6c79 5f6d 6172 6b75 7020 283a   reply_markup (:
+00024a90: 6f62 6a3a 607e 6e6f 656c 6772 616d 2e74  obj:`~noelgram.t
+00024aa0: 7970 6573 2e49 6e6c 696e 654b 6579 626f  ypes.InlineKeybo
+00024ab0: 6172 644d 6172 6b75 7060 207c 203a 6f62  ardMarkup` | :ob
+00024ac0: 6a3a 607e 6e6f 656c 6772 616d 2e74 7970  j:`~noelgram.typ
+00024ad0: 6573 2e52 6570 6c79 4b65 7962 6f61 7264  es.ReplyKeyboard
+00024ae0: 4d61 726b 7570 6020 7c20 3a6f 626a 3a60  Markup` | :obj:`
+00024af0: 7e6e 6f65 6c67 7261 6d2e 7479 7065 732e  ~noelgram.types.
+00024b00: 5265 706c 794b 6579 626f 6172 6452 656d  ReplyKeyboardRem
+00024b10: 6f76 6560 207c 203a 6f62 6a3a 607e 6e6f  ove` | :obj:`~no
+00024b20: 656c 6772 616d 2e74 7970 6573 2e46 6f72  elgram.types.For
+00024b30: 6365 5265 706c 7960 2c20 2a6f 7074 696f  ceReply`, *optio
+00024b40: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
+00024b50: 2020 2020 2020 2020 4164 6469 7469 6f6e          Addition
+00024b60: 616c 2069 6e74 6572 6661 6365 206f 7074  al interface opt
+00024b70: 696f 6e73 2e20 416e 206f 626a 6563 7420  ions. An object 
+00024b80: 666f 7220 616e 2069 6e6c 696e 6520 6b65  for an inline ke
+00024b90: 7962 6f61 7264 2c20 6375 7374 6f6d 2072  yboard, custom r
+00024ba0: 6570 6c79 206b 6579 626f 6172 642c 0d0a  eply keyboard,..
+00024bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024bc0: 696e 7374 7275 6374 696f 6e73 2074 6f20  instructions to 
+00024bd0: 7265 6d6f 7665 2072 6570 6c79 206b 6579  remove reply key
+00024be0: 626f 6172 6420 6f72 2074 6f20 666f 7263  board or to forc
+00024bf0: 6520 6120 7265 706c 7920 6672 6f6d 2074  e a reply from t
+00024c00: 6865 2075 7365 722e 0d0a 2020 2020 2020  he user...      
+00024c10: 2020 2020 2020 6669 6c74 6572 7320 283a        filters (:
+00024c20: 6f62 6a3a 6046 696c 7465 7273 6029 3a0d  obj:`Filters`):.
+00024c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024c40: 2050 6173 7320 6f6e 6520 6f72 206d 6f72   Pass one or mor
+00024c50: 6520 6669 6c74 6572 7320 746f 2061 6c6c  e filters to all
+00024c60: 6f77 206f 6e6c 7920 6120 7375 6273 6574  ow only a subset
+00024c70: 206f 6620 6361 6c6c 6261 636b 2071 7565   of callback que
+00024c80: 7269 6573 2074 6f20 6265 2070 6173 7365  ries to be passe
+00024c90: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00024ca0: 2020 2069 6e20 796f 7572 2063 616c 6c62     in your callb
+00024cb0: 6163 6b20 6675 6e63 7469 6f6e 2e0d 0a20  ack function... 
+00024cc0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+00024cd0: 7574 2028 6060 696e 7460 602c 202a 6f70  ut (``int``, *op
+00024ce0: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00024cf0: 2020 2020 2020 2020 2020 2054 696d 656f             Timeo
+00024d00: 7574 2069 6e20 7365 636f 6e64 732e 0d0a  ut in seconds...
+00024d10: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00024d20: 0d0a 2020 2020 2020 2020 2020 2020 3a6f  ..            :o
+00024d30: 626a 3a60 7e6e 6f65 6c67 7261 6d2e 7479  bj:`~noelgram.ty
+00024d40: 7065 732e 4d65 7373 6167 6560 3a20 4f6e  pes.Message`: On
+00024d50: 2073 7563 6365 7373 2c20 7468 6520 7265   success, the re
+00024d60: 706c 7920 6d65 7373 6167 6520 6973 2072  ply message is r
+00024d70: 6574 7572 6e65 642e 0d0a 2020 2020 2020  eturned...      
+00024d80: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
+00024d90: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+00024da0: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+00024db0: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+00024dc0: 2e0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
+00024dd0: 7379 6e63 696f 2e54 696d 656f 7574 4572  syncio.TimeoutEr
+00024de0: 726f 723a 2049 6e20 6361 7365 2072 6570  ror: In case rep
+00024df0: 6c79 206e 6f74 2072 6563 6569 7665 6420  ly not received 
+00024e00: 7769 7468 696e 2074 6865 2074 696d 656f  within the timeo
+00024e10: 7574 2e0d 0a20 2020 2020 2020 2022 2222  ut...        """
+00024e20: 0d0a 2020 2020 2020 2020 6966 2071 756f  ..        if quo
+00024e30: 7465 2069 7320 4e6f 6e65 3a0d 0a20 2020  te is None:..   
+00024e40: 2020 2020 2020 2020 2071 756f 7465 203d           quote =
+00024e50: 2073 656c 662e 6368 6174 2e74 7970 6520   self.chat.type 
+00024e60: 213d 2065 6e75 6d73 2e43 6861 7454 7970  != enums.ChatTyp
+00024e70: 652e 5052 4956 4154 450d 0a0d 0a20 2020  e.PRIVATE....   
+00024e80: 2020 2020 2069 6620 7265 706c 795f 746f       if reply_to
+00024e90: 5f6d 6573 7361 6765 5f69 6420 6973 204e  _message_id is N
+00024ea0: 6f6e 6520 616e 6420 7175 6f74 653a 0d0a  one and quote:..
+00024eb0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00024ec0: 795f 746f 5f6d 6573 7361 6765 5f69 6420  y_to_message_id 
+00024ed0: 3d20 7365 6c66 2e69 640d 0a0d 0a20 2020  = self.id....   
+00024ee0: 2020 2020 2072 6571 7565 7374 203d 2061       request = a
+00024ef0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+00024f00: 742e 7365 6e64 5f6d 6573 7361 6765 280d  t.send_message(.
+00024f10: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00024f20: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+00024f30: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+00024f40: 7465 7874 3d74 6578 742c 0d0a 2020 2020  text=text,..    
+00024f50: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
+00024f60: 6465 3d70 6172 7365 5f6d 6f64 652c 0d0a  de=parse_mode,..
+00024f70: 2020 2020 2020 2020 2020 2020 656e 7469              enti
+00024f80: 7469 6573 3d65 6e74 6974 6965 732c 0d0a  ties=entities,..
+00024f90: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00024fa0: 626c 655f 7765 625f 7061 6765 5f70 7265  ble_web_page_pre
+00024fb0: 7669 6577 3d64 6973 6162 6c65 5f77 6562  view=disable_web
+00024fc0: 5f70 6167 655f 7072 6576 6965 772c 0d0a  _page_preview,..
+00024fd0: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00024fe0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00024ff0: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
+00025000: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
+00025010: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
+00025020: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
+00025030: 5f6d 6573 7361 6765 5f69 642c 0d0a 2020  _message_id,..  
+00025040: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00025050: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
+00025060: 6b75 700d 0a20 2020 2020 2020 2029 0d0a  kup..        )..
+00025070: 0d0a 2020 2020 2020 2020 7265 706c 795f  ..        reply_
+00025080: 6d65 7373 6167 6520 3d20 6177 6169 7420  message = await 
+00025090: 7365 6c66 2e5f 636c 6965 6e74 2e77 6169  self._client.wai
+000250a0: 745f 666f 725f 6d65 7373 6167 6528 0d0a  t_for_message(..
+000250b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000250c0: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
+000250d0: 2020 2020 2020 2066 696c 7465 7273 3d66         filters=f
+000250e0: 696c 7465 7273 2c0d 0a20 2020 2020 2020  ilters,..       
+000250f0: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
+00025100: 656f 7574 0d0a 2020 2020 2020 2020 290d  eout..        ).
+00025110: 0a0d 0a20 2020 2020 2020 2072 6570 6c79  ...        reply
+00025120: 5f6d 6573 7361 6765 2e72 6571 7565 7374  _message.request
+00025130: 203d 2072 6571 7565 7374 0d0a 2020 2020   = request..    
+00025140: 2020 2020 7265 7475 726e 2072 6570 6c79      return reply
+00025150: 5f6d 6573 7361 6765 0d0a                 _message..
```

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/message_entity.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/message_reactions.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/photo.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/poll.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/poll_option.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/reaction.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/sticker.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/stripped_thumbnail.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/thumbnail.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/venue.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/video.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/video_note.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/voice.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/web_app_data.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/messages_and_media/web_page.py` & `noelgram1-0.0.2/noelgram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/object.py` & `noelgram1-0.0.2/noelgram/types/object.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/update.py` & `noelgram1-0.0.2/noelgram/types/update.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/__init__.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,23 @@
         if isinstance(chat, raw.types.Chat):
             return Chat._parse_chat_chat(client, chat)
         elif isinstance(chat, raw.types.User):
             return Chat._parse_user_chat(client, chat)
         else:
             return Chat._parse_channel_chat(client, chat)
 
+    def listen(self, *args, **kwargs):
+        return self._client.listen(self.id, *args, **kwargs)
+
+    def ask(self, *args, **kwargs):
+        return self._client.ask(self.id, *args, **kwargs)
+
+    def cancel_listener(self):
+        return self._client.cancel_listener(self.id)
+
     async def archive(self):
         """Bound method *archive* of :obj:`~noelgram.types.Chat`.
 
         Use as a shortcut for:
 
         .. code-block:: python
```

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_admin_with_invite_links.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_event.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_event_filter.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_invite_link.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_join_request.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_joiner.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_member.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_member_updated.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_permissions.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_photo.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_preview.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_privileges.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/chat_reactions.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/dialog.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/emoji_status.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/invite_link_importer.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/restriction.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/user.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,14 +279,23 @@
     def _parse_user_status(client, user_status: "raw.types.UpdateUserStatus"):
         return User(
             id=user_status.user_id,
             **User._parse_status(user_status.status),
             client=client
         )
 
+    def listen(self, *args, **kwargs):
+        return self._client.listen(self.id, *args, **kwargs)
+
+    def ask(self, *args, **kwargs):
+        return self._client.ask(self.id, *args, **kwargs)
+
+    def cancel_listener(self):
+        return self._client.cancel_listener(self.id)
+
     async def archive(self):
         """Bound method *archive* of :obj:`~noelgram.types.User`.
 
         Use as a shortcut for:
 
         .. code-block:: python
```

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_ended.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_members_invited.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_scheduled.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/types/user_and_chats/video_chat_started.py` & `noelgram1-0.0.2/noelgram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram/utils.py` & `noelgram1-0.0.2/noelgram/utils.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/noelgram1.egg-info/PKG-INFO` & `noelgram1-0.0.2/noelgram1.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noelgram1
-Version: 0.0.1
+Version: 0.0.2
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram
 Download-URL: https://github.com/noelgram/noelgram/releases/latest
 Author: Dan
 Author-email: dan@noelgram.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/noelgram/noelgram/issues
@@ -36,16 +36,16 @@
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
-    <a href="https://github.com/noelgram/noelgram">
-        <img src="https://docs.noelgram.org/_static/noelgram.png" alt="Noelgram" width="128">
+    <a href="https://github.com/pyrogram/pyrogram">
+        <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="Noelgram" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
     <br>
     <a href="https://noelgram.org">
         Homepage
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noelgram1 Version: 0.0.1 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: noelgram1 Version: 0.0.2 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/noelgram Download-URL: https://github.com/
 noelgram/noelgram/releases/latest Author: Dan Author-email: dan@noelgram.org
 License: LGPLv3 Project-URL: Tracker, https://github.com/noelgram/noelgram/
 issues Project-URL: Community, https://t.me/noelgram Project-URL: Source,
 https://github.com/noelgram/noelgram Project-URL: Documentation, https://
 docs.noelgram.org Keywords: telegram chat messenger mtproto api client library
```

### Comparing `noelgram1-0.0.1/noelgram1.egg-info/SOURCES.txt` & `noelgram1-0.0.2/noelgram1.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,16 @@
 noelgram/methods/messages/send_venue.py
 noelgram/methods/messages/send_video.py
 noelgram/methods/messages/send_video_note.py
 noelgram/methods/messages/send_voice.py
 noelgram/methods/messages/stop_poll.py
 noelgram/methods/messages/stream_media.py
 noelgram/methods/messages/vote_poll.py
+noelgram/methods/messages/wait_for_callback_query.py
+noelgram/methods/messages/wait_for_message.py
 noelgram/methods/password/__init__.py
 noelgram/methods/password/change_cloud_password.py
 noelgram/methods/password/enable_cloud_password.py
 noelgram/methods/password/remove_cloud_password.py
 noelgram/methods/users/__init__.py
 noelgram/methods/users/block_user.py
 noelgram/methods/users/delete_profile_photos.py
```

### Comparing `noelgram1-0.0.1/setup.py` & `noelgram1-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/__init__.py` & `noelgram1-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/filters/__init__.py` & `noelgram1-0.0.2/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/filters/test_command.py` & `noelgram1-0.0.2/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/parser/__init__.py` & `noelgram1-0.0.2/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/parser/test_html.py` & `noelgram1-0.0.2/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `noelgram1-0.0.1/tests/test_file_id.py` & `noelgram1-0.0.2/tests/test_file_id.py`

 * *Files identical despite different names*

