# Comparing `tmp/ast_grep_cli-0.9.0.tar.gz` & `tmp/ast_grep_cli-0.9.1.tar.gz`

## Comparing `ast_grep_cli-0.9.0.tar` & `ast_grep_cli-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    11138 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15431 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123    10142 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2990 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     2041 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6357 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11610 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7730 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11369 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4312 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     5396 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10205 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22611 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7648 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     9061 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10644 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     7418 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24703 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      901 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1363 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/scan_test.rs
--rw-r--r--   0     1001      123     1025 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/pyproject.toml
--rw-r--r--   0     1001      123    59770 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4951 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/README.md
--rw-r--r--   0     1001      123     1077 2023-07-16 01:25:16.000000 ast_grep_cli-0.9.0/LICENSE
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1023 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123      858 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123      823 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     1192 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123     1216 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/kotlin.rs
+-rw-r--r--   0     1001      123    12673 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     3094 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     2043 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     1974 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     1646 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15493 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7940 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     5396 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10205 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    23910 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7648 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9061 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10644 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24703 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      901 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1363 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1025 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      123    59830 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-16 18:21:19.000000 ast_grep_cli-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.1/PKG-INFO
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.0"
+version= "0.9.1"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.9.1" , optional = true }
 thiserror= "1.0.43"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/node.rs`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
   pub(crate) doc: D,
 }
 
 impl<L: Language> Root<StrDoc<L>> {
   pub fn str(src: &str, lang: L) -> Self {
     Self::try_new(src, lang).expect("should parse")
   }
+  pub fn get_text(&self) -> &str {
+    &self.doc.src
+  }
 }
 
 impl<D: Doc> Root<D> {
   pub fn try_new(src: &str, lang: D::Lang) -> Result<Self, TSParseError> {
     let doc = D::from_str(src, lang);
     let inner = doc.parse(None)?;
     Ok(Self { inner, doc })
@@ -214,16 +217,16 @@
       matched: self.text(),
       leading: &self.root.doc.get_source().as_str()[leading..start],
       trailing: &self.root.doc.get_source().as_str()[end..=trailing],
       start_line: self.inner.start_position().row() as usize + 1,
     }
   }
 
-  pub fn root(&self) -> Self {
-    self.root.root()
+  pub fn root(&self) -> &Root<StrDoc<L>> {
+    self.root
   }
 }
 
 /**
  * Corresponds to inside/has/precedes/follows
  */
 impl<'r, D: Doc> Node<'r, D> {
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.0"
+version= "0.9.1"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
 
@@ -24,14 +24,15 @@
 tree-sitter-go = { version = "0.19.1", optional = true }
 tree-sitter-html = { version = "0.19.0", optional = true }
 tree-sitter-java = { version = "0.20.0", optional = true }
 tree-sitter-javascript = { version = "0.20.0", optional = true }
 tree-sitter-kotlin = { version = "0.2.11", optional = true }
 tree-sitter-lua = { version = "0.0.18", optional = true }
 tree-sitter-python = { version = "0.20.2", optional = true }
+tree-sitter-ruby = { version = "0.20.0", optional = true }
 tree-sitter-rust = { version = "0.20.3", optional = true }
 tree-sitter-scala = { version = "0.20.1", optional = true }
 tree-sitter-swift = { version = "0.3.6", optional = true }
 tree-sitter-thrift = { version = "0.5.0", optional = true }
 tree-sitter-typescript= { version = "0.20.2", optional = true }
 
 [features]
@@ -44,14 +45,15 @@
   "tree-sitter-go",
   "tree-sitter-html",
   "tree-sitter-java",
   "tree-sitter-javascript",
   "tree-sitter-kotlin",
   "tree-sitter-lua",
   "tree-sitter-python",
+  "tree-sitter-ruby",
   "tree-sitter-rust",
   "tree-sitter-scala",
   "tree-sitter-swift",
   "tree-sitter-thrift",
   "tree-sitter-typescript",
 ]
 default = ["builtin-parser"]
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 //! This module defines the supported programming languages for ast-grep.
+//!
 //! It provides a set of customized languages with expando_char / pre_process_pattern,
 //! and a set of stub languages without preprocessing.
 //! A rule of thumb: if your language does not accept identifiers like `$VAR`.
-//! You need to create a standalone file and implement expando_char / pre_process_pattern.
+//! You need use `impl_lang_expando!` macro and a standalone file for testing.
 //! Otherwise, you can define it as a stub language using `impl_lang!`.
+//! To see the full list of languages, visit `<https://ast-grep.github.io/reference/languages.html>`
 
 mod cpp;
 mod csharp;
 mod css;
 mod go;
+mod kotlin;
 mod parsers;
 mod python;
 mod rust;
 mod scala;
 
 use ast_grep_core::language::TSLanguage;
 use ast_grep_core::meta_var::MetaVariable;
@@ -22,44 +25,87 @@
 use std::fmt;
 use std::fmt::{Display, Formatter};
 use std::path::Path;
 use std::str::FromStr;
 
 pub use ast_grep_core::Language;
 
+/// this macro implements bare-bone methods for a language
 macro_rules! impl_lang {
   ($lang: ident, $func: ident) => {
     #[derive(Clone, Copy)]
     pub struct $lang;
     impl Language for $lang {
       fn get_ts_language(&self) -> TSLanguage {
         parsers::$func().into()
       }
     }
   };
 }
 
