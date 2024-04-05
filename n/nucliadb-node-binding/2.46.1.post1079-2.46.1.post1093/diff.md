# Comparing `tmp/nucliadb_node_binding-2.46.1.post1079.tar.gz` & `tmp/nucliadb_node_binding-2.46.1.post1093.tar.gz`

## Comparing `nucliadb_node_binding-2.46.1.post1079.tar` & `nucliadb_node_binding-2.46.1.post1093.tar`

### file list

```diff
@@ -1,312 +1,310 @@
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/query_io.rs
--rw-r--r--   0     1001      127    21119 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0     1001      127     2761 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0     1001      127     8676 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0     1001      127     9257 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0     1001      127     3389 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/common/mod.rs
--rw-r--r--   0     1001      127     2044 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_reader.rs
--rw-r--r--   0     1001      127     8063 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3458 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_writer.rs
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0     1001      127     4221 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0     1001      127    21255 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
--rw-r--r--   0     1001      127    17196 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     4192 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      941 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     6724 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py
--rw-r--r--   0     1001      127     2424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10762 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2461 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     4963 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py
--rw-r--r--   0     1001      127     2361 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     4989 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5083 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8259 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1816 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2566 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18837 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    17047 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2490 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1467 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2770 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13613 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1937 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2421 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127      997 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14059 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11702 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127     7945 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/inner_settings.rs
--rw-r--r--   0     1001      127     7559 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/mod.rs
--rw-r--r--   0     1001      127     6920 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/providers.rs
--rw-r--r--   0     1001      127     1345 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/mod.rs
--rw-r--r--   0     1001      127     2860 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs
--rw-r--r--   0     1001      127    10693 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1111 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    10834 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1137 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    24437 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    21502 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127    10251 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127     9377 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6383 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     7024 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22604 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     8881 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12250 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    19361 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    12611 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1405 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    11778 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2722 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10271 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    22479 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127     8043 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     4762 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
--rw-r--r--   0     1001      127     1087 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/state.rs
--rw-r--r--   0     1001      127     2172 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    24262 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     2884 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15365 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8399 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3806 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0     1001      127     9354 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0     1001      127     1761 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0     1001      127    21119 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0     1001      127     1784 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0     1001      127    10531 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0     1001      127     1003 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0     1001      127     5550 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0     1001      127     5249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0     1001      127     2658 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0     1001      127      970 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0     1001      127     9828 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0     1001      127    10781 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0     1001      127     3071 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0     1001      127     7110 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9078 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77192 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10215 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43211 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    18949 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    32720 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/Makefile
--rw-r--r--   0     1001      127       52 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/pyproject.toml
--rw-r--r--   0     1001      127     2203 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/lib.rs
--rw-r--r--   0     1001      127     9575 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/reader.rs
--rw-r--r--   0     1001      127     2162 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/update.rs
--rw-r--r--   0     1001      127    12082 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0     1001      127     9354 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0     1001      127     1761 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0     1001      127    21119 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0     1001      127     1784 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0     1001      127    10531 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0     1001      127     1003 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0     1001      127     5550 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0     1001      127     5249 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0     1001      127     2658 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0     1001      127      970 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0     1001      127     9828 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0     1001      127    10781 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0     1001      127     3071 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0     1001      127     7110 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9078 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77192 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10215 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43211 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    18949 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    32797 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/query_io.rs
+-rw-r--r--   0     1001      127    21119 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0     1001      127     2761 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0     1001      127     8676 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0     1001      127     9257 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0     1001      127     3389 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2044 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8063 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3458 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_writer.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15365 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8399 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3806 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12250 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    19361 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    12611 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1405 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    11778 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2722 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10271 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    22479 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127     8043 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     4762 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
+-rw-r--r--   0     1001      127     1087 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/indexset/state.rs
+-rw-r--r--   0     1001      127     2172 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    18388 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    24262 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     2884 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22604 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10377 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8881 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3460 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0     1001      127     4221 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0     1001      127    21255 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
+-rw-r--r--   0     1001      127    17196 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     4192 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      941 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     6724 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py
+-rw-r--r--   0     1001      127     2424 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10718 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2461 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     4963 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py
+-rw-r--r--   0     1001      127     2361 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     4989 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     4935 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8058 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1816 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     2566 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18837 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    17037 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2490 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1473 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2765 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13680 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1035 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14060 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11690 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    10154 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1345 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/mod.rs
+-rw-r--r--   0     1001      127     2860 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    10767 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1111 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    10834 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1137 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    24437 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    21502 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127    10251 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/versions.rs
+-rw-r--r--   0     1001      127     9196 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12739 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     7024 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17053 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8279 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18507 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/pyproject.toml
+-rw-r--r--   0     1001      127     2203 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/lib.rs
+-rw-r--r--   0     1001      127     9421 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/reader.rs
+-rw-r--r--   0     1001      127     2162 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/update.rs
+-rw-r--r--   0     1001      127    11928 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-05 07:50:56.000000 nucliadb_node_binding-2.46.1.post1093/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1093/PKG-INFO
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_search.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_streaming.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/stop_words.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ar.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/az.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/bn.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ch.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/da.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/de.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/el.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/eu.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/extract.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fi.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/he.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/hu.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/id.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/it.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/kk.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ne.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/nl.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/no.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/pt.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ro.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ru.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sl.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sv.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tg.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 http = "0.2"
 hyper = "0.14.26"
 tower = "0.4.13"
 thiserror = "1"
 opentelemetry = { version = "0.17", features = ["rt-tokio", "trace"] }
 tracing-opentelemetry = "0.17.2"
 reqwest = { version = "0.11.16", features = ["json", "rustls-tls", "blocking"] }
-derive_builder = "0.12.0"
 num_cpus = "1.16.0"
 crossbeam-utils = "0.8.16"
 
 # Text Service
 async-stream = "0.3.2"
 
 rand = "0.8.4"
@@ -95,14 +94,15 @@
 tracing = { version = "0.1.29" }
 hostname = "0.3"
 username = "0.2"
 md5 = "0.7"
 lazy_static = "1.4.0"
 lru = "0.12.1"
 sysinfo = { version = "0.30.5", default-features = false }
+envy = "0.4.2"
 
 
 [build-dependencies]
 tonic-build = "0.7.0"
 
 [features]
 ci-test = []
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,16 @@
     def __lt__(self, other):
         if not isinstance(other, WorkUnit):
             return NotImplemented  # pragma: no cover
         return self._sortable_id.__lt__(other._sortable_id)
 
 
 class ConcurrentShardIndexer:
+    storage: Storage
+
     def __init__(self, writer: Writer, node_id: str):
         self.writer = writer
         self.node_id = node_id
         self.indexers: dict[str, tuple["PriorityIndexer", asyncio.Task]] = {}
 
     async def initialize(self):
         self.storage = await get_storage(service_name=SERVICE_NAME)
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     "version": "latest",
     "env": {
         "NUCLIADB_DISABLE_ANALYTICS": "True",
         "DATA_PATH": "/data",
         "READER_LISTEN_ADDRESS": "0.0.0.0:4445",
         "RUST_BACKTRACE": "full",
         "RUST_LOG": "nucliadb_*=DEBUG",  # noqa
-        "DEBUG": "1",
     },
     "options": {
         "command": [
             "/usr/local/bin/node_reader",
         ],
         "platform": "linux/amd64",
         "mem_limit": "3g",
@@ -70,15 +69,14 @@
     "version": "latest",
     "env": {
         "NUCLIADB_DISABLE_ANALYTICS": "True",
         "DATA_PATH": "/data",
         "WRITER_LISTEN_ADDRESS": "0.0.0.0:4446",
         "RUST_BACKTRACE": "full",
         "RUST_LOG": "nucliadb_*=DEBUG",  # noqa
-        "DEBUG": "1",
     },
     "options": {
         "command": [
             "/usr/local/bin/node_writer",
         ],
         "platform": "linux/amd64",
         "mem_limit": "3g",
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,32 @@
 use nucliadb_core::{node_error, NodeResult};
 use nucliadb_node::grpc::middleware::{GrpcDebugLogsLayer, GrpcInstrumentorLayer, GrpcTasksMetricsLayer};
 use nucliadb_node::grpc::reader::NodeReaderGRPCDriver;
 use nucliadb_node::http_server::run_http_server;
 use nucliadb_node::lifecycle;
 use nucliadb_node::replication::health::ReplicationHealthManager;
 use nucliadb_node::replication::NodeRole;
-use nucliadb_node::settings::providers::env::EnvSettingsProvider;
-use nucliadb_node::settings::providers::SettingsProvider;
-use nucliadb_node::settings::Settings;
+use nucliadb_node::settings::{load_settings, Settings};
 use nucliadb_node::telemetry::init_telemetry;
 use tokio::signal::unix::SignalKind;
 use tokio::signal::{ctrl_c, unix};
 use tokio::sync::Notify;
 use tonic::transport::Server;
 use tonic_health::server::HealthReporter;
 
 type GrpcServer = NodeReaderServer<NodeReaderGRPCDriver>;
 
 #[tokio::main]
 async fn main() -> NodeResult<()> {
     eprintln!("NucliaDB Reader Node starting...");
     let start_bootstrap = Instant::now();
 
-    let settings: Settings = EnvSettingsProvider::generate_settings()?;
+    let settings = load_settings()?;
 
-    if !settings.data_path().exists() {
+    if !settings.data_path.exists() {
         return Err(node_error!("Data directory missing"));
     }
 
     // XXX it probably should be moved to a more clear abstraction
     lifecycle::initialize_reader(settings.clone());
 
     let _guard = init_telemetry(&settings)?;
@@ -87,15 +85,15 @@
 
     shutdown_notifier.notify_waiters();
 
     Ok(())
 }
 
 async fn health_checker(mut health_reporter: HealthReporter, settings: Settings) -> NodeResult<()> {
-    if settings.node_role() == NodeRole::Primary {
+    if settings.node_role == NodeRole::Primary {
         // cut out early, this check is for secondaries only right now
         health_reporter.set_serving::<GrpcServer>().await;
         return Ok(());
     }
 
     let repl_health_mng = ReplicationHealthManager::new(settings.clone());
     loop {
@@ -105,15 +103,15 @@
             health_reporter.set_not_serving::<GrpcServer>().await;
         }
         tokio::time::sleep(std::time::Duration::from_secs(5)).await;
     }
 }
 
 pub async fn start_grpc_service(settings: Settings, shutdown_notifier: Arc<Notify>) -> NodeResult<()> {
-    let listen_address = settings.reader_listen_address();
+    let listen_address = settings.reader_listen_address;
     eprintln!("Reader listening for gRPC requests at: {:?}", listen_address);
 
     let tracing_middleware = GrpcInstrumentorLayer;
     let debug_logs_middleware = GrpcDebugLogsLayer;
     let metrics_middleware = GrpcTasksMetricsLayer;
 
     let (health_reporter, health_service) = tonic_health::server::health_reporter();
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 use nucliadb_node::grpc::middleware::{GrpcDebugLogsLayer, GrpcInstrumentorLayer, GrpcTasksMetricsLayer};
 use nucliadb_node::grpc::writer::{NodeWriterEvent, NodeWriterGRPCDriver};
 use nucliadb_node::http_server::run_http_server;
 use nucliadb_node::node_metadata::NodeMetadata;
 use nucliadb_node::replication::replicator::connect_to_primary_and_replicate_forever;
 use nucliadb_node::replication::service::ReplicationServiceGRPCDriver;
 use nucliadb_node::replication::NodeRole;
-use nucliadb_node::settings::providers::env::EnvSettingsProvider;
-use nucliadb_node::settings::providers::SettingsProvider;
-use nucliadb_node::settings::Settings;
+use nucliadb_node::settings::{load_settings, Settings};
 use nucliadb_node::shards::cache::ShardWriterCache;
 use nucliadb_node::telemetry::init_telemetry;
 use nucliadb_node::{lifecycle, utils};
 use nucliadb_protos::replication;
 use tokio::signal::unix::SignalKind;
 use tokio::signal::{ctrl_c, unix};
 use tokio::sync::mpsc::{UnboundedReceiver, UnboundedSender};
@@ -72,43 +70,42 @@
 }
 
 #[tokio::main]
 async fn main() -> NodeResult<()> {
     eprintln!("NucliaDB Writer Node starting...");
     let start_bootstrap = Instant::now();
 
-    let settings: Settings = EnvSettingsProvider::generate_settings()?;
+    let settings = load_settings()?;
 
     let _guard = init_telemetry(&settings)?;
     let metrics = metrics::get_metrics();
 
-    let data_path = settings.data_path();
+    let data_path = &settings.data_path;
     if !data_path.exists() {
-        std::fs::create_dir(data_path.clone())?;
+        std::fs::create_dir(data_path)?;
     }
 
     lifecycle::initialize_writer(settings.clone())?;
 
     let node_metadata = NodeMetadata::new(settings.clone()).await?;
     let (metadata_sender, metadata_receiver) = tokio::sync::mpsc::unbounded_channel();
 
-    let host_key_path = settings.host_key_path();
-    let node_id = utils::read_or_create_host_key(host_key_path)?;
+    let node_id = utils::read_or_create_host_key(&settings.host_key_path)?;
 
     nucliadb_node::analytics::sync::start_analytics_loop();
 
     let (shutdown_notifier, shutdown_notified) = get_shutdown_notifier();
     let shard_cache = Arc::new(ShardWriterCache::new(settings.clone()));
 
-    if settings.node_role() == NodeRole::Primary {
+    if settings.node_role == NodeRole::Primary {
         lifecycle::initialize_merger(Arc::clone(&shard_cache), settings.clone())?;
     }
 
     let mut replication_task = None;
-    if settings.node_role() == NodeRole::Secondary {
+    if settings.node_role == NodeRole::Secondary {
         // when it's a secondary server, do not even run the writer GRPC service
         // because nothing should happen through that interface
         replication_task = Some(tokio::spawn(connect_to_primary_and_replicate_forever(
             settings.clone(),
             Arc::clone(&shard_cache),
             node_id.to_string(),
             Arc::clone(&shutdown_notified),
@@ -136,15 +133,15 @@
 
     let metrics_task = tokio::spawn(run_http_server(settings.clone()));
     info!("Bootstrap complete in: {:?}", start_bootstrap.elapsed());
 
     wait_for_sigkill().await?;
 
     shutdown_notifier.notify_waiters();
-    if settings.node_role() == NodeRole::Primary {
+    if settings.node_role == NodeRole::Primary {
         lifecycle::finalize_merger();
     }
 
     info!("Shutting down NucliaDB Writer Node...");
     metrics_task.abort();
     grpc_task.await??; // wait for shutdown of server instead of aborting it
     let _ = metrics_task.await;
@@ -171,30 +168,30 @@
 pub async fn start_grpc_service(
     settings: Settings,
     shard_cache: Arc<ShardWriterCache>,
     metadata_sender: UnboundedSender<NodeWriterEvent>,
     node_id: String,
     shutdown_notifier: Arc<Notify>,
 ) -> NodeResult<()> {
-    let listen_address = settings.writer_listen_address();
+    let listen_address = settings.writer_listen_address;
 
     let tracing_middleware = GrpcInstrumentorLayer;
     let debug_logs_middleware = GrpcDebugLogsLayer;
     let metrics_middleware = GrpcTasksMetricsLayer;
 
     let (mut health_reporter, health_service) = tonic_health::server::health_reporter();
     health_reporter.set_serving::<GrpcServer>().await;
 
     let mut server_builder = Server::builder()
         .layer(tracing_middleware)
         .layer(debug_logs_middleware)
         .layer(metrics_middleware)
         .add_service(health_service);
 
-    if settings.node_role() == NodeRole::Primary {
+    if settings.node_role == NodeRole::Primary {
         let grpc_driver = NodeWriterGRPCDriver::new(settings.clone(), shard_cache.clone()).with_sender(metadata_sender);
         server_builder = server_builder.add_service(GrpcServer::new(grpc_driver));
     }
     let replication_server = replication::replication_service_server::ReplicationServiceServer::new(
         ReplicationServiceGRPCDriver::new(settings.clone(), shard_cache.clone(), node_id),
     );
     server_builder = server_builder.add_service(replication_server);
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -339,26 +339,26 @@
                 Ok(tonic::Response::new(list))
             }
             Err(error) => Err(tonic::Status::internal(error.to_string())),
         }
     }
 
     async fn get_metadata(&self, _request: Request<EmptyQuery>) -> Result<Response<NodeMetadata>, Status> {
-        let settings = &self.settings.clone();
+        let settings = &self.settings;
         let mut total_disk = 0;
         let mut available_disk = 0;
 
         for disk in sysinfo::Disks::new_with_refreshed_list().into_iter() {
             total_disk += disk.total_space();
             available_disk += disk.available_space();
         }
         Ok(tonic::Response::new(NodeMetadata {
             shard_count: list_shards(settings.shards_path()).await.len().try_into().unwrap(),
-            node_id: read_host_key(settings.host_key_path()).unwrap().to_string(),
-            primary_node_id: get_primary_node_id(settings.data_path()),
+            node_id: read_host_key(&settings.host_key_path).unwrap().to_string(),
+            primary_node_id: get_primary_node_id(&settings.data_path),
             available_disk,
             total_disk,
             ..Default::default()
         }))
     }
 
     async fn gc(&self, request: Request<ShardId>) -> Result<Response<GarbageCollectorResponse>, Status> {
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 use axum::routing::get;
 use axum::Router;
 
 use crate::settings::Settings;
 
 pub async fn run_http_server(settings: Settings) {
     // Add routes to services
-    let addr = SocketAddr::from(([0, 0, 0, 0], settings.metrics_port()));
+    let addr = SocketAddr::from(([0, 0, 0, 0], settings.metrics_port));
     let router = Router::new().route("/metrics", get(metrics_service::metrics_service));
     let router = router.route("/__dump", get(traces_service::thread_dump_service));
     axum_server::bind(addr).serve(router.into_make_service()).await.expect("Error starting the HTTP server");
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 use nucliadb_core::merge::{install_merge_requester, MergerError};
 use nucliadb_core::prelude::*;
 use nucliadb_core::thread::ThreadPoolBuilder;
 
 /// Initialize the index node writer. This function must be called before using
 /// a writer
 pub fn initialize_writer(settings: Settings) -> NodeResult<()> {
-    let data_path = settings.data_path();
+    let data_path = &settings.data_path;
     let shards_path = settings.shards_path();
     if !data_path.exists() {
         return Err(node_error!("Data directory ({:?}) should be already created", data_path));
     }
 
     if !shards_path.exists() {
         std::fs::create_dir(shards_path)?;
     }
 
     // We shallow the error if the threadpools were already initialized
-    let _ = ThreadPoolBuilder::new().num_threads(settings.num_global_rayon_threads()).build_global();
+    let _ = ThreadPoolBuilder::new().num_threads(settings.num_global_rayon_threads).build_global();
 
     Ok(())
 }
 
 /// Initialize the global merge scheduler. This function must be called if merge
 /// scheduler should run
 pub fn initialize_merger(shard_cache: Arc<ShardWriterCache>, settings: Settings) -> Result<(), MergerError> {
@@ -63,9 +63,9 @@
     merge::stop_global_merger();
 }
 
 /// Initialize the index node reader. This function must be called before using
 /// a reader
 pub fn initialize_reader(settings: Settings) {
     // We swallow the error if the threadpool was already initialized
-    let _ = ThreadPoolBuilder::new().num_threads(settings.num_global_rayon_threads()).build_global();
+    let _ = ThreadPoolBuilder::new().num_threads(settings.num_global_rayon_threads).build_global();
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     /// Signals the scheduler to stop
     pub fn stop(&self) {
         self.shutdown.store(true, Ordering::Relaxed);
     }
 
     fn run(&self) {
-        let work = self.wait_for_work(self.settings.merge_scheduler_free_time_work_scheduling_delay());
+        let work = self.wait_for_work(self.settings.merge_scheduler_free_time_work_scheduling_delay);
 
         match work {
             Some(request) => {
                 let merge = self.process(request);
                 if let Err(error) = merge {
                     warn!("An error occurred while merging: {}", error);
                 }
@@ -296,24 +296,26 @@
 mod tests {
     use std::fs;
     use std::thread;
     use tempfile::{self, TempDir};
     use tokio;
 
     use crate::disk_structure;
+    use crate::settings::EnvSettings;
 
     use super::*;
 
     fn merge_scheduler() -> (MergeScheduler, TempDir) {
         let temp_dir = tempfile::tempdir().unwrap();
-        let settings = Settings::builder()
-            .data_path(temp_dir.path())
-            .merge_scheduler_free_time_work_scheduling_delay(Duration::from_millis(5))
-            .build()
-            .unwrap();
+        let settings: Settings = EnvSettings {
+            data_path: temp_dir.path().to_owned(),
+            merge_scheduler_free_time_work_scheduling_delay: Duration::from_millis(5),
+            ..Default::default()
+        }
+        .into();
         let shard_cache = Arc::new(ShardWriterCache::new(settings.clone()));
         fs::create_dir_all(settings.shards_path()).unwrap();
 
         (MergeScheduler::new(shard_cache, settings), temp_dir)
     }
 
     #[test]
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     pub shard_count: u64,
     pub settings: Settings,
 }
 
 pub fn create_node_metadata_pb(settings: Settings, node_metadata: NodeMetadata) -> nucliadb_core::protos::NodeMetadata {
     nucliadb_core::protos::NodeMetadata {
         shard_count: node_metadata.shard_count,
-        node_id: utils::read_host_key(settings.host_key_path()).unwrap().to_string(),
-        primary_node_id: get_primary_node_id(settings.data_path()),
+        node_id: utils::read_host_key(&settings.host_key_path).unwrap().to_string(),
+        primary_node_id: get_primary_node_id(&settings.data_path),
         ..Default::default()
     }
 }
 
 impl NodeMetadata {
     pub async fn new(settings: Settings) -> NodeResult<Self> {
         Ok(Self {
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     pub fn new(settings: Settings) -> Self {
         Self {
             settings,
         }
     }
 
     fn health_filepath(&self) -> String {
-        format!("{}/{}", self.settings.data_path().to_string_lossy(), REPLICATION_HEALTH_FILE)
+        format!("{}/{}", self.settings.data_path.to_string_lossy(), REPLICATION_HEALTH_FILE)
     }
 
     pub fn update_healthy(&self) {
         if OpenOptions::new().write(true).create(true).open(self.health_filepath()).is_err() {
             error!("Error updating replication health status");
             return;
         }
@@ -60,10 +60,10 @@
             return false;
         }
         let metaddata = Path::new(&self.health_filepath()).metadata();
         if metaddata.is_err() {
             return false;
         }
         let metadata = metaddata.unwrap();
-        metadata.modified().unwrap() > std::time::SystemTime::now() - self.settings.replication_healthy_delay()
+        metadata.modified().unwrap() > std::time::SystemTime::now() - self.settings.replication_healthy_delay
     }
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
+//
+
+use nucliadb_procs::{measure};
+
+#[measure(actor = "vectors", metric = "my-test", metric = "my-other-test")]
+fn test_metric_defined_twice() {}
 
-pub mod health;
-pub mod replicator;
-pub mod service;
 
-#[derive(Clone, PartialEq, Debug, Copy)]
-pub enum NodeRole {
-    Primary,
-    Secondary,
-}
+// Make trybuild happy and avoid errors due to not having a main function
+fn main() {}
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -193,40 +193,40 @@
 
 pub async fn connect_to_primary_and_replicate(
     settings: Settings,
     shard_cache: Arc<ShardWriterCache>,
     secondary_id: String,
     shutdown_notified: Arc<AtomicBool>,
 ) -> NodeResult<()> {
-    let mut primary_address = settings.primary_address();
+    let mut primary_address = settings.primary_address.clone();
     if !primary_address.starts_with("http://") {
         primary_address = format!("http://{}", primary_address);
     }
     eprintln!("Connecting to primary: {:?}", primary_address);
     let mut client =
         replication::replication_service_client::ReplicationServiceClient::connect(primary_address.clone()).await?;
     // .max_decoding_message_size(256 * 1024 * 1024)
     // .max_encoding_message_size(256 * 1024 * 1024);address);
 
     let repl_health_mng = ReplicationHealthManager::new(settings.clone());
     let metrics = metrics::get_metrics();
 
     let primary_node_metadata = client.get_metadata(Request::new(EmptyQuery {})).await?.into_inner();
 
-    set_primary_node_id(settings.data_path(), primary_node_metadata.node_id)?;
+    set_primary_node_id(&settings.data_path, primary_node_metadata.node_id)?;
 
     let shards_path = settings.shards_path();
     loop {
         if shutdown_notified.load(std::sync::atomic::Ordering::Relaxed) {
             return Ok(());
         }
 
         let existing_shards = list_shards(settings.shards_path()).await;
         let mut shard_states = Vec::new();
-        let mut worker_pool = ReplicateWorkerPool::new(settings.replication_max_concurrency() as usize);
+        let mut worker_pool = ReplicateWorkerPool::new(settings.replication_max_concurrency as usize);
         for shard_id in existing_shards.clone() {
             if let Some(metadata) = shard_cache.get_metadata(shard_id.clone()) {
                 shard_states.push(replication::SecondaryShardReplicationState {
                     shard_id: shard_id.clone(),
                     generation_id: metadata.get_generation_id().unwrap_or("UNSET_SECONDARY".to_string()),
                 });
             }
@@ -321,15 +321,15 @@
         worker_pool.wait_for_workers().await?;
 
         // Healthy check and delays for manage replication.
         //
         // 1. If we're healthy, we'll sleep for a while and check again.
         // 2. If backed up replicating, we'll try replicating again immediately and check again.
         let elapsed = start.elapsed();
-        if elapsed < settings.replication_healthy_delay() {
+        if elapsed < settings.replication_healthy_delay {
             // only update healthy marker if we're up-to-date in the configured healthy time
             repl_health_mng.update_healthy();
         }
 
         if no_shards_to_sync && no_shards_to_remove {
             // if we have any changes, check again immediately
             // otherwise, wait for a bit
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 impl replication::replication_service_server::ReplicationService for ReplicationServiceGRPCDriver {
     type ReplicateShardStream = ReceiverStream<Result<replication::ReplicateShardResponse, tonic::Status>>;
 
     async fn check_replication_state(
         &self,
         raw_request: tonic::Request<replication::SecondaryCheckReplicationStateRequest>,
     ) -> Result<tonic::Response<replication::PrimaryCheckReplicationStateResponse>, tonic::Status> {
-        if self.settings.node_role() != NodeRole::Primary {
+        if self.settings.node_role != NodeRole::Primary {
             return Err(tonic::Status::unavailable("This node is not a primary node"));
         }
         let request = raw_request.into_inner();
         let mut resp_shard_states = Vec::new();
         let request_shard_states = request.shard_states;
         let shard_ids = list_shards(self.settings.shards_path()).await;
         let shards_to_remove = request_shard_states
@@ -289,25 +289,25 @@
         Ok(Response::new(ReceiverStream::new(receiver.1)))
     }
 
     async fn get_metadata(
         &self,
         _request: tonic::Request<noderesources::EmptyQuery>,
     ) -> Result<tonic::Response<noderesources::NodeMetadata>, tonic::Status> {
-        let settings = &self.settings.clone();
+        let settings = &self.settings;
         let mut total_disk = 0;
         let mut available_disk = 0;
 
         for disk in sysinfo::Disks::new_with_refreshed_list().into_iter() {
             total_disk += disk.total_space();
             available_disk += disk.available_space();
         }
         Ok(tonic::Response::new(noderesources::NodeMetadata {
             shard_count: list_shards(settings.shards_path()).await.len().try_into().unwrap(),
-            node_id: read_host_key(settings.host_key_path()).unwrap().to_string(),
-            primary_node_id: get_primary_node_id(settings.data_path()),
+            node_id: read_host_key(&settings.host_key_path).unwrap().to_string(),
+            primary_node_id: get_primary_node_id(&settings.data_path),
             total_disk,
             available_disk,
             ..Default::default()
         }))
     }
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs`

 * *Files 2% similar despite different names*

