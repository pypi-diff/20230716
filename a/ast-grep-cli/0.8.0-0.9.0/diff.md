# Comparing `tmp/ast_grep_cli-0.8.0.tar.gz` & `tmp/ast_grep_cli-0.9.0.tar.gz`

## Comparing `ast_grep_cli-0.8.0.tar` & `ast_grep_cli-0.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6357 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11610 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7730 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    11138 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15431 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123    10142 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2990 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     2041 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11369 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4312 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     4996 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10205 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22621 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7648 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     9039 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10644 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     7418 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24629 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      901 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1363 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/scan_test.rs
--rw-r--r--   0     1001      123     1025 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/pyproject.toml
--rw-r--r--   0     1001      123    60241 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4951 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/README.md
--rw-r--r--   0     1001      123     1077 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/LICENSE
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15431 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1911 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123     1815 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123     1515 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     2024 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123    10142 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     2990 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     3114 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     2915 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     2041 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7730 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     5396 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10205 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    22611 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7648 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9061 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10644 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24703 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      901 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1363 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1025 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123    59770 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/PKG-INFO
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.8.0"
+version= "0.9.0"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 anyhow = "1.0"
 bit-set= { version = "0.5.3" }
-globset = "0.4.10"
+globset = "0.4.11"
 regex = { version = "1.9.1" , optional = true }
 serde= { version = "1.0", features = ["derive"] }
 serde_yaml = "0.9.22"
 thiserror= "1.0.43"
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.8.0"
+version= "0.9.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.8.0"
+version= "0.9.0"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.9.1" , optional = true }
 thiserror= "1.0.43"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.8.0"
+version= "0.9.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.8.0"
+version= "0.9.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 ast-grep-config.path = "../ast-grep-config"
 
 dashmap = "5.4.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.100"
+serde_json = "1.0.102"
 tower-lsp = "0.19.0"
```

### Comparing `ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/Cargo.toml` & `ast_grep_cli-0.9.0/crates/cli/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.8.0"
+version= "0.9.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 # license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
@@ -31,18 +31,18 @@
 ast-grep-dynamic.path = "../../local_dependencies/ast-grep-dynamic"
 ast-grep-language.path = "../../local_dependencies/ast-grep-language"
 ast-grep-lsp.path = "../../local_dependencies/ast-grep-lsp"
 
 ansi_term = "0.12"
 anyhow = "1.0"
 atty = "0.2.14"
-clap = { version = "4.3.11", features = ["derive"] }
+clap = { version = "4.3.12", features = ["derive"] }
 codespan-reporting = "0.11.1"
 crossterm = "0.26.1"
 ignore= { version = "0.4.20" }
 inquire = "0.6.2"
 num_cpus = "1.16.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.100"
+serde_json = "1.0.102"
 serde_yaml = "0.9.22"
 similar = { version = "2.2.1", features = ["inline"] }
 tokio = { version = "1", features = ["rt-multi-thread", "io-std"] }
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/config.rs` & `ast_grep_cli-0.9.0/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/error.rs` & `ast_grep_cli-0.9.0/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/lang.rs` & `ast_grep_cli-0.9.0/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/lib.rs` & `ast_grep_cli-0.9.0/crates/cli/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -152,19 +152,23 @@
     ok("run -p test -i");
     ok("run -p test --interactive dir");
     ok("run -p test -r Test dir");
     ok("run -p test -l rs --debug-query");
     ok("run -p test -l rs --color always");
     ok("run -p test -l rs --heading always");
     ok("run -p test dir1 dir2 dir3"); // multiple paths
+    ok("run -p testm -r restm -U"); // update all
+    ok("run -p testm -r restm --update-all"); // update all
     error("run test");
     error("run --debug-query test"); // missing lang
     error("run -r Test dir");
     error("run -p test -i --json dir"); // conflict
     error("run -p test -l rs -c always"); // no color shortcut
+    error("run -p test -U");
+    error("run -p test --update-all");
   }
 
   #[test]
   fn test_scan() {
     ok("scan");
     ok("scan dir");
     ok("scan -r test-rule.yml dir");
@@ -172,8 +176,18 @@
     ok("scan -c test-rule.yml");
     ok("scan --report-style short"); // conflict
     ok("scan dir1 dir2 dir3"); // multiple paths
     error("scan -i --json dir"); // conflict
     error("scan --report-style rich --json dir"); // conflict
     error("scan -r test.yml -c test.yml --json dir"); // conflict
   }