-// Customized Language with expando_char / pre_process_pattern
-pub use cpp::Cpp;
-pub use csharp::CSharp;
-pub use css::Css;
-pub use go::Go;
-pub use python::Python;
-pub use rust::Rust;
-pub use scala::Scala;
+/// this macro will implement expando_char and pre_process_pattern
+/// use this if your language does not accept $ as valid identifier char
+macro_rules! impl_lang_expando {
+  ($lang: ident, $func: ident, $char: expr) => {
+    #[derive(Clone, Copy)]
+    pub struct $lang;
+    impl ast_grep_core::language::Language for $lang {
+      fn get_ts_language(&self) -> ast_grep_core::language::TSLanguage {
+        $crate::parsers::$func().into()
+      }
+      fn expando_char(&self) -> char {
+        $char
+      }
+      fn pre_process_pattern<'q>(&self, query: &'q str) -> std::borrow::Cow<'q, str> {
+        // use stack buffer to reduce allocation
+        let mut buf = [0; 4];
+        let expando = self.expando_char().encode_utf8(&mut buf);
+        // TODO: use more precise replacement
+        let replaced = query.replace(self.meta_var_char(), expando);
+        std::borrow::Cow::Owned(replaced)
+      }
+    }
+  };
+}
+
+/* Customized Language with expando_char / pre_process_pattern */
+// https://en.cppreference.com/w/cpp/language/identifiers
+// Due to some issues in the tree-sitter parser, it is not possible to use
+// unicode literals in identifiers for C/C++ parsers
+impl_lang_expando!(C, language_c, '_');
+impl_lang_expando!(Cpp, language_cpp, '_');
+// https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/lexical-structure#643-identifiers
+// all letter number is accepted
+// https://www.compart.com/en/unicode/category/Nl
+impl_lang_expando!(CSharp, language_c_sharp, 'µ');
+// https://www.w3.org/TR/CSS21/grammar.html#scanner
+impl_lang_expando!(Css, language_css, '_');
+// we can use any Unicode code point categorized as "Letter"
+// https://go.dev/ref/spec#letter
+impl_lang_expando!(Go, language_go, 'µ');
+// https://github.com/fwcd/tree-sitter-kotlin/pull/93
+impl_lang_expando!(Kotlin, language_kotlin, '_');
+// we can use any char in unicode range [:XID_Start:]
+// https://docs.python.org/3/reference/lexical_analysis.html#identifiers
+// see also [PEP 3131](https://peps.python.org/pep-3131/) for further details.
+impl_lang_expando!(Python, language_python, 'µ');
+// https://github.com/tree-sitter/tree-sitter-ruby/blob/f257f3f57833d584050336921773738a3fd8ca22/grammar.js#L30C26-L30C78
+impl_lang_expando!(Ruby, language_ruby, 'µ');
+// we can use any char in unicode range [:XID_Start:]
+// https://doc.rust-lang.org/reference/identifiers.html
+impl_lang_expando!(Rust, language_rust, 'µ');
 
 // Stub Language without preprocessing
 // Language Name, tree-sitter-name, alias, extension
-impl_lang!(C, language_c);
 impl_lang!(Dart, language_dart);
 impl_lang!(Html, language_html);
 impl_lang!(Java, language_java);
 impl_lang!(JavaScript, language_javascript);
-impl_lang!(Kotlin, language_kotlin);
 impl_lang!(Lua, language_lua);
+impl_lang!(Scala, language_scala);
 impl_lang!(Swift, language_swift);
 impl_lang!(Thrift, language_thrift);
 impl_lang!(Tsx, language_tsx);
 impl_lang!(TypeScript, language_typescript);
 // See ripgrep for extensions
 // https://github.com/BurntSushi/ripgrep/blob/master/crates/ignore/src/default_types.rs
 
@@ -74,28 +120,29 @@
   Go,
   Html,
   Java,
   JavaScript,
   Kotlin,
   Lua,
   Python,
+  Ruby,
   Rust,
   Scala,
   Swift,
   Thrift,
   Tsx,
   TypeScript,
 }
 
 impl SupportLang {
   pub const fn all_langs() -> &'static [SupportLang] {
     use SupportLang::*;
     &[
-      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Rust, Scala,
-      Swift, Thrift, Tsx, TypeScript,
+      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Ruby, Rust,
+      Scala, Swift, Thrift, Tsx, TypeScript,
     ]
   }
 
   pub fn file_types(&self) -> Types {
     file_types(self)
   }
 }
@@ -143,14 +190,15 @@
     Go => &["go", "golang"],
     Html => &["html"],
     Java => &["java"],
     JavaScript => &["javascript", "js", "jsx"],
     Kotlin => &["kotlin", "kt"],
     Lua => &["lua"],
     Python => &["py", "python"],
+    Ruby => &["rb", "ruby"],
     Rust => &["rs", "rust"],
     Scala => &["scala"],
     Swift => &["swift"],
     Thrift => &["thrift"],
     TypeScript => &["ts", "typescript"],
     Tsx => &["tsx"],
   }
