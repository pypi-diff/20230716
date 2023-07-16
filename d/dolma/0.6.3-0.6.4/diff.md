# Comparing `tmp/dolma-0.6.3.tar.gz` & `tmp/dolma-0.6.4.tar.gz`

## Comparing `dolma-0.6.3.tar` & `dolma-0.6.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dolma-0.6.3/Cargo.toml
--rw-r--r--   0     1001      123      299 2023-07-11 03:40:04.000000 dolma-0.6.3/.cargo/config.toml
--rw-r--r--   0     1001      123      475 2023-07-11 03:40:04.000000 dolma-0.6.3/.flake8
--rw-r--r--   0     1001      123     3220 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     2194 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0     1001      123      691 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0     1001      123     1077 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0     1001      123      414 2023-07-11 03:40:04.000000 dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0     1001      123      549 2023-07-11 03:40:04.000000 dolma-0.6.3/.gitignore
--rw-r--r--   0     1001      123     1813 2023-07-11 03:40:04.000000 dolma-0.6.3/CITATION.cff
--rw-r--r--   0     1001      123    11357 2023-07-11 03:40:04.000000 dolma-0.6.3/LICENSE
--rw-r--r--   0     1001      123     2209 2023-07-11 03:40:04.000000 dolma-0.6.3/Makefile
--rw-r--r--   0     1001      123     3156 2023-07-11 03:40:04.000000 dolma-0.6.3/README.md
--rw-r--r--   0     1001      123     3217 2023-07-11 03:40:04.000000 dolma-0.6.3/pyproject.toml
--rw-r--r--   0     1001      123      736 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/__init__.py
--rw-r--r--   0     1001      123     4401 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/__init__.py
--rw-r--r--   0     1001      123     1494 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/__main__.py
--rw-r--r--   0     1001      123     4689 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/deduper.py
--rw-r--r--   0     1001      123     4589 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/mixer.py
--rw-r--r--   0     1001      123      473 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/shared.py
--rw-r--r--   0     1001      123     1957 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/cli/tagger.py
--rw-r--r--   0     1001      123      219 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/__init__.py
--rw-r--r--   0     1001      123     6111 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/data_types.py
--rw-r--r--   0     1001      123      337 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/errors.py
--rw-r--r--   0     1001      123     6482 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/ft_dataset.py
--rw-r--r--   0     1001      123     5557 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/ft_tagger.py
--rw-r--r--   0     1001      123    15587 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/parallel.py
--rw-r--r--   0     1001      123     6326 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/paths.py
--rw-r--r--   0     1001      123     1254 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/registry.py
--rw-r--r--   0     1001      123    11812 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/runtime.py
--rw-r--r--   0     1001      123     1032 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/taggers.py
--rw-r--r--   0     1001      123       42 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/trainer.py
--rw-r--r--   0     1001      123     2031 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/utils.py
--rw-r--r--   0     1001      123     9484 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/core/vizualizer.py
--rw-r--r--   0     1001      123     3777 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/data/naughty_words_en.txt
--rw-r--r--   0     1001      123        0 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/py.typed
--rw-r--r--   0     1001      123       72 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/__init__.py
--rw-r--r--   0     1001      123     3277 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/c4.py
--rw-r--r--   0     1001      123     6433 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/code.py
--rw-r--r--   0     1001      123     6857 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/gopher.py
--rw-r--r--   0     1001      123     1898 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/jigsaw.py
--rw-r--r--   0     1001      123     6391 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/language.py
--rw-r--r--   0     1001      123     4876 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/length.py
--rw-r--r--   0     1001      123    10494 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/pii.py
--rw-r--r--   0     1001      123      744 2023-07-11 03:40:04.000000 dolma-0.6.3/python/dolma/taggers/sampling.py
--rw-r--r--   0     1001      123      232 2023-07-11 03:40:04.000000 dolma-0.6.3/res/logo.md
--rw-r--r--   0     1001      123  1813803 2023-07-11 03:40:04.000000 dolma-0.6.3/res/logo.png
--rw-r--r--   0     1001      123     9277 2023-07-11 03:40:04.000000 dolma-0.6.3/src/bloom_filter.rs
--rw-r--r--   0     1001      123    13521 2023-07-11 03:40:04.000000 dolma-0.6.3/src/deduper.rs
--rw-r--r--   0     1001      123     1124 2023-07-11 03:40:04.000000 dolma-0.6.3/src/lib.rs
--rw-r--r--   0     1001      123     7515 2023-07-11 03:40:04.000000 dolma-0.6.3/src/mixer.rs
--rw-r--r--   0     1001      123    10738 2023-07-11 03:40:04.000000 dolma-0.6.3/src/s3_util.rs
--rw-r--r--   0     1001      123    27475 2023-07-11 03:40:04.000000 dolma-0.6.3/src/shard.rs
--rw-r--r--   0     1001      123      863 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/c4-cleaned.json
--rw-r--r--   0     1001      123      564 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/dedupe-by-url.json
--rw-r--r--   0     1001      123      553 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/dedupe-paragraphs.json
--rw-r--r--   0     1001      123      815 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/email-spans.json
--rw-r--r--   0     1001      123      799 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/filter-by-spans.json
--rw-r--r--   0     1001      123      749 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/mixer-local.json
--rw-r--r--   0     1001      123      792 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/mixer.json
--rw-r--r--   0     1001      123      716 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/config/paragraph-spans.json
--rw-r--r--   0     1001      123    25985 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/documents.json.gz
--rw-r--r--   0     1001      123      702 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/duplicate-paragraphs.json.gz
--rw-r--r--   0     1001      123      489 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/dedupe-by-url.json.gz
--rw-r--r--   0     1001      123      746 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/dedupe-paragraphs.json.gz
--rw-r--r--   0     1001      123    26447 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/email-spans.json.gz
--rw-r--r--   0     1001      123    14879 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/filter-by-spans.json.gz
--rw-r--r--   0     1001      123    15748 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/mixer.json.gz
--rw-r--r--   0     1001      123    26524 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/expected/remove-paragraphs.json.gz
--rw-r--r--   0     1001      123      614 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/pii-attributes.json.gz
--rw-r--r--   0     1001      123      570 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/sample-attributes.json.gz
--rw-r--r--   0     1001      123      543 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/data/toxicity-attributes.json.gz
--rw-r--r--   0     1001      123      352 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/__init__.py
--rw-r--r--   0     1001      123     3342 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_data_types.py
--rw-r--r--   0     1001      123      471 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_deduper.py
--rw-r--r--   0     1001      123      820 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_mixer.py
--rw-r--r--   0     1001      123     1395 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_omegaconf.py
--rw-r--r--   0     1001      123     2459 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_parallel.py
--rw-r--r--   0     1001      123     8972 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_paths.py
--rw-r--r--   0     1001      123     1846 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_runtime.py
--rw-r--r--   0     1001      123     9701 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_taggers.py
--rw-r--r--   0     1001      123     4043 2023-07-11 03:40:04.000000 dolma-0.6.3/tests/python/test_utils.py
--rw-r--r--   0     1001      123    57396 2023-07-11 03:40:16.000000 dolma-0.6.3/Cargo.lock
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 dolma-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dolma-0.6.4/Cargo.toml
+-rw-r--r--   0     1001      123      299 2023-07-16 00:59:05.000000 dolma-0.6.4/.cargo/config.toml
+-rw-r--r--   0     1001      123      475 2023-07-16 00:59:05.000000 dolma-0.6.4/.flake8
+-rw-r--r--   0     1001      123     5194 2023-07-16 00:59:05.000000 dolma-0.6.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     2194 2023-07-16 00:59:05.000000 dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      123      691 2023-07-16 00:59:05.000000 dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0     1001      123     1077 2023-07-16 00:59:05.000000 dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      123      414 2023-07-16 00:59:05.000000 dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0     1001      123      549 2023-07-16 00:59:05.000000 dolma-0.6.4/.gitignore
+-rw-r--r--   0     1001      123     1813 2023-07-16 00:59:05.000000 dolma-0.6.4/CITATION.cff
+-rw-r--r--   0     1001      123    11357 2023-07-16 00:59:05.000000 dolma-0.6.4/LICENSE
+-rw-r--r--   0     1001      123     1395 2023-07-16 00:59:05.000000 dolma-0.6.4/Makefile
+-rw-r--r--   0     1001      123     3150 2023-07-16 00:59:05.000000 dolma-0.6.4/README.md
+-rw-r--r--   0     1001      123     3296 2023-07-16 00:59:05.000000 dolma-0.6.4/pyproject.toml
+-rw-r--r--   0     1001      123     1019 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/__init__.py
+-rw-r--r--   0     1001      123     4401 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/__init__.py
+-rw-r--r--   0     1001      123     1494 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/__main__.py
+-rw-r--r--   0     1001      123     4689 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/deduper.py
+-rw-r--r--   0     1001      123     4589 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/mixer.py
+-rw-r--r--   0     1001      123      473 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/shared.py
+-rw-r--r--   0     1001      123     1957 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/cli/tagger.py
+-rw-r--r--   0     1001      123      219 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/__init__.py
+-rw-r--r--   0     1001      123     6111 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/data_types.py
+-rw-r--r--   0     1001      123      401 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/errors.py
+-rw-r--r--   0     1001      123     6482 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/ft_dataset.py
+-rw-r--r--   0     1001      123     5557 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/ft_tagger.py
+-rw-r--r--   0     1001      123    15575 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/parallel.py
+-rw-r--r--   0     1001      123     6326 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/paths.py
+-rw-r--r--   0     1001      123     1254 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/registry.py
+-rw-r--r--   0     1001      123    11812 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/runtime.py
+-rw-r--r--   0     1001      123     1032 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/taggers.py
+-rw-r--r--   0     1001      123       42 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/trainer.py
+-rw-r--r--   0     1001      123     2031 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/utils.py
+-rw-r--r--   0     1001      123     9515 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/core/vizualizer.py
+-rw-r--r--   0     1001      123     3777 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/data/naughty_words_en.txt
+-rw-r--r--   0     1001      123        0 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/py.typed
+-rw-r--r--   0     1001      123       72 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/__init__.py
+-rw-r--r--   0     1001      123     3277 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/c4.py
+-rw-r--r--   0     1001      123     6433 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/code.py
+-rw-r--r--   0     1001      123     6857 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/gopher.py
+-rw-r--r--   0     1001      123     1898 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/jigsaw.py
+-rw-r--r--   0     1001      123     6639 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/language.py
+-rw-r--r--   0     1001      123     4860 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/length.py
+-rw-r--r--   0     1001      123    10494 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/pii.py
+-rw-r--r--   0     1001      123      744 2023-07-16 00:59:05.000000 dolma-0.6.4/python/dolma/taggers/sampling.py
+-rw-r--r--   0     1001      123      232 2023-07-16 00:59:05.000000 dolma-0.6.4/res/logo.md
+-rw-r--r--   0     1001      123  1813803 2023-07-16 00:59:05.000000 dolma-0.6.4/res/logo.png
+-rw-r--r--   0     1001      123     9277 2023-07-16 00:59:05.000000 dolma-0.6.4/src/bloom_filter.rs
+-rw-r--r--   0     1001      123    11000 2023-07-16 00:59:05.000000 dolma-0.6.4/src/deduper.rs
+-rw-r--r--   0     1001      123     1498 2023-07-16 00:59:05.000000 dolma-0.6.4/src/lib.rs
+-rw-r--r--   0     1001      123     2499 2023-07-16 00:59:05.000000 dolma-0.6.4/src/mixer.rs
+-rw-r--r--   0     1001      123    10922 2023-07-16 00:59:05.000000 dolma-0.6.4/src/s3_util.rs
+-rw-r--r--   0     1001      123    28608 2023-07-16 00:59:05.000000 dolma-0.6.4/src/shard.rs
+-rw-r--r--   0     1001      123      863 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/c4-cleaned.json
+-rw-r--r--   0     1001      123      567 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/dedupe-by-url.json
+-rw-r--r--   0     1001      123      537 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/dedupe-paragraphs.json
+-rw-r--r--   0     1001      123      745 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/email-spans.json
+-rw-r--r--   0     1001      123      740 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/filter-by-spans.json
+-rw-r--r--   0     1001      123      713 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/mixer.json
+-rw-r--r--   0     1001      123      647 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/config/paragraph-spans.json
+-rw-r--r--   0     1001      123      489 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/dedupe-by-url.json.gz
+-rw-r--r--   0     1001      123      746 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/dedupe-paragraphs.json.gz
+-rw-r--r--   0     1001      123    26447 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/email-spans.json.gz
+-rw-r--r--   0     1001      123    14879 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/filter-by-spans.json.gz
+-rw-r--r--   0     1001      123    15748 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/mixer.json.gz
+-rw-r--r--   0     1001      123    26524 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/expected/remove-paragraphs.json.gz
+-rw-r--r--   0     1001      123      702 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz
+-rw-r--r--   0     1001      123      614 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/provided/attributes/pii/000.json.gz
+-rw-r--r--   0     1001      123      570 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/provided/attributes/sample/000.json.gz
+-rw-r--r--   0     1001      123      543 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/provided/attributes/toxicity/000.json.gz
+-rw-r--r--   0     1001      123    25985 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/data/provided/documents/000.json.gz
+-rw-r--r--   0     1001      123      352 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/__init__.py
+-rw-r--r--   0     1001      123     3321 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_data_types.py
+-rw-r--r--   0     1001      123     3349 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_deduper.py
+-rw-r--r--   0     1001      123     4486 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_mixer.py
+-rw-r--r--   0     1001      123     1395 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_omegaconf.py
+-rw-r--r--   0     1001      123     2459 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_parallel.py
+-rw-r--r--   0     1001      123     9316 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_paths.py
+-rw-r--r--   0     1001      123     1846 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_runtime.py
+-rw-r--r--   0     1001      123     9701 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_taggers.py
+-rw-r--r--   0     1001      123     3996 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/test_utils.py
+-rw-r--r--   0     1001      123     3772 2023-07-16 00:59:05.000000 dolma-0.6.4/tests/python/utils.py
+-rw-r--r--   0     1001      123    57396 2023-07-16 00:59:05.000000 dolma-0.6.4/Cargo.lock
+-rw-r--r--   0        0        0     5288 1970-01-01 00:00:00.000000 dolma-0.6.4/PKG-INFO
```

### Comparing `dolma-0.6.3/Cargo.toml` & `dolma-0.6.4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dolma"
-version = "0.6.3"
+version = "0.6.4"
 edition = "2021"
 license = "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dolma"
 crate-type = ["cdylib"]