```diff
@@ -229,22 +229,26 @@
     use std::thread::sleep;
     use std::time::Duration;
 
     use crossbeam_utils::thread::scope;
     use tempfile::tempdir;
 
     use super::ShardWriterCache;
-    use crate::settings::Settings;
+    use crate::settings::{EnvSettings, Settings};
     use crate::shards::metadata::{ShardMetadata, Similarity};
     use crate::shards::ShardId;
 
     #[test]
     fn test_safe_deletion() {
         let data_dir = tempdir().unwrap();
-        let settings = Settings::builder().data_path(data_dir.into_path()).build().unwrap();
+        let settings: Settings = EnvSettings {
+            data_path: data_dir.into_path(),
+            ..Default::default()
+        }
+        .into();
         let cache = Arc::new(ShardWriterCache::new(settings.clone()));
 
         let shard_id_0 = ShardId::from("shard_id_0");
         let shard_0_path = settings.shards_path().join(shard_id_0.clone());
         fs::create_dir(settings.shards_path()).unwrap();
 
         let shard_meta = ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None);
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/versions.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/shards/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,29 +38,22 @@
 
 pub fn init_telemetry(settings: &Settings) -> NodeResult<Option<ClientInitGuard>> {
     let mut layers = Vec::new();
 
     let stdout = stdout_layer(settings);
     layers.push(stdout);
 
-    if settings.jaeger_enabled() {
+    if settings.jaeger_enabled {
         let jaeger = jaeger_layer(settings)?;
         layers.push(jaeger);
     }
 
-    let sentry_guard;
-
-    if settings.sentry_enabled() {
-        sentry_guard = Some(setup_sentry(settings.sentry_env(), settings.sentry_url()));
-        let sentry = sentry_layer();
-        layers.push(sentry);
-    } else {
-        eprintln!("Sentry disabled");
-        sentry_guard = None;
-    }
+    let sentry_guard = Some(setup_sentry(settings.sentry_env(), settings.sentry_url.clone()));
+    let sentry = sentry_layer();
+    layers.push(sentry);
 
     tracing_subscriber::registry().with(layers).try_init().with_context(|| "trying to init tracing")?;
 
     Ok(sentry_guard)
 }
 
 pub struct LogLevelsFilter {
@@ -138,15 +131,15 @@
 /// - catch-all using `*`
 fn stdout_layer(settings: &Settings) -> Box<dyn Layer<Registry> + Send + Sync> {
     let log_levels = settings.log_levels().to_vec();
     let layer = tracing_subscriber::fmt::layer().with_level(true).with_target(true);
 
     let filter = LogLevelsFilter::new(log_levels);
 
-    if settings.plain_logs() || settings.debug() {
+    if settings.debug {
         layer.event_format(tracing_subscriber::fmt::format().compact()).with_filter(filter).boxed()
     } else {
         layer
             .event_format(tracing_subscriber::fmt::format::Format::default().json())
             .fmt_fields(tracing_subscriber::fmt::format::JsonFields::new())
             .with_filter(filter)
             .boxed()
@@ -171,15 +164,15 @@
     let span_filter = FilterFn::new(|metadata| {
         metadata.is_span() && metadata.file().filter(|file| file.contains("nucliadb")).is_some()
     });
 
     Ok(tracing_opentelemetry::layer().with_tracer(tracer).with_filter(level_filter).with_filter(span_filter).boxed())
 }
 
-fn setup_sentry(env: &'static str, sentry_url: String) -> ClientInitGuard {
+fn setup_sentry(env: String, sentry_url: String) -> ClientInitGuard {
     sentry::init((
         sentry_url,
         sentry::ClientOptions {
             release: sentry::release_name!(),
             environment: Some(env.into()),
             ..Default::default()
         },
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 use std::net::{SocketAddr, ToSocketAddrs};
-use std::path::PathBuf;
+use std::path::{Path, PathBuf};
 use std::str::FromStr;
 use std::time::Duration;
 use std::{fs, thread};
 
 use http::Uri;
 use nucliadb_core::tracing::{info, Level};
 use nucliadb_core::{Context, NodeResult};
@@ -62,58 +62,59 @@
     }
     SocketAddr::from_str(&host).unwrap_or_else(|_| panic!("Unable to resolve IP address for {}", host))
 }
 
 pub fn parse_log_levels(levels: &str) -> Vec<(String, Level)> {
     levels
         .split(',')
+        .filter(|s| !s.is_empty())
         .map(|s| s.splitn(2, '=').collect::<Vec<_>>())
         .map(|v| (v[0].to_string(), Level::from_str(v[1]).unwrap()))
         .collect()
 }
 
-pub fn read_host_key(hk_path: PathBuf) -> NodeResult<Uuid> {
+pub fn read_host_key(hk_path: &Path) -> NodeResult<Uuid> {
     let host_key_contents =
-        fs::read(hk_path.clone()).with_context(|| format!("Failed to read host key from '{}'", hk_path.display()))?;
+        fs::read(hk_path).with_context(|| format!("Failed to read host key from '{}'", hk_path.display()))?;
 
     let host_key = Uuid::from_slice(host_key_contents.as_slice())
         .with_context(|| format!("Invalid host key from '{}'", hk_path.display()))?;
 
     Ok(host_key)
 }
 
 /// Reads the key that makes a node unique from the given file.
 /// If the file does not exist, it generates an ID and writes it to the file
 /// so that it can be reused on reboot.
-pub fn read_or_create_host_key(hk_path: PathBuf) -> NodeResult<Uuid> {
+pub fn read_or_create_host_key(hk_path: &Path) -> NodeResult<Uuid> {
     let host_key;
 
     if hk_path.exists() {
         host_key = read_host_key(hk_path)?;
         info!(host_key=?host_key, "Read existing host key.");
     } else {
         host_key = Uuid::new_v4();
-        fs::write(hk_path.clone(), host_key.as_bytes())
+        fs::write(hk_path, host_key.as_bytes())
             .with_context(|| format!("Failed to write host key to '{}'", hk_path.display()))?;
         info!(host_key=?host_key, host_key_path=?hk_path, "Create new host key.");
     }
 
     Ok(host_key)
 }
 
-pub fn set_primary_node_id(data_path: PathBuf, primary_id: String) -> NodeResult<()> {
+pub fn set_primary_node_id(data_path: &Path, primary_id: String) -> NodeResult<()> {
     let filepath = data_path.join("primary_id");
 
     fs::write(filepath.clone(), primary_id)
         .with_context(|| format!("Failed to write primary ID to '{}'", filepath.display()))?;
 
     Ok(())
 }
 
-pub fn get_primary_node_id(data_path: PathBuf) -> Option<String> {
+pub fn get_primary_node_id(data_path: &Path) -> Option<String> {
     let filepath = data_path.join("primary_id");
     let read_result = fs::read(filepath.clone());
     if read_result.is_err() {
         return None;
     }
     read_result.map(|bytes| String::from_utf8(bytes).unwrap()).ok()
 }
@@ -179,12 +180,12 @@
     #[test]
     #[serial]
     fn test_set_primary_id() {
         let tempdir = TempDir::new().expect("Unable to create temporary data directory");
         let tempdir_path = tempdir.into_path();
         // set env variable
         let primary_id = "test_primary_id".to_string();
-        set_primary_node_id(tempdir_path.clone(), primary_id.clone()).unwrap();
-        let read_primary_id = get_primary_node_id(tempdir_path).unwrap();
+        set_primary_node_id(&tempdir_path, primary_id.clone()).unwrap();
+        let read_primary_id = get_primary_node_id(&tempdir_path).unwrap();
         assert_eq!(primary_id, read_primary_id);
     }
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files 3% similar despite different names*

```diff
@@ -111,35 +111,38 @@
         let tempdir = TempDir::new().expect("Unable to create temporary data directory");
         let secondary_tempdir = TempDir::new().expect("Unable to create temporary data directory");
 
         let reader_addr = SocketAddr::new(IpAddr::V4(Ipv4Addr::new(127, 0, 0, 1)), find_open_port());
         let writer_addr = SocketAddr::new(IpAddr::V4(Ipv4Addr::new(127, 0, 0, 1)), find_open_port());
         let secondary_reader_addr = SocketAddr::new(IpAddr::V4(Ipv4Addr::new(127, 0, 0, 1)), find_open_port());
 