@@ -183,14 +231,15 @@
       S::Go => Go.$method($($pname,)*),
       S::Html => Html.$method($($pname,)*),
       S::Java => Java.$method($($pname,)*),
       S::JavaScript => JavaScript.$method($($pname,)*),
       S::Kotlin => Kotlin.$method($($pname,)*),
       S::Lua => Lua.$method($($pname,)*),
       S::Python => Python.$method($($pname,)*),
+      S::Ruby => Ruby.$method($($pname,)*),
       S::Rust => Rust.$method($($pname,)*),
       S::Scala => Scala.$method($($pname,)*),
       S::Swift => Swift.$method($($pname,)*),
       S::Thrift => Thrift.$method($($pname,)*),
       S::Tsx => Tsx.$method($($pname,)*),
       S::TypeScript => TypeScript.$method($($pname,)*),
     }
@@ -232,14 +281,15 @@
     Go => &["go"],
     Html => &["html", "htm", "xhtml"],
     Java => &["java"],
     JavaScript => &["cjs", "js", "mjs", "jsx"],
     Kotlin => &["kt", "ktm", "kts"],
     Lua => &["lua"],
     Python => &["py", "py3", "pyi", "bzl"],
+    Ruby => &["rb", "rbw", "gemspec"],
     Rust => &["rs"],
     Scala => &["scala", "sc", "sbt"],
     Swift => &["swift"],
     Thrift => &["thrift"],
     TypeScript => &["ts", "cts", "mts"],
     Tsx => &["tsx"],
   }
@@ -284,14 +334,15 @@
     L::Java => builder.select("java"),
     L::JavaScript => {
       add_custom_file_type(&mut builder, "myjs", &["*.js", "*.cjs", "*.jsx", "*.mjs"])
     }
     L::Kotlin => builder.select("kotlin"),
     L::Lua => builder.select("lua"),
     L::Python => builder.select("py"),
+    L::Ruby => builder.select("ruby"),
     L::Rust => builder.select("rust"),
     L::Scala => builder.select("scala"),
     L::Swift => builder.select("swift"),
     L::Thrift => builder.select("thrift"),
     L::Tsx => {
       builder
         .add("mytsx", "*.tsx")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
   }
   pub fn language_lua() -> TSLanguage {
     tree_sitter_lua::language().into()
   }
   pub fn language_python() -> TSLanguage {
     tree_sitter_python::language().into()
   }
+  pub fn language_ruby() -> TSLanguage {
+    tree_sitter_ruby::language().into()
+  }
   pub fn language_rust() -> TSLanguage {
     tree_sitter_rust::language().into()
   }
   pub fn language_scala() -> TSLanguage {
     tree_sitter_scala::language().into()
   }
   pub fn language_swift() -> TSLanguage {
@@ -92,14 +95,15 @@
     language_go,
     language_html,
     language_java,
     language_javascript,
     language_kotlin,
     language_lua,
     language_python,
+    language_ruby,
     language_rust,
     language_scala,
     language_swift,
     language_thrift,
     language_tsx,
     language_typescript,
   );
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/python.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,110 @@
-use crate::parsers::language_python;
-use ast_grep_core::language::{Language, TSLanguage};
-use std::borrow::Cow;
-
-// impl_lang!(Python, language_python);
-#[derive(Clone, Copy)]
-pub struct Python;
-impl Language for Python {
-  fn get_ts_language(&self) -> TSLanguage {
-    language_python()
-  }
-  // we can use any char in unicode range [:XID_Start:]
-  // https://docs.python.org/3/reference/lexical_analysis.html#identifiers
-  // see also [PEP 3131](https://peps.python.org/pep-3131/) for further details.
-  fn expando_char(&self) -> char {
-    'µ'
-  }
-  fn pre_process_pattern<'q>(&self, query: &'q str) -> Cow<'q, str> {
-    // use stack buffer to reduce allocation
-    let mut buf = [0; 4];
-    let expando = self.expando_char().encode_utf8(&mut buf);
-    // TODO: use more precise replacement
-    let replaced = query.replace(self.meta_var_char(), expando);
-    Cow::Owned(replaced)
-  }
-}
-
-#[cfg(test)]
-mod test {
-  use ast_grep_core::source::TSParseError;
-
-  use super::*;
-
-  fn test_match(query: &str, source: &str) {
-    use crate::test::test_match_lang;
-    test_match_lang(query, source, Python);
-  }
-
-  fn test_non_match(query: &str, source: &str) {
-    use crate::test::test_non_match_lang;
-    test_non_match_lang(query, source, Python);
-  }
-
-  #[test]
-  fn test_python_str() {
-    test_match("print($A)", "print(123)");
-    test_match("print('123')", "print('123')");
-    test_non_match("print('123')", "print('456')");
-    test_non_match("'123'", "'456'");
-  }
-
-  #[test]
-  fn test_python_pattern() {
-    test_match("$A = 0", "a = 0");
-    // A test case from https://peps.python.org/pep-0636/#appendix-a-quick-intro
-    test_match(
-      r#"
+#![cfg(test)]
+use ast_grep_core::source::TSParseError;
+
+use super::*;
+
+fn test_match(query: &str, source: &str) {
+  use crate::test::test_match_lang;
+  test_match_lang(query, source, Python);
+}
+
+fn test_non_match(query: &str, source: &str) {
+  use crate::test::test_non_match_lang;
+  test_non_match_lang(query, source, Python);
+}
+
+#[test]
+fn test_python_str() {
+  test_match("print($A)", "print(123)");
+  test_match("print('123')", "print('123')");
+  test_non_match("print('123')", "print('456')");
+  test_non_match("'123'", "'456'");
+}
+
+#[test]
+fn test_python_pattern() {
+  test_match("$A = 0", "a = 0");
+  // A test case from https://peps.python.org/pep-0636/#appendix-a-quick-intro
+  test_match(
+    r#"
 match $A:
-    case $B:
-        $C
-    case [$D(0, 0)]:
-        $E
-    case [$D($F, $G)]:
-        $H
-    case [$D(0, $I), $D(0, $J)]:
-        $K
-    case _:
-        $L
+  case $B:
+      $C
+  case [$D(0, 0)]:
+      $E
+  case [$D($F, $G)]:
+      $H
+  case [$D(0, $I), $D(0, $J)]:
+      $K
+  case _:
+      $L
 "#,
-      r#"
+    r#"
 match points:
-    case []:
-        print("No points")
-    case [Point(0, 0)]:
-        print("The origin")
-    case [Point(x, y)]:
-        print(f"Single point {x}, {y}")
-    case [Point(0, y1), Point(0, y2)]:
-        print(f"Two on the Y axis at {y1}, {y2}")
-    case _:
-        print("Something else")
+  case []:
+      print("No points")
+  case [Point(0, 0)]:
+      print("The origin")
+  case [Point(x, y)]:
+      print(f"Single point {x}, {y}")
+  case [Point(0, y1), Point(0, y2)]:
+      print(f"Two on the Y axis at {y1}, {y2}")
+  case _:
+      print("Something else")
 "#,
-    );
-  }
+  );
+}
+
+fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
+  use crate::test::test_replace_lang;
+  test_replace_lang(src, pattern, replacer, Python)
+}
 