+
+  #[test]
+  fn test_test() {
+    ok("test");
+    ok("test -c sgconfig.yml");
+    ok("test --skip-snapshot-tests");
+    ok("test -U");
+    ok("test --update-all");
+    error("test --update-all --skip-snapshot-tests");
+  }
 }
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/lsp.rs` & `ast_grep_cli-0.9.0/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/new.rs` & `ast_grep_cli-0.9.0/crates/cli/src/new.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.9.0/crates/cli/src/print/colored_print.rs`

 * *Files 0% similar despite different names*

```diff
@@ -301,27 +301,27 @@
       styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     let lines = ret.lines().count();
     let mut num = merger.last_start_line;
     let width = (lines + num).to_string().chars().count();
-    write!(writer, "{num:>width$}│")?; // initial line num
+    write!(writer, "{num:>width$}:")?; // initial line num
     print_highlight(ret.lines(), width, &mut num, writer)?;
     writeln!(writer)?; // end match new line
                        //
     merger.conclude_match(&nm);
     ret = display.leading.to_string();
     styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   let lines = ret.lines().count();
   let mut num = merger.last_start_line;
   let width = (lines + num).to_string().chars().count();
-  write!(writer, "{num:>width$}│")?; // initial line num
+  write!(writer, "{num:>width$}:")?; // initial line num
   print_highlight(ret.lines(), width, &mut num, writer)?;
   writeln!(writer)?; // end match new line
   writeln!(writer)?; // end
   Ok(())
 }
 
 fn print_matches_with_prefix<'a, W: WriteColor>(
@@ -405,15 +405,15 @@
 ) -> Result<()> {
   if let Some(line) = lines.next() {
     write!(writer, "{line}")?;
   }
   for line in lines {
     writeln!(writer)?;
     *num += 1;
-    write!(writer, "{num:>width$}│{line}")?;
+    write!(writer, "{num:>width$}:{line}")?;
   }
   Ok(())
 }
 
 fn index_display(index: Option<usize>, style: Style, width: usize) -> impl Display {
   let index_str = match index {
     None => format!("{:width$}", ""),
@@ -454,15 +454,15 @@
         let (sign, s, em) = match change.tag() {
           ChangeTag::Delete => ("-", styles.delete, styles.delete_emphasis),
           ChangeTag::Insert => ("+", styles.insert, styles.insert_emphasis),
           ChangeTag::Equal => (" ", Style::new(), Style::new()),
         };
         write!(
           writer,
-          "{} {}│{}",
+          "{} {}:{}",
           index_display(change.old_index(), s, old_width),
           index_display(change.new_index(), s, new_width),
           s.paint(sign),
         )?;
         for (emphasized, value) in change.iter_strings_lossy() {
           if emphasized {
             write!(writer, "{}", em.paint(value))?;
@@ -689,15 +689,15 @@
       let printer = make_test_printer().heading(Heading::Always);
       let grep = SgLang::from(SupportLang::Tsx).ast_grep(source);
       let matches = grep.root().find_all(pattern);
       printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
       let expected: String = source
         .lines()
         .enumerate()
-        .map(|(i, l)| format!("{}│{l}\n", i + 1))
+        .map(|(i, l)| format!("{}:{l}\n", i + 1))
         .collect();
       // append heading to expected
       let output = format!("test.tsx\n{expected}\n");
       assert_eq!(get_text(&printer), output, "{note}");
     }
   }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.9.0/crates/cli/src/print/interactive_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.9.0/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.9.0/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/run.rs` & `ast_grep_cli-0.9.0/crates/cli/src/run.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
   interactive: bool,
 
   /// The paths to search. You can provide multiple paths separated by spaces.
   #[clap(value_parser, default_value = ".")]
   paths: Vec<PathBuf>,
 
   /// Apply all rewrite without confirmation if true.
-  #[clap(short = 'A', long)]
-  accept_all: bool,
+  #[clap(short = 'U', long, requires = "rewrite")]
+  update_all: bool,
 
   /// Output matches in structured JSON text useful for tools like jq.
   /// Conflicts with interactive.
   #[clap(long, conflicts_with = "interactive")]
   json: bool,
 
   /// Print the file name as heading before all matches of that file.
@@ -98,18 +98,18 @@
 // Every run will include Search or Replace
 // Search or Replace by arguments `pattern` and `rewrite` passed from CLI
 pub fn run_with_pattern(arg: RunArg) -> Result<()> {
   if arg.json {
     return run_pattern_with_printer(arg, JSONPrinter::stdout());
   }
   let printer = ColoredPrinter::stdout(arg.color).heading(arg.heading);
-  let interactive = arg.interactive || arg.accept_all;
+  let interactive = arg.interactive || arg.update_all;
   if interactive {
     let from_stdin = arg.stdin && is_from_stdin();
-    let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
+    let printer = InteractivePrinter::new(printer, arg.update_all, from_stdin)?;
     run_pattern_with_printer(arg, printer)
   } else {
     run_pattern_with_printer(arg, printer)
   }
 }
 
 fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
@@ -272,15 +272,15 @@
       no_ignore: vec![],
       stdin: false,
       interactive: false,
       lang: None,
       json: false,
       heading: Heading::Never,
       debug_query: false,
-      accept_all: false,
+      update_all: false,
       paths: vec![PathBuf::from(".")],
     };
     assert!(run_with_pattern(arg).is_ok())
   }
 
   #[test]
   fn test_run_with_specific_lang() {
@@ -290,14 +290,14 @@
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       lang: Some(SupportLang::Rust.into()),
       json: false,
       heading: Heading::Never,
       debug_query: false,
-      accept_all: false,
+      update_all: false,
       stdin: true,
       paths: vec![PathBuf::from(".")],
     };
     assert!(run_with_pattern(arg).is_ok())
   }
 }
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/scan.rs` & `ast_grep_cli-0.9.0/crates/cli/src/scan.rs`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
   /// Output matches in structured JSON text. This is useful for tools like jq.
   /// Conflicts with color and report-style.
   #[clap(long, conflicts_with = "color", conflicts_with = "report_style")]
   json: bool,
 
   /// Apply all rewrite without confirmation if true.
-  #[clap(short = 'A', long)]
-  accept_all: bool,
+  #[clap(short = 'U', long)]
+  update_all: bool,
 
   /// The paths to search. You can provide multiple paths separated by spaces.
   #[clap(value_parser, default_value = ".")]
   paths: Vec<PathBuf>,
 
   /// Do not respect ignore files. You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
@@ -68,18 +68,18 @@
 pub fn run_with_config(arg: ScanArg) -> Result<()> {
   register_custom_language(arg.config.clone());
   if arg.json {
     let printer = JSONPrinter::stdout();
     return run_scan(arg, printer);
   }
   let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
-  let interactive = arg.interactive || arg.accept_all;
+  let interactive = arg.interactive || arg.update_all;
   if interactive {
     let from_stdin = arg.stdin && is_from_stdin();
-    let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
+    let printer = InteractivePrinter::new(printer, arg.update_all, from_stdin)?;
     run_scan(arg, printer)
   } else {
     run_scan(arg, printer)
   }
 }
 
 fn run_scan<P: Printer + Sync>(arg: ScanArg, printer: P) -> Result<()> {
@@ -342,14 +342,14 @@
       config: Some(dir.path().join("sgconfig.yml")),
       rule: None,
       report_style: ReportStyle::Rich,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       json: false,
-      accept_all: false,
+      update_all: false,
       paths: vec![PathBuf::from(".")],
       stdin: false,
     };
     assert!(run_with_config(arg).is_ok());
   }
 }
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/utils.rs` & `ast_grep_cli-0.9.0/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/src/verify.rs` & `ast_grep_cli-0.9.0/crates/cli/src/verify.rs`

 * *Files 1% similar despite different names*