```

### Comparing `dolma-0.6.3/.github/workflows/CI.yml` & `dolma-0.6.4/.github/workflows/CI.yml`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,92 @@
    workflow_dispatch:
 
 
 permissions:
   contents: read
 
 jobs:
+
+  tests:
+    runs-on: ubuntu-latest
+    env:
+      AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
+      AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
+    if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
+    strategy:
+      fail-fast: false
+      matrix:
+        python: [3.8]
+        task:
+          - name: Check Python style
+            run: |
+              isort --check .
+              black --check .
+
+          - name: Check Rust style
+            run: |
+              rustfmt --edition 2021 src/*.rs --check
+
+          - name: Lint
+            run: |
+              flake8 .
+
+          - name: Type check
+            run: |
+              mypy .
+
+          - name: Test
+            run: |
+              pytest -v --color=yes tests/python/
+
+    steps:
+      - name: Checkout repository
+        uses: actions/checkout@v1
+
+      - name: Setup system libraries
+        run:  |
+          sudo apt-get update
+          sudo apt-get install --yes --upgrade build-essential cmake protobuf-compiler libssl-dev glibc-source
+
+      - name: Install Rust
+        uses: actions-rs/toolchain@v1
+        with:
+          toolchain: stable
+          components: rustfmt
+
+      - name: Install Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python }}
+          architecture: "x64"
+          sccache: true
+
+      - name: Create a new Python environment & install maturin
+        run: |
+          python -m venv .venv
+          source .venv/bin/activate
+          pip install -U pip
+          pip install maturin
+
+      - name: Install dolma wheels
+        run: |
+          source .venv/bin/activate
+          maturin develop --extras=dev
+
+      - name: ${{ matrix.task.name }}
+        run: |
+          source .venv/bin/activate
+          ${{ matrix.task.run }}
+
+      - name: Clean up
+        if: always()
+        run: |
+          source .venv/bin/activate
+          pip uninstall -y dolma
+
   build-linux:
     runs-on: ubuntu-latest
     env:
       CC:   gcc-11
       CXX:  g++-11
     strategy:
       matrix:
```