-  fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
-    use crate::test::test_replace_lang;
-    test_replace_lang(src, pattern, replacer, Python)
-  }
-
-  #[test]
-  fn test_python_replace() -> Result<(), TSParseError> {
-    let ret = test_replace(
-      r#"
+#[test]
+fn test_python_replace() -> Result<(), TSParseError> {
+  let ret = test_replace(
+    r#"
 if flag:
-    a = value_pos
+  a = value_pos
 else:
-    a = value_neg"#,
-      r#"
+  a = value_neg"#,
+    r#"
 if $FLAG:
-    $VAR = $POS
+  $VAR = $POS
 else:
-    $VAR = $NEG
+  $VAR = $NEG
 "#,
-      "$VAR = $POS if $FLAG else $NEG",
-    )?;
-    assert_eq!(ret, "\na = value_pos if flag else value_neg");
+    "$VAR = $POS if $FLAG else $NEG",
+  )?;
+  assert_eq!(ret, "\na = value_pos if flag else value_neg");
 
-    let ret = test_replace(
-      r#"
+  let ret = test_replace(
+    r#"
 try:
-    f = open(file_path, "r")
-    file_content = f.read()
+  f = open(file_path, "r")
+  file_content = f.read()
 except:
-    pass
+  pass
 finally:
-    f.close()"#,
-      r#"
+  f.close()"#,
+    r#"
 try:
-    $A = open($B, $C)
-    $D = $A.read()
+  $A = open($B, $C)
+  $D = $A.read()
 except:
-    pass
+  pass
 finally:
-    $A.close()"#,
-      r#"
+  $A.close()"#,
+    r#"
 with open($B, $C) as $A:
-    $D = $A.open()"#,
-    )?;
-    assert_eq!(
-      ret,
-      r#"
+  $D = $A.open()"#,
+  )?;
+  assert_eq!(
+    ret,
+    r#"
 
 with open(file_path, "r") as f:
-    file_content = f.open()"#
-    );
-    Ok(())
-  }
+  file_content = f.open()"#
+  );
+  Ok(())
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,87 @@
-use crate::parsers::language_rust;
-use ast_grep_core::language::{Language, TSLanguage};
-use std::borrow::Cow;
-
-// impl_lang!(Rust, language_rust);
-#[derive(Clone, Copy)]
-pub struct Rust;
-impl Language for Rust {
-  fn get_ts_language(&self) -> TSLanguage {
-    language_rust()
-  }
-  // we can use any char in unicode range [:XID_Start:]
-  // https://doc.rust-lang.org/reference/identifiers.html
-  fn expando_char(&self) -> char {
-    'µ'
-  }
-  fn pre_process_pattern<'q>(&self, query: &'q str) -> Cow<'q, str> {
-    // use stack buffer to reduce allocation
-    let mut buf = [0; 4];
-    let expando = self.expando_char().encode_utf8(&mut buf);
-    // TODO: use more precise replacement
-    let replaced = query.replace(self.meta_var_char(), expando);
-    Cow::Owned(replaced)
-  }
-}
-
-#[cfg(test)]
-mod test {
-  use super::*;
-  use ast_grep_core::{source::TSParseError, Matcher, Pattern};
-
-  fn test_match(s1: &str, s2: &str) {
-    let pattern = Pattern::str(s1, Rust);
-    let cand = Rust.ast_grep(s2);
-    assert!(
-      pattern.find_node(cand.root()).is_some(),
-      "goal: {:?}, candidate: {}",
-      pattern,
-      cand.root().to_sexp(),
-    );
-  }
-
-  #[test]
-  fn test_rust_pattern() {
-    // fix #6
-    test_match("Some($A)", "fn test() { Some(123) }");
-    test_match(
-      "
+#![cfg(test)]
+use super::*;
+use ast_grep_core::{source::TSParseError, Matcher, Pattern};
+
+fn test_match(s1: &str, s2: &str) {
+  let pattern = Pattern::str(s1, Rust);
+  let cand = Rust.ast_grep(s2);
+  assert!(
+    pattern.find_node(cand.root()).is_some(),
+    "goal: {:?}, candidate: {}",
+    pattern,
+    cand.root().to_sexp(),
+  );
+}
+
+#[test]
+fn test_rust_pattern() {
+  // fix #6
+  test_match("Some($A)", "fn test() { Some(123) }");
+  test_match(
+    "
 match $A {
-    Some($B) => $B,
-    None => $C,
+  Some($B) => $B,
+  None => $C,
 }",
-      r#"fn test() {
+    r#"fn test() {
 patterns = match config.include.clone() {
-    Some(patterns) => patterns,
-    None => Vec::from([cwd
-        .join("**/*.toml")
-        .normalize()
-        .to_string_lossy()
-        .into_owned()]),
+  Some(patterns) => patterns,
+  None => Vec::from([cwd
+      .join("**/*.toml")
+      .normalize()
+      .to_string_lossy()
+      .into_owned()]),
 };
 }"#,
-    );
-  }
+  );
+}
+
+#[test]
+fn test_rust_wildcard_pattern() {
+  // fix #412
+  test_match("|$A, $B|", "let w = v.into_iter().reduce(|x, y| x + y);");
+  test_match("|$$A, $$B|", "let w = v.into_iter().reduce(|x, _| x + x);");
+  test_match("let ($$X, $$Y) = $$$T;", "let (_, y) = (1, 2);");
+}
+
+#[test]
+fn test_rust_spread_syntax() {
+  test_match(
+    "let ($X, $Y) = $$$T;",
+    "let (.., y) = (1,2,3,4,5,6,7,8,9,10);",
+  );
+  test_match(
+    "$C { $$$A, ..$B};",
+    r#"User {
+    username: String::from(name),
+    ..DEFAULT_USER
+  };"#,
+  );
+}
+
+fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
+  let mut source = Rust.ast_grep(src);
+  let replacer = Pattern::new(replacer, Rust);
+  assert!(source.replace(pattern, replacer)?);
+  Ok(source.generate())
+}
 