-        let settings = Settings::builder()
-            .data_path(tempdir.path())
-            .reader_listen_address(reader_addr.to_string())
-            .writer_listen_address(writer_addr.to_string())
-            .build()
-            .expect("Error while building test settings");
-        let secondary_settings = Settings::builder()
-            .data_path(secondary_tempdir.path())
-            .reader_listen_address(secondary_reader_addr.to_string())
-            .primary_address(writer_addr.to_string())
-            .replication_delay(Duration::from_secs(1))
-            .build()
-            .expect("Error while building test settings");
+        let settings: Settings = EnvSettings {
+            data_path: tempdir.path().to_owned(),
+            reader_listen_address: reader_addr,
+            writer_listen_address: writer_addr,
+            ..Default::default()
+        }
+        .into();
+
+        let secondary_settings = EnvSettings {
+            data_path: secondary_tempdir.path().to_owned(),
+            reader_listen_address: secondary_reader_addr,
+            primary_address: writer_addr.to_string(),
+            replication_delay_seconds: 1,
+            ..Default::default()
+        }
+        .into();
 
-        for _setting in [&settings, &secondary_settings] {
-            let data_path = _setting.data_path();
+        for setting in [&settings, &secondary_settings] {
+            let data_path = &setting.data_path;
             if !data_path.exists() {
-                std::fs::create_dir(&data_path).expect("Cannot create data directory");
+                std::fs::create_dir(data_path).expect("Cannot create data directory");
             }
 
-            let shards_path = _setting.shards_path();
+            let shards_path = setting.shards_path();
             if !shards_path.exists() {
                 std::fs::create_dir(&shards_path).expect("Cannot create shards directory");
             }
         }
 
         let shutdown_notifier = Arc::new(Notify::new());
         let shutdown_notified = Arc::new(AtomicBool::new(false));
@@ -225,16 +228,15 @@
     pub async fn with_secondary_writer(&mut self) -> anyhow::Result<&mut Self> {
         if self.secondary_writer_server_task.is_some() {
             return Ok(self);
         }
 
         let settings = self.secondary_settings.clone();
         let cache_settings = self.secondary_settings.clone();
-        let host_key_path = settings.host_key_path();
-        let node_id = read_or_create_host_key(host_key_path)?;
+        let node_id = read_or_create_host_key(&settings.host_key_path)?;
         let shards_cache = Arc::new(ShardWriterCache::new(cache_settings));
         self.secondary_shard_cache = Some(shards_cache.clone());
         let notified = Arc::clone(&self.shutdown_notified);
         self.secondary_writer_server_task = Some(tokio::spawn(async move {
             lifecycle::initialize_writer(settings.clone()).expect("Writer initialization has failed");
             connect_to_primary_and_replicate(settings, shards_cache, node_id.to_string(), notified).await.unwrap();
         }));
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-use nucliadb_procs::{measure};
-
-#[measure(actor = "vectors", metric = "my-test", metric = "my-other-test")]
-fn test_metric_defined_twice() {}
+use nucliadb_procs::measure;
 
+#[measure(actor = "wrong", metric = "my-test")]
+fn test_wrong_actor() {}
 
 // Make trybuild happy and avoid errors due to not having a main function
 fn main() {}
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,29 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-use nucliadb_procs::measure;
+//! Set of parameters needed by the HNSW algorithm
+//! as named and used in the paper.
 
-#[measure(actor = "wrong", metric = "my-test")]
-fn test_wrong_actor() {}
+/// Factor by which the layer distribution should deviate.
+pub fn level_factor() -> f64 {
+    1.0 / (m() as f64).ln()
+}
 
-// Make trybuild happy and avoid errors due to not having a main function
-fn main() {}
+/// Upper limit to the number of out-edges a embedding can have.
+pub const fn m_max() -> usize {
+    60
+}
+
+/// Number of bi-directional links created for every new element.
+pub const fn m() -> usize {
+    30
+}
+
+/// Number of neighbours that are searched for before adding a new embedding.
+pub const fn ef_construction() -> usize {
+    100
+}
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -12,31 +12,19 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
-//
-
-//! Set of parameters needed by the HNSW algorithm
-//! as named and used in the paper.
-
-/// Factor by which the layer distribution should deviate.
-pub fn level_factor() -> f64 {
-    1.0 / (m() as f64).ln()
-}
 
-/// Upper limit to the number of out-edges a embedding can have.
-pub const fn m_max() -> usize {
-    60
-}
+use serde::Deserialize;
 
-/// Number of bi-directional links created for every new element.
-pub const fn m() -> usize {
-    30
-}
+pub mod health;
+pub mod replicator;
+pub mod service;
 
-/// Number of neighbours that are searched for before adding a new embedding.
-pub const fn ef_construction() -> usize {
-    100
+#[derive(Clone, PartialEq, Debug, Copy, Deserialize)]
+pub enum NodeRole {
+    Primary,
+    Secondary,
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/indexset/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/state.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/indexset/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files 0% similar despite different names*

```diff
@@ -700,14 +700,16 @@
     pub uri: ::prost::alloc::string::String,
     #[prost(string, tag="5")]
     pub language: ::prost::alloc::string::String,
     #[prost(map="string, string", tag="6")]
     pub localstorage: ::std::collections::HashMap<::prost::alloc::string::String, ::prost::alloc::string::String>,
     #[prost(string, tag="7")]
     pub css_selector: ::prost::alloc::string::String,
+    #[prost(string, tag="8")]
+    pub xpath: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Keyword {
     #[prost(string, tag="1")]
     pub value: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-2.46.1.post1093/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1093/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "2.46.1-post1079"
+version = "2.46.1-post1093"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/CHANGELOG.md` & `nucliadb_node_binding-2.46.1.post1093/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/Makefile` & `nucliadb_node_binding-2.46.1.post1093/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/cov.sh` & `nucliadb_node_binding-2.46.1.post1093/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/pyproject.toml` & `nucliadb_node_binding-2.46.1.post1093/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/collect_garbage.rs` & `nucliadb_node_binding-2.46.1.post1093/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/errors.rs` & `nucliadb_node_binding-2.46.1.post1093/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1093/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1093/src/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 use crate::errors::{IndexNodeException, LoadShardError};
 use crate::update::{update_loop, UpdateParameters};
 use crate::RawProtos;
 use nucliadb_core::paragraphs::ParagraphIterator;
 use nucliadb_core::protos::*;
 use nucliadb_core::texts::DocumentIterator;
 use nucliadb_node::lifecycle;
-use nucliadb_node::settings::providers::env::EnvSettingsProvider;
-use nucliadb_node::settings::providers::SettingsProvider;
-use nucliadb_node::settings::Settings;
+use nucliadb_node::settings::load_settings;
 use nucliadb_node::shards::cache::ShardReaderCache;
 use nucliadb_node::shards::reader::ShardReader;
 use prost::Message;
 use pyo3::exceptions::{PyStopIteration, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 use pyo3::PyErr;
@@ -84,15 +82,15 @@
     }
 }
 
 #[pymethods]
 impl NodeReader {
     #[new]
     pub fn new() -> Self {
-        let settings: Settings = EnvSettingsProvider::generate_settings().unwrap();
+        let settings = load_settings().unwrap();
         lifecycle::initialize_reader(settings.clone());
 
         let shards = Arc::new(ShardReaderCache::new(settings.clone()));
         let shards_update_loop_copy = Arc::clone(&shards);
         let update_parameters = UpdateParameters {
             shards_path: settings.shards_path(),
             refresh_rate: REFRESH_RATE,
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/update.rs` & `nucliadb_node_binding-2.46.1.post1093/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1093/src/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 use crate::RawProtos;
 use nucliadb_core::merge::MergerError;
 use nucliadb_core::protos::*;
 use nucliadb_core::Channel;
 use nucliadb_node::analytics::blocking::send_analytics_event;
 use nucliadb_node::analytics::payload::AnalyticsEvent;
 use nucliadb_node::lifecycle;
-use nucliadb_node::settings::providers::env::EnvSettingsProvider;
-use nucliadb_node::settings::providers::SettingsProvider;
-use nucliadb_node::settings::Settings;
+use nucliadb_node::settings::load_settings;
 use nucliadb_node::shards::cache::ShardWriterCache;
 use nucliadb_node::shards::metadata::ShardMetadata;
 use nucliadb_node::shards::writer::ShardWriter;
 use prost::Message;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyList;
@@ -62,15 +60,15 @@
     }
 }
 
 #[pymethods]
 impl NodeWriter {
     #[new]
     pub fn new() -> PyResult<Self> {
-        let settings: Settings = EnvSettingsProvider::generate_settings().unwrap();
+        let settings = load_settings().unwrap();
         let shard_cache = Arc::new(ShardWriterCache::new(settings.clone()));
         let shards_gc_loop_copy = Arc::clone(&shard_cache);
         let gc_parameters = GCParameters {
             shards_path: settings.shards_path(),
             loop_interval: GC_LOOP_INTERVAL,
         };
         let gc_loop_handle = std::thread::spawn(|| {
```

### Comparing `nucliadb_node_binding-2.46.1.post1079/tests/__init__.py` & `nucliadb_node_binding-2.46.1.post1093/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/tests/conftest.py` & `nucliadb_node_binding-2.46.1.post1093/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1079/tests/integration/test_indexing.py` & `nucliadb_node_binding-2.46.1.post1093/tests/integration/test_indexing.py`

 * *Files identical despite different names*