### Comparing `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/bug_report.yml` & `dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/documentation.yml` & `dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/.github/workflows/ISSUE_TEMPLATE/feature_request.yml` & `dolma-0.6.4/.github/workflows/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/.gitignore` & `dolma-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/CITATION.cff` & `dolma-0.6.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/LICENSE` & `dolma-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/README.md` & `dolma-0.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # dolma
 
 *Data to feed OLMo's Appetite*
 
 
-<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256"></img>
+<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256">
 
 Data and tools for generating and inspecting OLMo pre-training data.
 
 To get started, install dolma using [pip](https://pypi.org/project/dolma/).
 
 ```shell
 pip install dolma
```

### Comparing `dolma-0.6.3/pyproject.toml` & `dolma-0.6.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [project]
 name = "dolma"
-version = "0.6.3"
+version = "0.6.4"
 description = "Data filters"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "requests",
-    "tqdm",
+    "anyascii>=0.3.2",
+    "blingfire==0.1.8",
     "boto3",
     "cached-path==1.3.4",
+    "detect-secrets==1.4.0",
+    # "fasttext==0.9.2",    # broken with new version of setuptools; using fasttext-wheel instead
+    "fasttext-wheel==0.9.2",
+    "fsspec",
     "msgspec>=0.14.2",
+    "nltk==3.8.1",
+    "omegaconf>=2.3.0",
     "presidio_analyzer==2.2.32",
     "pycld2==0.41",
-    # "pycld3==0.22",
-    "fasttext>=0.9.2",
+    # "pycld3==0.22",       # does not instlal correctly
+    "pyyaml",
+    "requests",
+    "rich",
+    "s3fs",
+    "smart-open",
     "tokenizers>=0.13.3,<1.0.0",
-    "omegaconf>=2.3.0",
-    "anyascii>=0.3.2",
+    "tqdm",
     "uniseg",
-    "pyyaml",
-    "blingfire==0.1.8",
-    "detect-secrets==1.4.0",
-    "rich>=10.12.0",
-    "smart-open>=6.3.0",
-    "nltk==3.8.1",
-    "fsspec>=2021.10.0",
-    "s3fs>=2021.10.0",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -99,15 +100,14 @@
     "pytest>=5.2",
     "ipython>=8.4.0",
     "autopep8>=1.7.0",
     "flake8>=5.0",
     "ipdb>=0.13.0",
     "flake8-pyi>=22.8.1",
     "Flake8-pyproject>=1.1.0",
-    "awscli>=1.16.0",
 ]
 [build-system]
 requires = [
     "maturin>=1.1,<2.0",
     "setuptools >= 61.0.0",
     "wheel"
 ]
```

### Comparing `dolma-0.6.3/python/dolma/cli/__init__.py` & `dolma-0.6.4/python/dolma/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/cli/__main__.py` & `dolma-0.6.4/python/dolma/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/cli/deduper.py` & `dolma-0.6.4/python/dolma/cli/deduper.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/cli/mixer.py` & `dolma-0.6.4/python/dolma/cli/mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/cli/tagger.py` & `dolma-0.6.4/python/dolma/cli/tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/data_types.py` & `dolma-0.6.4/python/dolma/core/data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/ft_dataset.py` & `dolma-0.6.4/python/dolma/core/ft_dataset.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/ft_tagger.py` & `dolma-0.6.4/python/dolma/core/ft_tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/parallel.py` & `dolma-0.6.4/python/dolma/core/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from queue import Queue
 from threading import Thread
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import smart_open
 import tqdm
 