-  #[test]
-  fn test_rust_wildcard_pattern() {
-    // fix #412
-    test_match("|$A, $B|", "let w = v.into_iter().reduce(|x, y| x + y);");
-    test_match("|$$A, $$B|", "let w = v.into_iter().reduce(|x, _| x + x);");
-    test_match("let ($$X, $$Y) = $$$T;", "let (_, y) = (1, 2);");
-  }
-
-  #[test]
-  fn test_rust_spread_syntax() {
-    test_match(
-      "let ($X, $Y) = $$$T;",
-      "let (.., y) = (1,2,3,4,5,6,7,8,9,10);",
-    );
-    test_match(
-      "$C { $$$A, ..$B};",
-      r#"User { 
-      username: String::from(name),
-      ..DEFAULT_USER 
-    };"#,
-    );
-  }
-
-  fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
-    let mut source = Rust.ast_grep(src);
-    let replacer = Pattern::new(replacer, Rust);
-    assert!(source.replace(pattern, replacer)?);
-    Ok(source.generate())
-  }
-
-  #[test]
-  fn test_rust_replace() -> Result<(), TSParseError> {
-    let ret = test_replace("fn test() { Some(123) }", "Some($A)", "Ok($A)")?;
-    assert_eq!(ret, "fn test() { Ok(123) }");
-    let ret = test_replace(
-      r#"
+#[test]
+fn test_rust_replace() -> Result<(), TSParseError> {
+  let ret = test_replace("fn test() { Some(123) }", "Some($A)", "Ok($A)")?;
+  assert_eq!(ret, "fn test() { Ok(123) }");
+  let ret = test_replace(
+    r#"
 patterns = match config.include.clone() {
-    Some(patterns) => patterns,
-    None => 123,
+  Some(patterns) => patterns,
+  None => 123,
 }"#,
-      "match $A {
-    Some($B) => $B,
-    None => $C,
+    "match $A {
+  Some($B) => $B,
+  None => $C,
 }",
-      "$A.unwrap_or($C)",
-    )?;
-    assert_eq!(ret, "\npatterns = config.include.clone().unwrap_or(123)");
-    Ok(())
-  }
+    "$A.unwrap_or($C)",
+  )?;
+  assert_eq!(ret, "\npatterns = config.include.clone().unwrap_or(123)");
+  Ok(())
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,55 @@
+#![cfg(test)]
 //! Standalone Scala file to test syntax.
 //! Scala does not need special processing and can be a stub lang.
 //! But this file is created for testing Scala2 and Scala3.
 
