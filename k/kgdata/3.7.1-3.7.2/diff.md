# Comparing `tmp/kgdata-3.7.1.tar.gz` & `tmp/kgdata-3.7.2.tar.gz`

## Comparing `kgdata-3.7.1.tar` & `kgdata-3.7.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 kgdata-3.7.1/Cargo.toml
--rw-r--r--   0     1001      123     1064 2023-06-05 04:54:27.000000 kgdata-3.7.1/LICENSE
--rw-r--r--   0     1001      123      747 2023-06-05 04:54:27.000000 kgdata-3.7.1/README.md
--rw-r--r--   0     1001      123     1551 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/bench/entity_design.rs
--rw-r--r--   0     1001      123      441 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/bench/mod.rs
--rw-r--r--   0     1001      123    33142 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/conversions.rs
--rw-r--r--   0     1001      123     4497 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/db.rs
--rw-r--r--   0     1001      123      655 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/error.rs
--rw-r--r--   0     1001      123      530 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/lib.rs
--rw-r--r--   0     1001      123     7440 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/macros.rs
--rw-r--r--   0     1001      123      527 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/class.rs
--rw-r--r--   0     1001      123     2088 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/entity.rs
--rw-r--r--   0     1001      123      245 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/entity_link.rs
--rw-r--r--   0     1001      123      426 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/entity_metadata.rs
--rw-r--r--   0     1001      123      562 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/mod.rs
--rw-r--r--   0     1001      123      648 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/multilingual.rs
--rw-r--r--   0     1001      123     3399 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/property.rs
--rw-r--r--   0     1001      123     7098 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/python/entity.rs
--rw-r--r--   0     1001      123    10911 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/python/iterators.rs
--rw-r--r--   0     1001      123      877 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/python/mod.rs
--rw-r--r--   0     1001      123     1308 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/python/multilingual.rs
--rw-r--r--   0     1001      123     8000 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/python/value.rs
--rw-r--r--   0     1001      123     5137 2023-06-05 04:54:27.000000 kgdata-3.7.1/src/models/value.rs
--rw-r--r--   0     1001      123     1499 2023-06-05 04:54:27.000000 kgdata-3.7.1/pyproject.toml
--rw-r--r--   0     1001      123    43877 2023-06-05 04:54:27.000000 kgdata-3.7.1/Cargo.lock
--rw-r--r--   0     1001      123     6129 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dataset.py
--rw-r--r--   0     1001      123       43 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/misc/__init__.py
--rw-r--r--   0     1001      123     6267 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/__init__.py
--rw-r--r--   0     1001      123     1401 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      123     7559 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      123     1138 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      123     1577 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      123     5859 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      123     3739 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      123     1829 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/multilingual.py
--rw-r--r--   0     1001      123      639 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      123      428 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      123     8252 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      123     1259 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      123     2435 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      123     9153 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      123     2426 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      123     1819 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      123     5067 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      123     1604 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      123     2893 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      123     1447 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      123     6010 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      123     1345 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      123     1908 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      123     1873 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      123     3104 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      123     1294 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      123     2454 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entity_wikilinks.py
--rw-r--r--   0     1001      123     8986 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      123     1201 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/wp2wd.py
--rw-r--r--   0     1001      123     4682 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      123     2965 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      123     1786 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      123    16555 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      123     2674 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/config.py
--rw-r--r--   0     1001      123     6623 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      123    18452 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikidata/db.py
--rw-r--r--   0     1001      123       42 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      123       27 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      123     3721 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      123     3470 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      123     1356 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      123     5053 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      123     8221 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      123     4166 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/grouped_articles.py
--rw-r--r--   0     1001      123     2910 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/articles.py
--rw-r--r--   0     1001      123     1754 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      123     1454 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      123     1983 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      123     1584 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      123     2600 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      123     4428 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      123     2805 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      123     2040 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      123     6777 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/splitter.py
--rw-r--r--   0     1001      123    13686 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/spark.py
--rw-r--r--   0     1001      123    13843 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/instances_extraction.py
--rw-r--r--   0     1001      123      138 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/prelude.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      123      648 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/infobox_property_dump.py
--rw-r--r--   0     1001      123        0 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      123     3914 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      123     1426 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      123     2040 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      123      603 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      123      608 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      123    12214 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/dbpediamodels.py
--rw-r--r--   0     1001      123    37449 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/table_extraction.py
--rw-r--r--   0     1001      123      417 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/table_tests.py
--rw-r--r--   0     1001      123     1886 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      123      364 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/config.py
--rw-r--r--   0     1001      123       27 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      123     5234 2023-06-05 04:54:27.000000 kgdata-3.7.1/kgdata/core/models.pyi
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 kgdata-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 kgdata-3.7.2/Cargo.toml
+-rw-r--r--   0     1001      123     1064 2023-06-11 01:07:48.000000 kgdata-3.7.2/LICENSE
+-rw-r--r--   0     1001      123      747 2023-06-11 01:07:48.000000 kgdata-3.7.2/README.md
+-rw-r--r--   0     1001      123     1551 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/bench/entity_design.rs
+-rw-r--r--   0     1001      123      441 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/bench/mod.rs
+-rw-r--r--   0     1001      123    33142 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/conversions.rs
+-rw-r--r--   0     1001      123     4497 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/db.rs
+-rw-r--r--   0     1001      123      655 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/error.rs
+-rw-r--r--   0     1001      123      530 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/lib.rs
+-rw-r--r--   0     1001      123     7440 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/macros.rs
+-rw-r--r--   0     1001      123      527 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/class.rs
+-rw-r--r--   0     1001      123     2088 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/entity.rs
+-rw-r--r--   0     1001      123      245 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/entity_link.rs
+-rw-r--r--   0     1001      123      426 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      123      562 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/mod.rs
+-rw-r--r--   0     1001      123      648 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/multilingual.rs
+-rw-r--r--   0     1001      123     3399 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/property.rs
+-rw-r--r--   0     1001      123     7098 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/python/entity.rs
+-rw-r--r--   0     1001      123    10911 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/python/iterators.rs
+-rw-r--r--   0     1001      123      877 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/python/mod.rs
+-rw-r--r--   0     1001      123     1308 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/python/multilingual.rs
+-rw-r--r--   0     1001      123     8000 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/python/value.rs
+-rw-r--r--   0     1001      123     5137 2023-06-11 01:07:48.000000 kgdata-3.7.2/src/models/value.rs
+-rw-r--r--   0     1001      123     1498 2023-06-11 01:07:48.000000 kgdata-3.7.2/pyproject.toml
+-rw-r--r--   0     1001      123    43877 2023-06-11 01:07:48.000000 kgdata-3.7.2/Cargo.lock
+-rw-r--r--   0     1001      123     6129 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dataset.py
+-rw-r--r--   0     1001      123       43 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      123     6267 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/__init__.py
+-rw-r--r--   0     1001      123     1401 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      123     7559 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      123     1138 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      123     1577 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      123     5859 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      123     3739 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      123     1829 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/multilingual.py
+-rw-r--r--   0     1001      123      639 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      123      428 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      123     8252 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      123     1259 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      123     2435 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      123     9153 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      123     2426 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      123     1819 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      123     5067 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      123     1604 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      123     2893 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      123     1447 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      123     6010 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      123     1345 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      123     1908 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      123     1873 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      123     3104 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      123     1294 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      123     2454 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entity_wikilinks.py
+-rw-r--r--   0     1001      123     8986 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      123     1201 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/wp2wd.py
+-rw-r--r--   0     1001      123     4682 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      123     2965 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      123     1786 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      123    16555 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      123     2674 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      123     6623 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      123    18452 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      123       42 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      123       27 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      123     3721 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      123     3470 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      123     1356 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      123     5053 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/__init__.py
+-rw-r--r--   0     1001      123     8221 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      123     4166 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/grouped_articles.py
+-rw-r--r--   0     1001      123     2910 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/articles.py
+-rw-r--r--   0     1001      123     1754 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     1454 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      123     1983 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      123     1584 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      123     2600 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      123     4428 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      123     2805 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      123     2040 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      123     6777 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/splitter.py
+-rw-r--r--   0     1001      123    13686 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/spark.py
+-rw-r--r--   0     1001      123    13843 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/instances_extraction.py
+-rw-r--r--   0     1001      123      138 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/prelude.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      123      648 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/infobox_property_dump.py
+-rw-r--r--   0     1001      123        0 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      123     3914 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      123     1426 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     2040 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      123      603 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      123      608 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      123    12214 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/dbpediamodels.py
+-rw-r--r--   0     1001      123    37449 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/table_extraction.py
+-rw-r--r--   0     1001      123      417 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/table_tests.py
+-rw-r--r--   0     1001      123     1886 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      123      364 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/config.py
+-rw-r--r--   0     1001      123       27 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      123     5234 2023-06-11 01:07:48.000000 kgdata-3.7.2/kgdata/core/models.pyi
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 kgdata-3.7.2/PKG-INFO
```

### Comparing `kgdata-3.7.1/Cargo.toml` & `kgdata-3.7.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/LICENSE` & `kgdata-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/README.md` & `kgdata-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/bench/entity_design.rs` & `kgdata-3.7.2/src/bench/entity_design.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/conversions.rs` & `kgdata-3.7.2/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/db.rs` & `kgdata-3.7.2/src/db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/error.rs` & `kgdata-3.7.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/lib.rs` & `kgdata-3.7.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/macros.rs` & `kgdata-3.7.2/src/macros.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/class.rs` & `kgdata-3.7.2/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/entity.rs` & `kgdata-3.7.2/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/mod.rs` & `kgdata-3.7.2/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/multilingual.rs` & `kgdata-3.7.2/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/property.rs` & `kgdata-3.7.2/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/python/entity.rs` & `kgdata-3.7.2/src/models/python/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/python/iterators.rs` & `kgdata-3.7.2/src/models/python/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/python/mod.rs` & `kgdata-3.7.2/src/models/python/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/python/multilingual.rs` & `kgdata-3.7.2/src/models/python/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/python/value.rs` & `kgdata-3.7.2/src/models/python/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/src/models/value.rs` & `kgdata-3.7.2/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/pyproject.toml` & `kgdata-3.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [project]
 name = "kgdata"