```diff
@@ -119,19 +119,21 @@
   #[clap(short, long)]
   test_dir: Option<PathBuf>,
   /// Specify the directory name storing snapshots. Default to __snapshots__.
   #[clap(long)]
   snapshot_dir: Option<PathBuf>,
   /// Only check if the test code is valid, without checking rule output.
   /// Turn it on when you want to ignore the output of rules.
-  #[clap(long)]
+  /// Conflicts with --update-all.
+  #[clap(long, conflicts_with = "update_all")]
   skip_snapshot_tests: bool,
   /// Update the content of all snapshots that have changed in test.
-  #[clap(short, long)]
-  update_snapshots: bool,
+  /// Conflicts with --skip-snapshot-tests.
+  #[clap(short = 'U', long)]
+  update_all: bool,
   /// start an interactive review to update snapshots selectively
   #[clap(short, long)]
   interactive: bool,
 }
 
 pub fn run_test_rule(arg: TestArg) -> Result<()> {
   register_custom_language(arg.config.clone());
@@ -141,15 +143,15 @@
       accepted_snapshots: HashMap::new(),
       should_accept_all: false,
     };
     run_test_rule_impl(arg, reporter)
   } else {
     let reporter = DefaultReporter {
       output: std::io::stdout(),
-      update_snapshots: arg.update_snapshots,
+      update_all: arg.update_all,
     };
     run_test_rule_impl(arg, reporter)
   }
 }
 
 fn parallel_collect<'a, T, R, F>(cases: &'a [T], filter_mapper: F) -> Vec<R>
 where
@@ -616,25 +618,25 @@
   }
   // continue
   Ok(true)
 }
 
 struct DefaultReporter<Output: Write> {
   output: Output,
-  update_snapshots: bool,
+  update_all: bool,
 }
 
 impl<O: Write> Reporter for DefaultReporter<O> {
   type Output = O;
 
   fn get_output(&mut self) -> &mut Self::Output {
     &mut self.output
   }
   fn collect_snapshot_action(&self) -> SnapshotAction {
-    if self.update_snapshots {
+    if self.update_all {
       SnapshotAction::AcceptAll
     } else {
       SnapshotAction::AcceptNone
     }
   }
 }
 
@@ -831,23 +833,23 @@
   }
 
   use codespan_reporting::term::termcolor::Buffer;
   #[test]
   fn test_run_verify() {
     let reporter = DefaultReporter {
       output: Buffer::no_color(),
-      update_snapshots: false,
+      update_all: false,
     };
     let arg = TestArg {
       config: None,
       interactive: false,
       skip_snapshot_tests: true,
       snapshot_dir: None,
       test_dir: None,
-      update_snapshots: false,
+      update_all: false,
     };
     // TODO
     assert!(run_test_rule_impl(arg, reporter).is_err());
   }
 
   #[test]
   fn test_verify_transform() {
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.9.0/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.9.0/crates/cli/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/tests/scan_test.rs` & `ast_grep_cli-0.9.0/crates/cli/tests/scan_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.9.0/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/pyproject.toml` & `ast_grep_cli-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.8.0/crates/cli/Cargo.lock` & `ast_grep_cli-0.9.0/crates/cli/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.18"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e37cfd5e7657ada45f742d6e99ca5788580b5c529dc78faf11ece6dc702656f"
-dependencies = [
- "memchr",
-]
-
-[[package]]
-name = "aho-corasick"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anes"
 version = "0.1.6"
@@ -88,30 +79,30 @@
 name = "anyhow"
 version = "1.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98161a4e3e2184da77bb14f02184cdd111e83bbbcc9979dfee3c44b9a85f5602"
 
 [[package]]
 name = "assert_cmd"
-version = "2.0.11"
+version = "2.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d6b683edf8d1119fe420a94f8a7e389239666aa72e65495d91c00462510151"
+checksum = "88903cb14723e4d4003335bb7f8a14f27691649105346a0f0957466c096adfe6"
 dependencies = [
  "anstyle",
  "bstr",
  "doc-comment",
  "predicates",
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -131,15 +122,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -147,38 +138,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -196,27 +187,27 @@
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -277,15 +268,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -314,21 +305,20 @@
 name = "bitflags"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d5dd14596c0e5b954530d0e6f1fd99b89c03e313aa2086e8da4303701a09e1cf"
 
 [[package]]
 name = "bstr"
-version = "1.1.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b45ea9b00a7b3f2988e9a65ad3917e62123c38dba709b666506207be96d1790b"
+checksum = "6798148dccfbff0fae41c7574d2fa8f1ef3492fba0face179de5d8d447d67b05"
 dependencies = [
  "memchr",
- "once_cell",
- "regex-automata 0.1.10",
+ "regex-automata",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -383,40 +373,40 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.11"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1640e5cc7fb47dbb8338fd471b105e7ed6c3cb2aeb00c2e067127ffd3764a05d"
+checksum = "3eab9e8ceb9afdade1ab3f0fd8dbce5b1b2f468ad653baf10e771781b2b67b73"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.11"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98c59138d527eeaf9b53f35a77fcc1fad9d883116070c63d5de1c7dc7b00c72b"
+checksum = "9f2763db829349bf00cfc06251268865ed4363b93a943174f638daf3ecdba2cd"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.2"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
+checksum = "54a9bb5758fc5dfe728d1019941681eccaf0cf8a4189b692a0ee2f2ecf90a050"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
@@ -751,19 +741,19 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "globset"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
+checksum = "1391ab1f92ffcc08911957149833e682aa3fe252b9f45f966d2ef972274c97df"
 dependencies = [
- "aho-corasick 0.7.18",
+ "aho-corasick",
  "bstr",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
@@ -1352,33 +1342,27 @@
 
 [[package]]
 name = "regex"
 version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
 dependencies = [
- "aho-corasick 1.0.1",
+ "aho-corasick",
  "memchr",
- "regex-automata 0.3.2",
+ "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
-
-[[package]]
-name = "regex-automata"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
 dependencies = [
- "aho-corasick 1.0.1",
+ "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.7.3"
@@ -1453,17 +1437,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.100"
+version = "1.0.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
+checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
```

### Comparing `ast_grep_cli-0.8.0/README.md` & `ast_grep_cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/LICENSE` & `ast_grep_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.8.0/PKG-INFO` & `ast_grep_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.8.0
+Version: 0.9.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.8.0 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
```