-use crate::parsers::language_scala;
-use ast_grep_core::language::{Language, TSLanguage};
+use ast_grep_core::source::TSParseError;
 
-#[derive(Clone, Copy)]
-pub struct Scala;
-impl Language for Scala {
-  fn get_ts_language(&self) -> TSLanguage {
-    language_scala()
-  }
-  // no need to configure expando_char
-  // nor pre_process_pattern
-}
-
-#[cfg(test)]
-mod test {
-  use ast_grep_core::source::TSParseError;
-
-  use super::*;
-
-  fn test_match(query: &str, source: &str) {
-    use crate::test::test_match_lang;
-    test_match_lang(query, source, Scala);
-  }
-
-  fn test_non_match(query: &str, source: &str) {
-    use crate::test::test_non_match_lang;
-    test_non_match_lang(query, source, Scala);
-  }
-
-  #[test]
-  fn test_scala_str() {
-    test_match("println($A)", "println(123)");
-    test_match("println(\"123\")", "println(\"123\")");
-    test_non_match("println(\"123\")", "println(\"456\")");
-    test_non_match("\"123\"", "\"456\"");
-  }
-
-  #[test]
-  fn test_scala_pattern() {
-    test_match("val $A = 0", "val a = 0");
-    test_match("foo($VAR)", "foo(bar)");
-    test_match("type $A = String", "type Foo = String");
-    test_match("$A.filter(_ == $B)", "foo.filter(_ == bar)");
-    test_match("if ($A) $B else $C", "if (foo) bar else baz");
-    // Scala 3 syntax
-    test_match("if $A then $B else $C", "if foo then bar else baz");
-    test_non_match("if ($A) $B else $C", "if foo then bar else baz");
-    test_non_match("type $A = Int", "type Foo = String");
-  }
-
-  fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
-    use crate::test::test_replace_lang;
-    test_replace_lang(src, pattern, replacer, Scala)
-  }
-
-  #[test]
-  fn test_scala_replace() -> Result<(), TSParseError> {
-    let ret = test_replace(
-      "foo.filter(_ == bar)",
-      "$A.filter(_ == $B)",
-      "$A.filter(_ == baz)",
-    )?;
-    assert_eq!(ret, "foo.filter(_ == baz)");
-    Ok(())
-  }
+use super::*;
+
+fn test_match(query: &str, source: &str) {
+  use crate::test::test_match_lang;
+  test_match_lang(query, source, Scala);
+}
+
+fn test_non_match(query: &str, source: &str) {
+  use crate::test::test_non_match_lang;
+  test_non_match_lang(query, source, Scala);
+}
+
+#[test]
+fn test_scala_str() {
+  test_match("println($A)", "println(123)");
+  test_match("println(\"123\")", "println(\"123\")");
+  test_non_match("println(\"123\")", "println(\"456\")");
+  test_non_match("\"123\"", "\"456\"");
+}
+
+#[test]
+fn test_scala_pattern() {
+  test_match("val $A = 0", "val a = 0");
+  test_match("foo($VAR)", "foo(bar)");
+  test_match("type $A = String", "type Foo = String");
+  test_match("$A.filter(_ == $B)", "foo.filter(_ == bar)");
+  test_match("if ($A) $B else $C", "if (foo) bar else baz");
+  // Scala 3 syntax
+  test_match("if $A then $B else $C", "if foo then bar else baz");
+  test_non_match("if ($A) $B else $C", "if foo then bar else baz");
+  test_non_match("type $A = Int", "type Foo = String");
+}
+
+fn test_replace(src: &str, pattern: &str, replacer: &str) -> Result<String, TSParseError> {
+  use crate::test::test_replace_lang;
+  test_replace_lang(src, pattern, replacer, Scala)
+}
+
+#[test]
+fn test_scala_replace() -> Result<(), TSParseError> {
+  let ret = test_replace(
+    "foo.filter(_ == bar)",
+    "$A.filter(_ == $B)",
+    "$A.filter(_ == baz)",
+  )?;
+  assert_eq!(ret, "foo.filter(_ == baz)");
+  Ok(())
 }
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.0"
+version= "0.9.1"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 anyhow = "1.0"
 bit-set= { version = "0.5.3" }
 globset = "0.4.11"
 regex = { version = "1.9.1" , optional = true }
 serde= { version = "1.0", features = ["derive"] }
-serde_yaml = "0.9.22"
+serde_yaml = "0.9.23"
 thiserror= "1.0.43"
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.0"
+version= "0.9.1"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -251,24 +251,30 @@
   }
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
 
-  #[cfg(target_os = "macos")]
-  #[test]
-  fn test_load_parser() {
-    let (_lib, lang) = unsafe {
-      load_ts_language(
-        "../../benches/fixtures/json-mac.so".into(),
-        "tree_sitter_json".into(),
-      )
-      .unwrap()
-    };
+  fn test_load_parser(path: &str) {
+    let (_lib, lang) = unsafe { load_ts_language(path.into(), "tree_sitter_json".into()).unwrap() };
     let sg = lang.ast_grep("{\"a\": 123}");
     assert_eq!(
       sg.root().to_sexp(),
       "(document (object (pair key: (string (string_content)) value: (number))))"
     );
   }
+
+  #[test]
+  #[cfg(target_os = "macos")]
+  fn test_load_parser_mac() {
+    let path = "../../benches/fixtures/json-mac.so";
+    test_load_parser(path);
+  }
+
+  #[test]
+  #[cfg(target_os = "linux")]
+  fn test_load_parser_mac() {
+    let path = "../../benches/fixtures/json-linux.so";
+    test_load_parser(path);
+  }
 }
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.9.0"
+version= "0.9.1"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 ast-grep-config.path = "../ast-grep-config"
 