-version = "3.7.1"
+version = "3.7.2"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [
     { name = "Binh Vu", email = "binh@toan2.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 requires-python = ">=3.8"
 
 dependencies = [
-    'orjson >= 3.8.2, < 4.0.0',
+    'orjson >= 3.9.0, < 4.0.0',
     'tqdm >= 4.64.0, < 5.0.0',
     'beautifulsoup4 >= 4.9.3, < 5.0.0',
     'pyspark >= 3.3.0, < 4.0.0',
     'loguru >= 0.6.0, < 0.7.0',
     'rdflib >= 6.1.1, < 7.0.0',
     'six >= 1.16.0, < 2.0.0',
     'ruamel.yaml >= 0.17.21, < 0.18.0',
     'chardet >= 5.0.0, < 6.0.0',
     'ujson >= 5.5.0, < 6.0.0',
     'redis >= 3.5.3, < 4.0.0',
     'numpy >= 1.22.3, < 2.0.0',
     'fastnumbers >= 3.2.1, < 4.0.0',
     'requests >= 2.28.0, < 3.0.0',
     'sem-desc >= 4.4.2, < 5.0.0',
-    'click >= 8.0.0, <= 8.0.4',
+    'click >= 8.1.3, < 9.0.0',
     'parsimonious >= 0.8.1, < 0.9.0',
-    'hugedict >= 2.9.1, < 3.0.0',
+    'hugedict >= 2.9.2, < 3.0.0',
     'rsoup >= 3.0.1, < 4.0.0',
     'lxml >= 4.9.0, < 5.0.0',
     'ray >= 2.0.1, < 3.0.0',
 ]
 
 [project.urls]
 homepage = "https://github.com/binh-vu/kgdata"
```

### Comparing `kgdata-3.7.1/Cargo.lock` & `kgdata-3.7.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dataset.py` & `kgdata-3.7.2/kgdata/dataset.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/misc/ntriples_parser.py` & `kgdata-3.7.2/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdvalue.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/__init__.py` & `kgdata-3.7.2/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdstatement.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdproperty.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdclass.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdclass.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/multilingual.py` & `kgdata-3.7.2/kgdata/wikidata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/wdentity.py` & `kgdata-3.7.2/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/models/propertystats.py` & `kgdata-3.7.2/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/property_domains.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/class_count.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/classes.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_types.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/__main__.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/property_count.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/page_ids.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/page_dump.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entity_wikilinks.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entity_wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/entities.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/wp2wd.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/wp2wd.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/properties.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-3.7.2/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-3.7.2/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/__main__.py` & `kgdata-3.7.2/kgdata/wikidata/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/config.py` & `kgdata-3.7.2/kgdata/wikidata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/extra_ent_db.py` & `kgdata-3.7.2/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikidata/db.py` & `kgdata-3.7.2/kgdata/wikidata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-3.7.2/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/models/html_article.py` & `kgdata-3.7.2/kgdata/wikipedia/models/html_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/models/page_article.py` & `kgdata-3.7.2/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/wikiapi.py` & `kgdata-3.7.2/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/grouped_articles.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/grouped_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/articles.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/__main__.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-3.7.2/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/misc.py` & `kgdata-3.7.2/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/wikipedia/config.py` & `kgdata-3.7.2/kgdata/wikipedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/splitter.py` & `kgdata-3.7.2/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/spark.py` & `kgdata-3.7.2/kgdata/spark.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/instances_extraction.py` & `kgdata-3.7.2/kgdata/dbpedia/instances_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/infobox_property_dump.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/infobox_property_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/__main__.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-3.7.2/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/dbpediamodels.py` & `kgdata-3.7.2/kgdata/dbpedia/dbpediamodels.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/table_extraction.py` & `kgdata-3.7.2/kgdata/dbpedia/table_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/dbpedia/config.py` & `kgdata-3.7.2/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/kgdata/core/models.pyi` & `kgdata-3.7.2/kgdata/core/models.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-3.7.1/PKG-INFO` & `kgdata-3.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: kgdata
-Version: 3.7.1
+Version: 3.7.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: orjson >=3.8.2, <4.0.0
+Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: pyspark >=3.3.0, <4.0.0
 Requires-Dist: loguru >=0.6.0, <0.7.0
 Requires-Dist: rdflib >=6.1.1, <7.0.0
 Requires-Dist: six >=1.16.0, <2.0.0
 Requires-Dist: ruamel.yaml >=0.17.21, <0.18.0
 Requires-Dist: chardet >=5.0.0, <6.0.0
 Requires-Dist: ujson >=5.5.0, <6.0.0
 Requires-Dist: redis >=3.5.3, <4.0.0
 Requires-Dist: numpy >=1.22.3, <2.0.0
 Requires-Dist: fastnumbers >=3.2.1, <4.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
 Requires-Dist: sem-desc >=4.4.2, <5.0.0
-Requires-Dist: click >=8.0.0, <=8.0.4
+Requires-Dist: click >=8.1.3, <9.0.0
 Requires-Dist: parsimonious >=0.8.1, <0.9.0
-Requires-Dist: hugedict >=2.9.1, <3.0.0
+Requires-Dist: hugedict >=2.9.2, <3.0.0
 Requires-Dist: rsoup >=3.0.1, <4.0.0
 Requires-Dist: lxml >=4.9.0, <5.0.0
 Requires-Dist: ray >=2.0.1, <3.0.0
 Requires-Dist: python-dotenv >=0.19.0, <0.20.0 ; extra == 'dev'
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
 Requires-Dist: black >=22.10.0, <23.0.0 ; extra == 'dev'
 Provides-Extra: dev
```