-from .errors import DolmaFilterError, DolmaRetryableFailure
+from .errors import DolmaError, DolmaRetryableFailure
 from .paths import add_suffix, glob_path, make_relative, mkdir_p, sub_prefix
 
 METADATA_SUFFIX = ".done.txt"
 
 
 class BaseParallelProcessor:
     """A base parallel processor that supports applying the same process_single method to a list of files.
@@ -158,15 +158,15 @@
                 cls.process_single(
                     source_path=source_path, destination_path=destination_path, queue=queue, **kwargs
                 )
                 break
             except DolmaRetryableFailure as e:
                 retries_on_error -= 1
                 if retries_on_error == 0:
-                    raise DolmaFilterError from e
+                    raise DolmaError from e
 
         with smart_open.open(metadata_path, "wt") as f:
             f.write(datetime.now().isoformat())
 
     @classmethod
     def increment_progressbar(
         cls, queue: "Queue[Union[None, Tuple[int, ...]]]", /, **kwargs: int
```

### Comparing `dolma-0.6.3/python/dolma/core/paths.py` & `dolma-0.6.4/python/dolma/core/paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/registry.py` & `dolma-0.6.4/python/dolma/core/registry.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/runtime.py` & `dolma-0.6.4/python/dolma/core/runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/taggers.py` & `dolma-0.6.4/python/dolma/core/taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/utils.py` & `dolma-0.6.4/python/dolma/core/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/core/vizualizer.py` & `dolma-0.6.4/python/dolma/core/vizualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# flake8: noqa
+# type: ignore
+
 import argparse
 import json
 import os
 from contextlib import ExitStack
 from typing import Dict, List, Optional
 
 import msgspec
```

### Comparing `dolma-0.6.3/python/dolma/data/naughty_words_en.txt` & `dolma-0.6.4/python/dolma/data/naughty_words_en.txt`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/c4.py` & `dolma-0.6.4/python/dolma/taggers/c4.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/code.py` & `dolma-0.6.4/python/dolma/taggers/code.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/gopher.py` & `dolma-0.6.4/python/dolma/taggers/gopher.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/jigsaw.py` & `dolma-0.6.4/python/dolma/taggers/jigsaw.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/language.py` & `dolma-0.6.4/python/dolma/taggers/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,38 @@
 Filters.
 
 @kylel, @soldni
 
 """
 from typing import Iterable, List, Tuple
 
-import cld3
+try:
+    import cld3
+
+    CLD3_AVAILABLE = True
+except ImportError:
+    CLD3_AVAILABLE = False
+
 import pycld2 as cld2
 import regex
 from anyascii import anyascii
 
 from ..core.data_types import DocResult, Document, Span, TextSlice
 from ..core.ft_tagger import BaseFastTextTagger, Prediction
 from ..core.registry import TaggerRegistry
 from ..core.taggers import BaseTagger
 from ..core.utils import split_paragraphs
 
 
 @TaggerRegistry.add("cld3_en_doc_v2")
 class Cld3LanguageTagger(BaseTagger):
+    def __init__(self) -> None:
+        if not CLD3_AVAILABLE:
+            raise ImportError(f"cld3 is not install, cannot instantiate {self.__class__.__name__}")
+
     def _predict_text(self, text: str) -> Tuple[str, float]:
         pred = cld3.get_language(text)  # pyright: ignore
         score = pred.probability if pred.language == "en" else 0.0
         return "en", score
 
     def predict(self, doc: Document) -> DocResult:
         lang, score = self._predict_text(doc.text)
```

### Comparing `dolma-0.6.3/python/dolma/taggers/length.py` & `dolma-0.6.4/python/dolma/taggers/length.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         doc_results.spans.append(Span(start=0, end=len(doc.text), type="negative_document", score=neg_len))
         return doc_results
 
 
 @TaggerRegistry.add("olmo_pretokenizer_v1")
 class OlmoPreTokenizerV1(BaseTagger):
     def __init__(self) -> None:
-        self.pre_tokenizer = pre_tokenizers.Sequence(  # type: ignore
+        self.pre_tokenizer = pre_tokenizers.Sequence(
             [
                 # Split on all punctuation.
                 pre_tokenizers.Split(
                     pattern=Regex(" ?[[:punct:]]"),
                     behavior="isolated",
                     invert=False,
                 ),
```

### Comparing `dolma-0.6.3/python/dolma/taggers/pii.py` & `dolma-0.6.4/python/dolma/taggers/pii.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/python/dolma/taggers/sampling.py` & `dolma-0.6.4/python/dolma/taggers/sampling.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/res/logo.png` & `dolma-0.6.4/res/logo.png`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/src/bloom_filter.rs` & `dolma-0.6.4/src/bloom_filter.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/src/deduper.rs` & `dolma-0.6.4/src/deduper.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 use std::collections::VecDeque;
 use std::fs::OpenOptions;
 use std::io;
 use std::io::{BufRead, BufReader, BufWriter, Write};
 use std::path::PathBuf;
-use std::process;
 use std::sync::atomic::{AtomicU32, Ordering};
 use std::sync::Arc;
 
 use flate2::read::MultiGzDecoder;
 use flate2::write::GzEncoder;
 use flate2::Compression;
 use serde_json::{json, Value};
 use threadpool::ThreadPool;
 
 use crate::bloom_filter::BloomFilter;
 use crate::s3_util;
 use crate::shard::shard_config::WorkDirConfig;
-use crate::shard::FileCache;
+use crate::shard::{find_objects_matching_patterns, FileCache};
 
 use deduper_config::*;
 
-pub fn run(config: DeduperConfig) {
-    assert!(
-        config.dedupe.paragraphs.is_some() ^ config.dedupe.documents.is_some(),
-        "Must dedupe either paragraphs or documents"
-    );
-
-    let s3_client = s3_util::new_client(None).unwrap();
-
+pub fn run(config: DeduperConfig) -> Result<u32, u32> {
     let bloom_filter = BloomFilter::initialize(&config.bloom_filter).unwrap();
     let bloom_filter = Arc::new(bloom_filter);
 
-    let paths = s3_util::find_objects_matching_patterns(&s3_client, &config.documents)
+    let paths = find_objects_matching_patterns(&config.documents)
         .unwrap()
         .clone();
 
+    if !(config.dedupe.paragraphs.is_some() ^ config.dedupe.documents.is_some()) {
+        log::error!("Must dedupe either paragraphs or documents");
+        return Err(paths.len() as u32);
+    }
+
     let threadpool = ThreadPool::new(config.processes);
     let failed_shard_count = AtomicU32::new(0);
     let failed_shard_count_ref = Arc::new(failed_shard_count);
     for p in paths {
         let path = p.clone();
         let work_dirs = config.work_dir.clone();
         let dedupe = config.dedupe.clone();
@@ -57,20 +54,25 @@
     }
     threadpool.join();
 
     let bloom_filter_file = PathBuf::from(&config.bloom_filter.file);
     log::info!("Writing bloom filter to {:?}...", config.bloom_filter.file);
     bloom_filter.write_to_file(&bloom_filter_file).unwrap();
     log::info!("Bloom filter written.");
+
     let failure_count = failed_shard_count_ref.fetch_add(0, Ordering::Relaxed);
-    if failure_count > 0 {
-        log::error!("{} shards failed to process.", failure_count);
-        process::exit(1);
-    } else {
-        log::info!("Done!");
+    match failure_count {
+        0 => {
+            log::info!("Done!");
+            return Ok(failure_count);
+        }
+        _ => {
+            log::error!("{} shards failed to process.", failure_count);
+            return Err(failure_count);
+        }
     }
 }
 
 // Write attributes for the documents in the given file:
 // For doc-level deduping, check the Bloom filter for existence of the configured key and set the configured attribute to true.
 // For paragraph-level deduping, check the Bloom filter for existence of a paragraph in the text and add a span to the configured attribute.
 fn write_attributes(
@@ -290,93 +292,7 @@
         }
         pub fn parse_from_string(s: &str) -> Result<DeduperConfig, io::Error> {
             let config: DeduperConfig = serde_json::from_str(s)?;
             Ok(config)
         }
     }
 }
-
-#[cfg(test)]
-mod test {
-    use std::fs::OpenOptions;
-    use std::io;
-    use std::io::{BufRead, BufReader};
-
-    use flate2::read::MultiGzDecoder;
-
-    use crate::s3_util;
-
-    use super::*;
-
-    fn compare_contents(expected: &str, actual: &str) {
-        let expected_lines = BufReader::new(MultiGzDecoder::new(
-            OpenOptions::new()
-                .read(true)
-                .write(false)
-                .create(false)
-                .open(expected)
-                .unwrap(),
-        ))
-        .lines()
-        .collect::<Vec<Result<String, io::Error>>>();
-        let actual_lines = BufReader::new(MultiGzDecoder::new(
-            OpenOptions::new()
-                .read(true)
-                .write(false)
-                .create(false)
-                .open(actual)
-                .unwrap(),
-        ))
-        .lines()
-        .collect::<Vec<Result<String, io::Error>>>();
-
-        assert_eq!(
-            expected_lines.len(),
-            actual_lines.len(),
-            "Wrong number of output documents"
-        );
-
-        for (actual, expected) in std::iter::zip(expected_lines, actual_lines) {
-            let actual = actual.unwrap();
-            let expected = expected.unwrap();
-            assert_eq!(actual, expected);
-        }
-    }
-
-    #[test]
-    fn test_dedupe_by_url() -> Result<(), io::Error> {
-        let config = DeduperConfig::read_from_file("tests/config/dedupe-by-url.json").unwrap();
-        run(config.clone());
-
-        let cache = FileCache {
-            s3_client: Box::new(s3_util::new_client(None)?),
-            work: config.work_dir.clone(),
-        };
-
-        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_by_url/head/0000.json.gz")?;
-
-        compare_contents(
-            "tests/data/expected/dedupe-by-url.json.gz",
-            &local_output_file.display().to_string(),
-        );
-        Ok(())
-    }
-
-    #[test]
-    fn test_dedupe_paragraphs() -> Result<(), io::Error> {
-        let config = DeduperConfig::read_from_file("tests/config/dedupe-paragraphs.json").unwrap();
-        run(config.clone());
-
-        let cache = FileCache {
-            s3_client: Box::new(s3_util::new_client(None)?),
-            work: config.work_dir.clone(),
-        };
-
-        let local_output_file = cache.prepare_input("s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/attributes/dedupe_paragraphs/head/0000.json.gz")?;
-
-        compare_contents(
-            "tests/data/expected/dedupe-paragraphs.json.gz",
-            &local_output_file.display().to_string(),
-        );
-        Ok(())
-    }
-}
```

### Comparing `dolma-0.6.3/src/lib.rs` & `dolma-0.6.4/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use pyo3::exceptions;
 use pyo3::prelude::*;
 
 pub mod bloom_filter;
 pub mod deduper;
 pub mod mixer;
 pub mod s3_util;
 pub mod shard;
@@ -9,23 +10,35 @@
 use crate::deduper::deduper_config::DeduperConfig;
 use crate::mixer::mixer_config::MixerConfig;
 use std::env;
 
 #[pyfunction]
 fn deduper_entrypoint(config_str: &str) -> PyResult<()> {
     let config: DeduperConfig = DeduperConfig::parse_from_string(config_str).unwrap();
-    deduper::run(config);
-    Ok(())
+
+    match deduper::run(config) {
+        Ok(_) => Ok(()),
+        Err(cnt) => Err(exceptions::PyRuntimeError::new_err(format!(
+            "Failed with {} errors",
+            cnt
+        ))),
+    }
 }
 
 #[pyfunction]
 fn mixer_entrypoint(config_str: &str) -> PyResult<()> {
+    //Result<u32, PyErr> {
     let config: MixerConfig = MixerConfig::parse_from_string(config_str).unwrap();
-    mixer::run(config);
-    Ok(())
+    match mixer::run(config) {
+        Ok(_) => Ok(()),
+        Err(cnt) => Err(exceptions::PyRuntimeError::new_err(format!(
+            "Failed with {} errors",
+            cnt
+        ))),
+    }
 }
 
 // A Python module implemented in Rust. The name of this function must match
 // the `lib.name` setting in the `Cargo.toml`, else Python will not be able to
 // import the module.
 #[pymodule]
 fn dolma(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `dolma-0.6.3/src/s3_util.rs` & `dolma-0.6.4/src/s3_util.rs`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,20 @@
             if index < pattern.len() - 1 {
                 suffix = Some(pattern[index + 2..].to_string());
             }
         }
         let mut has_more = true;
         let mut token: Option<String> = None;
         while has_more {
-            let (bucket, key) = split_url(&prefix).unwrap();
+            let (bucket, key) = match split_url(&prefix) {
+                Ok((bucket, key)) => (bucket, key),
+                Err(e) => {
+                    return Err(io::Error::new(io::ErrorKind::Other, e));
+                }
+            };
             let resp = if token.is_some() {
                 log::info!("Listing objects in bucket={}, prefix={}", bucket, key);
                 rt.block_on(
                     s3_client
                         .list_objects_v2()
                         .bucket(bucket)
                         .prefix(key)
```

### Comparing `dolma-0.6.3/src/shard.rs` & `dolma-0.6.4/src/shard.rs`

 * *Files 2% similar despite different names*

```diff
@@ -190,19 +190,41 @@
                     let mut data: Value = serde_json::from_str(&line)?;
                     let mut attrs = serde_json::Map::new();
                     let mut attr_reader_index = 0;
                     for (_, attr_reader) in local_attr_readers.iter_mut() {
                         match attr_reader.next() {
                             Some(Ok(line)) => {
                                 let attr_data: Value = serde_json::from_str(&line)?;
-                                assert_eq!(
-                                    attr_data["id"], data["id"],
-                                    "Mismatched ids for line {} of {}: {} != {}",
-                                    line_number, &input_path.doc_path, attr_data["id"], data["id"]
-                                );
+
+                                // raise an error if there if the id from attributes and the id from
+                                // the data do not match
+                                if attr_data["id"] != data["id"] {
+                                    return Err(io::Error::new(
+                                        io::ErrorKind::Other,
+                                        format!(
+                                            "Mismatched ids for line {} of {}: {} != {}",
+                                            line_number,
+                                            &input_path.doc_path,
+                                            attr_data["id"],
+                                            data["id"]
+                                        ),
+                                    ));
+                                }
+
+                                // raise an error if there is no attribute key
+                                if !attr_data["attributes"].is_object() {
+                                    return Err(io::Error::new(
+                                        io::ErrorKind::Other,
+                                        format!(
+                                            "Missing attributes for line {} of {}",
+                                            line_number, &input_path.doc_path
+                                        ),
+                                    ));
+                                }
+
                                 for (k, v) in attr_data["attributes"].as_object().unwrap().iter() {
                                     attrs.insert(k.clone(), v.clone());
                                 }
                             }
                             Some(Err(e)) => {
                                 if attr_reader_failure_counts[attr_reader_index] == 0 {
                                     log::warn!(
@@ -577,15 +599,15 @@
 
 pub fn find_objects_matching_patterns(patterns: &Vec<String>) -> Result<Vec<String>, io::Error> {
     let s3_url_count = patterns.iter().filter(|p| p.starts_with("s3://")).count();
     if s3_url_count == 0 {
         let mut matches = Vec::new();
         for pattern in patterns.iter() {
             for entry in
-            glob(pattern).expect(format! {"Invalid file pattern: {}", pattern.clone()}.as_str())
+                glob(pattern).expect(format! {"Invalid file pattern: {}", pattern.clone()}.as_str())
             {
                 matches.push(entry.unwrap().to_str().unwrap().to_owned());
             }
         }
         Ok(matches)
     } else if s3_url_count == patterns.len() {
         let s3_client = s3_util::new_client(None)?;
```

### Comparing `dolma-0.6.3/tests/config/c4-cleaned.json` & `dolma-0.6.4/tests/config/c4-cleaned.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/config/dedupe-paragraphs.json` & `dolma-0.6.4/tests/config/filter-by-spans.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2916666666666667%*

 * *Differences: {"'streams'": "[OrderedDict([('name', 'filter-by-spans-test'), ('documents', "*

 * *              "['tests/data/provided/documents/000.json.gz']), ('output', OrderedDict([('path', "*

 * *              "'tests/work/output/filter-by-spans'), ('max_size_in_bytes', 100000), "*

 * *              "('discard_fields', ['attributes', 'metadata', 'added', 'created'])])), "*

 * *              "('attributes', ['sample']), ('filter', OrderedDict([('include', "*

 * *              "['$.attributes[?(@.sample__random_number_v1__random[0][2] < 0.5)] […]*

```diff
@@ -1,23 +1,36 @@
 {
-    "bloom_filter": {
-        "desired_false_positive_rate": 0.001,
-        "estimated_doc_count": 1000,
-        "file": "tests/work/para_bloom_filter.bin",
-        "read_only": false,
-        "size_in_bytes": 0
-    },
-    "dedupe": {
-        "name": "dedupe_paragraphs",
-        "paragraphs": {
-            "attribute_name": "bff_duplicate_paragraph_spans"
+    "processes": 1,
+    "streams": [
+        {
+            "attributes": [
+                "sample"
+            ],
+            "documents": [
+                "tests/data/provided/documents/000.json.gz"
+            ],
+            "filter": {
+                "exclude": [
+                    "$.attributes[?(@.dummy && @.dummy[0] && @.dummy[0][2] > 0.5)]"
+                ],
+                "include": [
+                    "$.attributes[?(@.sample__random_number_v1__random[0][2] < 0.5)]"
+                ]
+            },
+            "name": "filter-by-spans-test",
+            "output": {
+                "discard_fields": [
+                    "attributes",
+                    "metadata",
+                    "added",
+                    "created"
+                ],
+                "max_size_in_bytes": 100000,
+                "path": "tests/work/output/filter-by-spans"
+            }
         }
-    },
-    "documents": [
-        "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/*/0000.json.gz"
     ],
-    "processes": 1,
     "work_dir": {
-        "input": "tests/work/para/input",
-        "output": "tests/work/para/output"
+        "input": "tests/work/temp/filter-by-spans/input",
+        "output": "tests/work/temp/filter-by-spans/output"
     }
 }
```

### Comparing `dolma-0.6.3/tests/config/email-spans.json` & `dolma-0.6.4/tests/config/email-spans.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8791666666666668%*

 * *Differences: {"'streams'": "{0: {'name': 'email-spans', 'documents': "*

 * *              "['tests/data/provided/documents/*.json.gz'], 'output': {'path': "*

 * *              "'tests/work/output/email-spans'}}}",*

 * * "'work_dir'": "{'input': 'tests/work/temp/email-spans/input', 'output': "*

 * *               "'tests/work/temp/email-spans/output'}"}*

```diff
@@ -2,20 +2,20 @@
     "processes": 1,
     "streams": [
         {
             "attributes": [
                 "pii"
             ],
             "documents": [
-                "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/*/0000.json.gz"
+                "tests/data/provided/documents/*.json.gz"
             ],
-            "name": "email-spans-test",
+            "name": "email-spans",
             "output": {
                 "max_size_in_bytes": 100000,
-                "path": "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head"
+                "path": "tests/work/output/email-spans"
             },
             "span_replacement": [
                 {
                     "min_score": 0.5,
                     "replacement": "[B-EMAIL]{}[E-EMAIL]",
                     "span": "$.attributes.pii.email"
                 },
@@ -24,11 +24,11 @@
                     "replacement": "",
                     "span": "$.attributes.pii.company_name"
                 }
             ]
         }
     ],
     "work_dir": {
-        "input": "tests/work/email-spans/input",
-        "output": "tests/work/email-spans/output"
+        "input": "tests/work/temp/email-spans/input",
+        "output": "tests/work/temp/email-spans/output"
     }
 }
```

### Comparing `dolma-0.6.3/tests/config/mixer-local.json` & `dolma-0.6.4/tests/config/dedupe-paragraphs.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2916666666666667%*

 * *Differences: {"'bloom_filter'": "OrderedDict([('file', 'tests/work/para_bloom_filter.bin'), ('size_in_bytes', "*

 * *                   "0), ('read_only', False), ('estimated_doc_count', 1000), "*

 * *                   "('desired_false_positive_rate', 0.001)])",*

 * * "'dedupe'": "OrderedDict([('name', 'dedupe_paragraphs'), ('paragraphs', "*

 * *             "OrderedDict([('attribute_name', 'bff_duplicate_paragraph_spans')]))])",*

 * * "'documents'": "['tests/data/provided/doc*/000.json.gz']",*

 * * "'work_dir'": "{'input': 'tests/work/temp/dedupe- […]*

```diff
@@ -1,33 +1,23 @@
 {
-    "processes": 1,
-    "streams": [
-        {
-            "attributes": [
-                "pii",
-                "toxicity"
-            ],
-            "documents": [
-                "tests/work/mixer-local/input/documents/*/0000.json.gz"
-            ],
-            "filter": {
-                "exclude": [
-                    "$.metadata[?(@.length < 500)]",
-                    "$.attributes[?(@.pii.too_much_pii == true)]",
-                    "$.attributes[?(@.toxicity > 0.8)]"
-                ],
-                "include": [
-                    "$.metadata[?(@.length < 10000)]"
-                ]
-            },
-            "name": "mixer-local-test",
-            "output": {
-                "max_size_in_bytes": 100000,
-                "path": "tests/work/mixer-local/output"
-            }
+    "bloom_filter": {
+        "desired_false_positive_rate": 0.001,
+        "estimated_doc_count": 1000,
+        "file": "tests/work/para_bloom_filter.bin",
+        "read_only": false,
+        "size_in_bytes": 0
+    },
+    "dedupe": {
+        "name": "dedupe_paragraphs",
+        "paragraphs": {
+            "attribute_name": "bff_duplicate_paragraph_spans"
         }
+    },
+    "documents": [
+        "tests/data/provided/doc*/000.json.gz"
     ],
+    "processes": 1,
     "work_dir": {
-        "input": "tests/work/mixer-local/input",
-        "output": "tests/work/mixer-local/output"
+        "input": "tests/work/temp/dedupe-para/input",
+        "output": "tests/work/temp/dedupe-para/output"
     }
 }
```

### Comparing `dolma-0.6.3/tests/config/paragraph-spans.json` & `dolma-0.6.4/tests/config/paragraph-spans.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8958333333333334%*

 * *Differences: {"'streams'": "{0: {'documents': ['tests/data/provided/documents/*'], 'output': {'path': "*

 * *              "'tests/work/output/paragraph-spans'}}}",*

 * * "'work_dir'": "{'input': 'tests/work/temp/paragraph-spans/input', 'output': "*

 * *               "'tests/work/temp/paragraph-spans/output'}"}*

```diff
@@ -2,28 +2,28 @@
     "processes": 1,
     "streams": [
         {
             "attributes": [
                 "duplicate_paragraphs"
             ],
             "documents": [
-                "s3://ai2-llm/pretraining-data/tests/mixer/inputs/v0/documents/*/0000.json.gz"
+                "tests/data/provided/documents/*"
             ],
             "name": "paragraph-spans-test",
             "output": {
                 "max_size_in_bytes": 100000,
-                "path": "s3://ai2-llm/pretraining-data/tests/mixer/outputs/v1/documents/head"
+                "path": "tests/work/output/paragraph-spans"
             },
             "span_replacement": [
                 {
                     "min_score": 0.5,
                     "replacement": "",
                     "span": "$.attributes.bff_duplicate_paragraph_spans"
                 }
             ]
         }
     ],
     "work_dir": {
-        "input": "tests/work/paragraph-spans/input",
-        "output": "tests/work/paragraph-spans/output"
+        "input": "tests/work/temp/paragraph-spans/input",
+        "output": "tests/work/temp/paragraph-spans/output"
     }
 }
```

### Comparing `dolma-0.6.3/tests/data/documents.json.gz` & `dolma-0.6.4/tests/data/provided/documents/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/duplicate-paragraphs.json.gz` & `dolma-0.6.4/tests/data/provided/attributes/duplicate_paragraphs/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/expected/dedupe-paragraphs.json.gz` & `dolma-0.6.4/tests/data/expected/dedupe-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/expected/email-spans.json.gz` & `dolma-0.6.4/tests/data/expected/email-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/expected/filter-by-spans.json.gz` & `dolma-0.6.4/tests/data/expected/filter-by-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/expected/mixer.json.gz` & `dolma-0.6.4/tests/data/expected/mixer.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/expected/remove-paragraphs.json.gz` & `dolma-0.6.4/tests/data/expected/remove-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/pii-attributes.json.gz` & `dolma-0.6.4/tests/data/provided/attributes/pii/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/sample-attributes.json.gz` & `dolma-0.6.4/tests/data/provided/attributes/sample/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/data/toxicity-attributes.json.gz` & `dolma-0.6.4/tests/data/provided/attributes/toxicity/000.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/python/test_data_types.py` & `dolma-0.6.4/tests/python/test_data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         span2 = Span.from_json(span_json2)
         self.assertEqual(span_json, span2.to_json())
 
     # TODO: add tests for to/from Spec
     def test_span_to_from_spec(self):
         span = Span(start=0, end=1, type="type", score=1.0)
         with self.assertRaises(AssertionError):
-            spec = span.to_spec()
+            span.to_spec()
 
 
 class TestDocResult(TestCase):
     def test_doc_result_to_from_json(self):
         doc = Document(source="source", version="version", id="id", text="text")
         spans = [
             Span(start=0, end=2, type="xxx", score=1.0),
@@ -68,15 +68,15 @@
                 {"start": 2, "end": 4, "type": "yyy", "score": 0.5, "mention": "xt"},
             ]
         }
         self.assertEqual(doc_result_json, doc_result_json2)
 
         # from_json() requires also providing the Document
         with self.assertRaises(KeyError):
-            doc_result2 = DocResult.from_json(doc_result_json2)
+            DocResult.from_json(doc_result_json2)
         doc_result_json3 = {
             "doc": {
                 "source": "source",
                 "version": "version",
                 "id": "id",
                 "text": "text",
             },
```

### Comparing `dolma-0.6.3/tests/python/test_omegaconf.py` & `dolma-0.6.4/tests/python/test_omegaconf.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/python/test_parallel.py` & `dolma-0.6.4/tests/python/test_parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/python/test_paths.py` & `dolma-0.6.4/tests/python/test_paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,27 @@
     make_relative,
     split_glob,
     split_path,
     sub_prefix,
     sub_suffix,
 )
 
+from .utils import clean_test_data, get_test_prefix, upload_s3_prefix
+
 LOCAL_DATA = Path(__file__).parent.parent / "data"
 
 
 class TestPaths(TestCase):
+    def setUp(self) -> None:
+        self.test_prefix = get_test_prefix()
+        upload_s3_prefix(s3_prefix=f"{self.test_prefix}", local_prefix="tests/data/expected/*")
+
+    def tearDown(self) -> None:
+        clean_test_data(self.test_prefix)
+
     def test_pathify(self):
         path = "s3://path/to/file"
         protocol, path = _pathify(path)
         self.assertEqual(protocol, "s3")
         self.assertEqual(path, Path("path/to/file"))
 
         path = "path/to/file"
@@ -41,17 +50,20 @@
     def test_local_glob_path(self):
         local_glob = str(LOCAL_DATA / "*.json.gz")
         paths = list(glob_path(local_glob))
         expected = [str(LOCAL_DATA / fn) for fn in os.listdir(LOCAL_DATA) if fn.endswith(".json.gz")]
         self.assertEqual(sorted(paths), sorted(expected))
 
     def test_remote_glob_path(self):
-        prefix = "s3://ai2-llm/pretraining-data/tests/mixer/expected"
-        paths = list(glob_path(f"{prefix}/*"))
-        expected = [f"{prefix}/{fn}" for fn in os.listdir(LOCAL_DATA / "expected") if fn.endswith(".json.gz")]
+        paths = list(glob_path(f"{self.test_prefix}/**/*.json.gz"))
+        expected = [
+            f"{self.test_prefix}/tests/data/expected/{fn}"
+            for fn in os.listdir(LOCAL_DATA / "expected")
+            if fn.endswith(".json.gz")
+        ]
         self.assertEqual(sorted(paths), sorted(expected))
 
     def test_local_glob_with_recursive(self):
         local_glob = str(LOCAL_DATA / "**/*-paragraphs.json.gz")
         paths = list(glob_path(local_glob))
         expected = list(
             itertools.chain.from_iterable(
```

### Comparing `dolma-0.6.3/tests/python/test_runtime.py` & `dolma-0.6.4/tests/python/test_runtime.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/python/test_taggers.py` & `dolma-0.6.4/tests/python/test_taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.3/tests/python/test_utils.py` & `dolma-0.6.4/tests/python/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 @kylel
 
 """
 
 
 from unittest import TestCase
 
-from dolma.core.data_types import DocResult, Document, Span, TextSlice
-from dolma.core.utils import make_variable_name, split_paragraphs, split_sentences
+from dolma.core.data_types import TextSlice
+from dolma.core.utils import split_paragraphs, split_sentences
 
 
 class TestUtils(TestCase):
     def test_make_variable_name(self):
         pass
 
     def test_split_paragraphs(self):
```

### Comparing `dolma-0.6.3/Cargo.lock` & `dolma-0.6.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dolma"
-version = "0.6.3"
+version = "0.6.4"
 dependencies = [
  "ahash",
  "aws-config",
  "aws-sdk-s3",
  "byteorder",
  "clap",
  "env_logger",
```

### Comparing `dolma-0.6.3/PKG-INFO` & `dolma-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: dolma
-Version: 0.6.3
+Version: 0.6.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: requests
-Requires-Dist: tqdm
+Requires-Dist: anyascii >=0.3.2
+Requires-Dist: blingfire ==0.1.8
 Requires-Dist: boto3
 Requires-Dist: cached-path ==1.3.4
+Requires-Dist: detect-secrets ==1.4.0
+Requires-Dist: fasttext-wheel ==0.9.2
+Requires-Dist: fsspec
 Requires-Dist: msgspec >=0.14.2
+Requires-Dist: nltk ==3.8.1
+Requires-Dist: omegaconf >=2.3.0
 Requires-Dist: presidio_analyzer ==2.2.32
 Requires-Dist: pycld2 ==0.41
-Requires-Dist: fasttext >=0.9.2
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: s3fs
+Requires-Dist: smart-open
 Requires-Dist: tokenizers >=0.13.3, <1.0.0
-Requires-Dist: omegaconf >=2.3.0
-Requires-Dist: anyascii >=0.3.2
+Requires-Dist: tqdm
 Requires-Dist: uniseg
-Requires-Dist: pyyaml
-Requires-Dist: blingfire ==0.1.8
-Requires-Dist: detect-secrets ==1.4.0
-Requires-Dist: rich >=10.12.0
-Requires-Dist: smart-open >=6.3.0
-Requires-Dist: nltk ==3.8.1
-Requires-Dist: fsspec >=2021.10.0
-Requires-Dist: s3fs >=2021.10.0
 Requires-Dist: black >=22.6.0 ; extra == 'dev'
 Requires-Dist: isort >=5.10.1 ; extra == 'dev'
 Requires-Dist: mypy >=0.971 ; extra == 'dev'
 Requires-Dist: pytest >=5.2 ; extra == 'dev'
 Requires-Dist: ipython >=8.4.0 ; extra == 'dev'
 Requires-Dist: autopep8 >=1.7.0 ; extra == 'dev'
 Requires-Dist: flake8 >=5.0 ; extra == 'dev'
 Requires-Dist: ipdb >=0.13.0 ; extra == 'dev'
 Requires-Dist: flake8-pyi >=22.8.1 ; extra == 'dev'
 Requires-Dist: Flake8-pyproject >=1.1.0 ; extra == 'dev'
-Requires-Dist: awscli >=1.16.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Summary: Data filters
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>, Rodney Kinney <rodneyk@allenai.org>, Aakanksha Naik <aakankshan@allenai.org>, Abhilasha Ravichander <abhilashar@allenai.org>, Akshita Bhagia <akshitab@allenai.org>, Dirk Groeneveld <dirkg@allenai.org>, Dustin Schwenk <dustins@allenai.org>, Ian Magnusson <ianm@allenai.org>, Khyathi Chandu <khyathic@allenai.org>
 Maintainer-email: Allen Institute for Artificial Intelligence <contact@allenai.org>
 License: Apache-2.0
 Requires-Python: >=3.8
@@ -48,15 +47,15 @@
 Project-URL: Homepage, https://github.com/allenai/dolma
 
 # dolma
 
 *Data to feed OLMo's Appetite*
 
 
-<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256"></img>
+<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256">
 
 Data and tools for generating and inspecting OLMo pre-training data.
 
 To get started, install dolma using [pip](https://pypi.org/project/dolma/).
 
 ```shell
 pip install dolma
```