-dashmap = "5.4.0"
+dashmap = "5.5.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.102"
+serde_json = "1.0.103"
 tower-lsp = "0.19.0"
```

### Comparing `ast_grep_cli-0.9.0/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.9.1/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/Cargo.toml` & `ast_grep_cli-0.9.1/crates/cli/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.9.0"
+version= "0.9.1"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 # license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
@@ -38,11 +38,11 @@
 clap = { version = "4.3.12", features = ["derive"] }
 codespan-reporting = "0.11.1"
 crossterm = "0.26.1"
 ignore= { version = "0.4.20" }
 inquire = "0.6.2"
 num_cpus = "1.16.0"
 serde= { version = "1.0", features = ["derive"] }
-serde_json = "1.0.102"
-serde_yaml = "0.9.22"
+serde_json = "1.0.103"
+serde_yaml = "0.9.23"
 similar = { version = "2.2.1", features = ["inline"] }
 tokio = { version = "1", features = ["rt-multi-thread", "io-std"] }
```

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/config.rs` & `ast_grep_cli-0.9.1/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/error.rs` & `ast_grep_cli-0.9.1/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/lang.rs` & `ast_grep_cli-0.9.1/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/lib.rs` & `ast_grep_cli-0.9.1/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/lsp.rs` & `ast_grep_cli-0.9.1/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/new.rs` & `ast_grep_cli-0.9.1/crates/cli/src/new.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.9.1/crates/cli/src/print/colored_print.rs`

 * *Files 2% similar despite different names*

```diff
@@ -279,15 +279,15 @@
   styles: &PrintStyles,
   writer: &mut W,
 ) -> Result<()> {
   print_prelude(path, styles, writer)?;
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
-  let source = first_match.root().text();
+  let source = first_match.root().get_text();
   let display = first_match.display_context(0);
 
   let mut merger = MatchMerger::new(&first_match);
   let mut ret = display.leading.to_string();
   styles.push_matched_to_ret(&mut ret, &display.matched)?;
 
   for nm in matches {
@@ -330,15 +330,15 @@
   styles: &PrintStyles,
   writer: &mut W,
 ) -> Result<()> {
   let path = path.display();
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
-  let source = first_match.root().text();
+  let source = first_match.root().get_text();
   let display = first_match.display_context(0);
 
   let mut merger = MatchMerger::new(&first_match);
   let mut ret = display.leading.to_string();
   styles.push_matched_to_ret(&mut ret, &display.matched)?;
   for nm in matches {
     if merger.check_overlapping(&nm) {
@@ -375,29 +375,29 @@
   writer: &mut W,
 ) -> Result<()> {
   print_prelude(path, styles, writer)?;
   let Some(first_diff) = diffs.next() else {
     return Ok(());
   };
   let range = first_diff.node_match.range();
-  let source = first_diff.node_match.root().text();
+  let source = first_diff.node_match.root().get_text();
   let mut start = range.end;
   let mut new_str = format!("{}{}", &source[..range.start], first_diff.replacement);
   for diff in diffs {
     let range = diff.node_match.range();
     // skip overlapping diff
     if range.start < start {
       continue;
     }
     new_str.push_str(&source[start..range.start]);
     new_str.push_str(&diff.replacement);
     start = range.end;
   }
   new_str.push_str(&source[start..]);
-  print_diff(&source, &new_str, styles, writer)?;
+  print_diff(source, &new_str, styles, writer)?;
   Ok(())
 }
 
 fn print_highlight<'a, W: Write>(
   mut lines: impl Iterator<Item = &'a str>,
   width: usize,
   num: &mut usize,
@@ -640,14 +640,15 @@
   }
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
   use ast_grep_config::{from_yaml_string, GlobalRules};
+  use ast_grep_core::replacer::Fixer;
   use ast_grep_language::{Language, SupportLang};
   use codespan_reporting::term::termcolor::Buffer;
 
   fn make_test_printer() -> ColoredPrinter<Buffer> {
     ColoredPrinter::new(Buffer::no_color()).color(ColorChoice::Never)
   }
   fn get_text(printer: &ColoredPrinter<Buffer>) -> String {
@@ -748,13 +749,54 @@
       let text = get_text(&printer);
       assert!(text.contains("test.tsx"), "{note}");
       assert!(text.contains("note[test-id]"), "{note}");
       assert!(text.contains("test rule"), "{note}");
     }
   }
 
+  // source, pattern, rewrite, debug note
+  type DiffCase<'a> = (&'a str, &'a str, &'a str, &'a str);
+
+  const DIFF_CASES: &[DiffCase] = &[
+    ("let a = 123", "a", "b", "Simple match"),
+    (
+      "Some(1), Some(2), Some(3)",
+      "Some",
+      "Any",
+      "Same line match",
+    ),
+    (
+      "Some(1), Some(2)\nSome(3), Some(4)",
+      "Some",
+      "Any",
+      "Multiple line match",
+    ),
+    (
+      "import a from 'b';import a from 'b';",
+      "import a from 'b';",
+      "",
+      "immediate following but not overlapping",
+    ),
+    (
+      "\n\ntest",
+      "test",
+      "rest",
+      // https://github.com/ast-grep/ast-grep/issues/517
+      "leading empty space",
+    ),
+  ];
+
   #[test]
-  #[ignore]
   fn test_print_diffs() {
-    todo!()
+    for &(source, pattern, rewrite, note) in DIFF_CASES {
+      // heading is required for CI
+      let printer = make_test_printer().heading(Heading::Always);
+      let lang = SgLang::from(SupportLang::Tsx);
+      let fixer = Fixer::try_new(rewrite, &lang).expect("should work");
+      let grep = lang.ast_grep(source);
+      let matches = grep.root().find_all(pattern);
+      let diffs = matches.map(|n| Diff::generate(n, &pattern, &fixer));
+      printer.print_diffs(diffs, "test.tsx".as_ref()).unwrap();
+      assert!(get_text(&printer).contains(rewrite), "{note}");
+    }
   }
 }
```

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.9.1/crates/cli/src/print/interactive_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.9.1/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.9.1/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/run.rs` & `ast_grep_cli-0.9.1/crates/cli/src/run.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/scan.rs` & `ast_grep_cli-0.9.1/crates/cli/src/scan.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/utils.rs` & `ast_grep_cli-0.9.1/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/src/verify.rs` & `ast_grep_cli-0.9.1/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.9.1/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.9.1/crates/cli/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/tests/scan_test.rs` & `ast_grep_cli-0.9.1/crates/cli/tests/scan_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.9.1/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/pyproject.toml` & `ast_grep_cli-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.9.0"
+version = "0.9.1"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.9.0/crates/cli/Cargo.lock` & `ast_grep_cli-0.9.1/crates/cli/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -122,15 +122,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -138,38 +138,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.9.0"
+version = "0.9.1"
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
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -178,36 +178,37 @@
  "tree-sitter-go",
  "tree-sitter-html",
  "tree-sitter-java",
  "tree-sitter-javascript",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-python",
+ "tree-sitter-ruby",
  "tree-sitter-rust",
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.9.0"
+version = "0.9.1"
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
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -268,15 +269,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -569,20 +570,20 @@
 dependencies = [
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown 0.12.3",
+ "hashbrown",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "difflib"
@@ -760,20 +761,14 @@
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-
-[[package]]
-name = "hashbrown"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 
 [[package]]
 name = "heck"
 version = "0.4.0"
@@ -832,15 +827,15 @@
 [[package]]
 name = "indexmap"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.0",
+ "hashbrown",
 ]
 
 [[package]]
 name = "inquire"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c33e7c1ddeb15c9abcbfef6029d8e29f69b52b6d6c891031b88ed91b5065803b"
@@ -937,17 +932,17 @@
 name = "linux-raw-sys"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
 
 [[package]]
 name = "lock_api"
-version = "0.4.8"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f80bf5aacaf25cbfc8210d1cfb718f2bf3b11c4c54e5afe36c236853a8ec390"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1096,17 +1091,17 @@
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
@@ -1118,23 +1113,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.3"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.36.1",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4fd5641d01c8f18a23da7b6fe29298ff4b55afcccdf78973b24cf3175fee32e"
@@ -1329,17 +1324,17 @@
 checksum = "678054eb77286b51581ba43620cc911abf02758c91f93f479767aed0f90458b2"
 dependencies = [
  "rand_core 0.3.1",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.9.1"
@@ -1437,17 +1432,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.102"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1460,17 +1455,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.98",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.22"
+version = "0.9.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "452e67b9c20c37fa79df53201dc03839651086ed9bbe92b3ca585ca9fdaa7d85"
+checksum = "da6075b41c7e3b079e5f246eb6094a44850d3a4c25a67c581c80796c80134012"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -1663,17 +1658,17 @@
 name = "toml_datetime"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.12"
+version = "0.19.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c500344a19072298cd05a7224b3c0c629348b78692bf48466c5238656e315a78"
+checksum = "f8123f27e969974a3dfba720fdb560be359f57b44302d280ba72e76a74480e8a"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -1898,14 +1893,24 @@
 checksum = "dda114f58048f5059dcf158aff691dffb8e113e6d2b50d94263fd68711975287"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-ruby"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ac30cbb1560363ae76e1ccde543d6d99087421e228cc47afcec004b86bb711a"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-rust"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "797842733e252dc11ae5d403a18060bf337b822fc2ae5ddfaa6ff4d9cc20bda6"
 dependencies = [
  "cc",
  "tree-sitter",
@@ -2347,17 +2352,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.6"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
+checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xtask"
 version = "0.0.0"
```

### Comparing `ast_grep_cli-0.9.0/README.md` & `ast_grep_cli-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/LICENSE` & `ast_grep_cli-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.0/PKG-INFO` & `ast_grep_cli-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.9.0
+Version: 0.9.1
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
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.0 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.1 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
```

