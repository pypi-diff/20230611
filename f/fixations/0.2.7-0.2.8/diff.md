# Comparing `tmp/fixations-0.2.7.tar.gz` & `tmp/fixations-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixations-0.2.7.tar", max compression
+gzip compressed data, was "fixations-0.2.8.tar", max compression
```

## Comparing `fixations-0.2.7.tar` & `fixations-0.2.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     2639 2023-02-05 04:22:42.567199 fixations-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-01-01 00:11:58.854979 fixations-0.2.7/fixations/__init__.py
--rwxr-xr-x   0        0        0     1711 2023-01-01 23:58:12.111271 fixations-0.2.7/fixations/fix_parse_log.py
--rw-r--r--   0        0        0     6148 2023-01-01 00:31:51.491830 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/.DS_Store
--rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.484908 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Components.xml
--rw-r--r--   0        0        0     4467 2023-01-01 00:31:51.485401 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Datatypes.xml
--rw-r--r--   0        0        0    42605 2023-01-01 00:31:51.484542 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Enums.xml
--rw-r--r--   0        0        0    34393 2023-01-01 00:31:51.483397 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Fields.xml
--rw-r--r--   0        0        0    13897 2023-01-01 00:31:51.485737 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Messages.xml
--rw-r--r--   0        0        0    90328 2023-01-01 00:31:51.483961 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/MsgContents.xml
--rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.488062 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Components.xml
--rw-r--r--   0        0        0     5193 2023-01-01 00:31:51.488407 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Datatypes.xml
--rw-r--r--   0        0        0    61939 2023-01-01 00:31:51.487702 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Enums.xml
--rw-r--r--   0        0        0    51793 2023-01-01 00:31:51.486758 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Fields.xml
--rw-r--r--   0        0        0    13436 2023-01-01 00:31:51.488717 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Messages.xml
--rw-r--r--   0        0        0   151901 2023-01-01 00:31:51.487249 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/MsgContents.xml
--rw-r--r--   0        0        0     6148 2023-01-01 00:31:51.543284 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/.DS_Store
--rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.545008 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Components.xml
--rw-r--r--   0        0        0     8642 2023-01-01 00:31:51.545304 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Datatypes.xml
--rw-r--r--   0        0        0   107855 2023-01-01 00:31:51.544764 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Enums.xml
--rw-r--r--   0        0        0   100936 2023-01-01 00:31:51.543938 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Fields.xml
--rw-r--r--   0        0        0    21311 2023-01-01 00:31:51.545633 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Messages.xml
--rw-r--r--   0        0        0   377367 2023-01-01 00:31:51.544335 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/MsgContents.xml
--rw-r--r--   0        0        0     8957 2023-01-01 00:31:51.539013 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Components.xml
--rw-r--r--   0        0        0     9900 2023-01-01 00:31:51.539300 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Datatypes.xml
--rw-r--r--   0        0        0   227928 2023-01-01 00:31:51.538730 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Enums.xml
--rw-r--r--   0        0        0   100936 2023-01-01 00:31:51.537633 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Fields.xml
--rw-r--r--   0        0        0    30287 2023-01-01 00:31:51.539531 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Messages.xml
--rw-r--r--   0        0        0   506296 2023-01-01 00:31:51.538248 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/MsgContents.xml
--rw-r--r--   0        0        0    21131 2023-01-01 00:31:51.535623 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Abbreviations.xml
--rw-r--r--   0        0        0     8891 2023-01-01 00:31:51.536603 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Categories.xml
--rw-r--r--   0        0        0    37979 2023-01-01 00:31:51.535949 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Components.xml
--rw-r--r--   0        0        0    21184 2023-01-01 00:31:51.536278 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Datatypes.xml
--rw-r--r--   0        0        0   321003 2023-01-01 00:31:51.532212 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Enums.xml
--rw-r--r--   0        0        0   277743 2023-01-01 00:31:51.530807 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Fields.xml
--rw-r--r--   0        0        0    45168 2023-01-01 00:31:51.536823 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Messages.xml
--rw-r--r--   0        0        0   756773 2023-01-01 00:31:51.531647 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/MsgContents.xml
--rw-r--r--   0        0        0     3904 2023-01-01 00:31:51.535286 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Sections.xml
--rw-r--r--   0        0        0    24484 2023-01-01 00:31:51.551053 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Abbreviations.xml
--rw-r--r--   0        0        0     8894 2023-01-01 00:31:51.551703 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Categories.xml
--rw-r--r--   0        0        0    44411 2023-01-01 00:31:51.551318 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Components.xml
--rw-r--r--   0        0        0    28426 2023-01-01 00:31:51.551513 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Datatypes.xml
--rw-r--r--   0        0        0   521672 2023-01-01 00:31:51.548289 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Enums.xml
--rw-r--r--   0        0        0   338818 2023-01-01 00:31:51.546461 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Fields.xml
--rw-r--r--   0        0        0    58107 2023-01-01 00:31:51.551904 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Messages.xml
--rw-r--r--   0        0        0   995798 2023-01-01 00:31:51.547586 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/MsgContents.xml
--rw-r--r--   0        0        0     3904 2023-01-01 00:31:51.548607 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Sections.xml
--rw-r--r--   0        0        0    27431 2023-01-01 00:31:51.496464 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Abbreviations.xml
--rw-r--r--   0        0        0    11513 2023-01-01 00:31:51.497372 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Categories.xml
--rw-r--r--   0        0        0    57935 2023-01-01 00:31:51.496761 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Components.xml
--rw-r--r--   0        0        0    28526 2023-01-01 00:31:51.497060 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Datatypes.xml
--rw-r--r--   0        0        0   587938 2023-01-01 00:31:51.495582 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Enums.xml
--rw-r--r--   0        0        0   418638 2023-01-01 00:31:51.493356 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Fields.xml
--rw-r--r--   0        0        0    63983 2023-01-01 00:31:51.497693 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Messages.xml
--rw-r--r--   0        0        0  1159920 2023-01-01 00:31:51.494599 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/MsgContents.xml
--rw-r--r--   0        0        0     4255 2023-01-01 00:31:51.496057 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Sections.xml
--rw-r--r--   0        0        0    27448 2023-01-01 00:31:51.555806 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Abbreviations.xml
--rw-r--r--   0        0        0    11792 2023-01-01 00:31:51.556707 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Categories.xml
--rw-r--r--   0        0        0    68147 2023-01-01 00:31:51.556128 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Components.xml
--rw-r--r--   0        0        0    28913 2023-01-01 00:31:51.556459 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Datatypes.xml
--rw-r--r--   0        0        0   628553 2023-01-01 00:31:51.555024 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Enums.xml
--rw-r--r--   0        0        0   447442 2023-01-01 00:31:51.552943 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Fields.xml
--rw-r--r--   0        0        0    66728 2023-01-01 00:31:51.556978 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Messages.xml
--rw-r--r--   0        0        0  1209212 2023-01-01 00:31:51.554173 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/MsgContents.xml
--rw-r--r--   0        0        0     4255 2023-01-01 00:31:51.555474 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Sections.xml
--rw-r--r--   0        0        0    23877 2023-01-01 00:31:51.490592 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Abbreviations.xml
--rw-r--r--   0        0        0    11511 2023-01-01 00:31:51.491294 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Categories.xml
--rw-r--r--   0        0        0     3810 2023-01-01 00:31:51.490847 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Components.xml
--rw-r--r--   0        0        0    18885 2023-01-01 00:31:51.491072 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Datatypes.xml
--rw-r--r--   0        0        0    13507 2023-01-01 00:31:51.490145 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Enums.xml
--rw-r--r--   0        0        0    24625 2023-01-01 00:31:51.489652 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Fields.xml
--rw-r--r--   0        0        0     6307 2023-01-01 00:31:51.491536 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Messages.xml
--rw-r--r--   0        0        0    27964 2023-01-01 00:31:51.489892 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/MsgContents.xml
--rw-r--r--   0        0        0     2906 2023-01-01 00:31:51.490362 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Sections.xml
--rw-r--r--   0        0        0   115801 2023-01-01 00:31:51.516888 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.0_en_phrases.xml
--rw-r--r--   0        0        0   184708 2023-01-01 00:31:51.519683 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.1_en_phrases.xml
--rw-r--r--   0        0        0   413170 2023-01-01 00:31:51.529721 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.2_en_phrases.xml
--rw-r--r--   0        0        0   657848 2023-01-01 00:31:51.522541 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.3_en_phrases.xml
--rw-r--r--   0        0        0   960603 2023-01-01 00:31:51.527317 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.4_en_phrases.xml
--rw-r--r--   0        0        0  1507477 2023-01-01 00:31:51.518751 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP1_en_phrases.xml
--rw-r--r--   0        0        0  1577360 2023-01-01 00:31:51.528913 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP2_en_phrases.xml
--rw-r--r--   0        0        0  1268783 2023-01-01 00:31:51.521548 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0_en_phrases.xml
--rw-r--r--   0        0        0      521 2023-01-01 00:31:51.515126 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIXRepositoryMetadata.xml
--rw-r--r--   0        0        0    78467 2023-01-01 00:31:51.498573 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIXT.1.1_en_phrases.xml
--rw-r--r--   0        0        0  8197493 2023-01-01 00:31:51.506495 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FixRepository.xml
--rw-r--r--   0        0        0      789 2023-01-01 00:31:51.520130 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FixRepositoryMeta.xsd
--rw-r--r--   0        0        0     3057 2023-01-01 00:31:51.540544 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Abbreviations.xsd
--rw-r--r--   0        0        0     3032 2023-01-01 00:31:51.541201 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Categories.xsd
--rw-r--r--   0        0        0     2977 2023-01-01 00:31:51.540341 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Components.xsd
--rw-r--r--   0        0        0     3076 2023-01-01 00:31:51.540149 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Datatypes.xsd
--rw-r--r--   0        0        0     2962 2023-01-01 00:31:51.542811 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Enums.xsd
--rw-r--r--   0        0        0     2965 2023-01-01 00:31:51.541651 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Fields.xsd
--rw-r--r--   0        0        0     2971 2023-01-01 00:31:51.540973 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Messages.xsd
--rw-r--r--   0        0        0     2980 2023-01-01 00:31:51.542242 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/MsgContents.xsd
--rw-r--r--   0        0        0     3028 2023-01-01 00:31:51.542040 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Sections.xsd
--rw-r--r--   0        0        0    30521 2023-01-01 00:31:51.542507 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/extensionpack.xsd
--rw-r--r--   0        0        0    20738 2023-01-01 00:31:51.540770 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/repositorystructures.xsd
--rw-r--r--   0        0        0    10175 2023-01-01 00:31:51.541418 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/repositorytypes.xsd
--rw-r--r--   0        0        0     4514 2023-01-01 00:31:51.541851 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/versions.xsd
--rw-r--r--   0        0        0     1564 2023-01-01 00:31:51.558935 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Abbreviations_2010_to_2009.xsl
--rw-r--r--   0        0        0     2001 2023-01-01 00:31:51.557814 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Categories_2010_to_2009.xsl
--rw-r--r--   0        0        0     1701 2023-01-01 00:31:51.557590 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Components_2010_to_2009.xsl
--rw-r--r--   0        0        0     1591 2023-01-01 00:31:51.558239 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Datatypes_2010_to_2009.xsl
--rw-r--r--   0        0        0     1609 2023-01-01 00:31:51.558754 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Enums_2010_to_2009.xsl
--rw-r--r--   0        0        0     2293 2023-01-01 00:31:51.558574 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Fields_2010_to_2009.xsl
--rw-r--r--   0        0        0     2176 2023-01-01 00:31:51.558402 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Messages_2010_to_2009.xsl
--rw-r--r--   0        0        0     1661 2023-01-01 00:31:51.559273 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_MsgContents_2010_to_2009.xsl
--rw-r--r--   0        0        0     1934 2023-01-01 00:31:51.558061 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Sections_2010_to_2009.xsl
--rw-r--r--   0        0        0     2519 2023-01-01 00:31:51.559110 fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_support.xsl
--rw-r--r--   0        0        0     2342 2023-02-06 23:35:54.250161 fixations-0.2.7/fixations/fix_store.py
--rwxr-xr-x   0        0        0     4081 2023-01-02 01:38:25.424285 fixations-0.2.7/fixations/fix_tags.py
--rw-r--r--   0        0        0    12287 2023-02-05 04:01:23.386549 fixations-0.2.7/fixations/fix_utils.py
--rw-r--r--   0        0        0     1848 2023-02-05 03:52:04.760215 fixations-0.2.7/fixations/short_str_id.py
--rw-r--r--   0        0        0    14042 2023-02-05 04:01:23.392749 fixations-0.2.7/fixations/templates/index.html
--rwxr-xr-x   0        0        0     2079 2023-02-05 04:17:53.663548 fixations-0.2.7/fixations/webfix.py
--rw-r--r--   0        0        0       79 2023-01-02 01:21:27.781766 fixations-0.2.7/fixations/wsgi.py
--rw-r--r--   0        0        0      790 2023-02-06 23:33:25.297890 fixations-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 fixations-0.2.7/setup.py
--rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 fixations-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2639 2023-02-05 04:22:42.567199 fixations-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-01-01 00:11:58.854979 fixations-0.2.8/fixations/__init__.py
+-rwxr-xr-x   0        0        0     1711 2023-01-01 23:58:12.111271 fixations-0.2.8/fixations/fix_parse_log.py
+-rw-r--r--   0        0        0     6148 2023-01-01 00:31:51.491830 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/.DS_Store
+-rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.484908 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Components.xml
+-rw-r--r--   0        0        0     4467 2023-01-01 00:31:51.485401 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Datatypes.xml
+-rw-r--r--   0        0        0    42605 2023-01-01 00:31:51.484542 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Enums.xml
+-rw-r--r--   0        0        0    34393 2023-01-01 00:31:51.483397 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Fields.xml
+-rw-r--r--   0        0        0    13897 2023-01-01 00:31:51.485737 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Messages.xml
+-rw-r--r--   0        0        0    90328 2023-01-01 00:31:51.483961 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/MsgContents.xml
+-rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.488062 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Components.xml
+-rw-r--r--   0        0        0     5193 2023-01-01 00:31:51.488407 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Datatypes.xml
+-rw-r--r--   0        0        0    61939 2023-01-01 00:31:51.487702 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Enums.xml
+-rw-r--r--   0        0        0    51793 2023-01-01 00:31:51.486758 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Fields.xml
+-rw-r--r--   0        0        0    13436 2023-01-01 00:31:51.488717 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Messages.xml
+-rw-r--r--   0        0        0   151901 2023-01-01 00:31:51.487249 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/MsgContents.xml
+-rw-r--r--   0        0        0     6148 2023-01-01 00:31:51.543284 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/.DS_Store
+-rw-r--r--   0        0        0     3194 2023-01-01 00:31:51.545008 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Components.xml
+-rw-r--r--   0        0        0     8642 2023-01-01 00:31:51.545304 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Datatypes.xml
+-rw-r--r--   0        0        0   107855 2023-01-01 00:31:51.544764 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Enums.xml
+-rw-r--r--   0        0        0   100936 2023-01-01 00:31:51.543938 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Fields.xml
+-rw-r--r--   0        0        0    21311 2023-01-01 00:31:51.545633 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Messages.xml
+-rw-r--r--   0        0        0   377367 2023-01-01 00:31:51.544335 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/MsgContents.xml
+-rw-r--r--   0        0        0     8957 2023-01-01 00:31:51.539013 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Components.xml
+-rw-r--r--   0        0        0     9900 2023-01-01 00:31:51.539300 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Datatypes.xml
+-rw-r--r--   0        0        0   227928 2023-01-01 00:31:51.538730 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Enums.xml
+-rw-r--r--   0        0        0   100936 2023-01-01 00:31:51.537633 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Fields.xml
+-rw-r--r--   0        0        0    30287 2023-01-01 00:31:51.539531 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Messages.xml
+-rw-r--r--   0        0        0   506296 2023-01-01 00:31:51.538248 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/MsgContents.xml
+-rw-r--r--   0        0        0    21131 2023-01-01 00:31:51.535623 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Abbreviations.xml
+-rw-r--r--   0        0        0     8891 2023-01-01 00:31:51.536603 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Categories.xml
+-rw-r--r--   0        0        0    37979 2023-01-01 00:31:51.535949 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Components.xml
+-rw-r--r--   0        0        0    21184 2023-01-01 00:31:51.536278 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Datatypes.xml
+-rw-r--r--   0        0        0   321003 2023-01-01 00:31:51.532212 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Enums.xml
+-rw-r--r--   0        0        0   277743 2023-01-01 00:31:51.530807 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Fields.xml
+-rw-r--r--   0        0        0    45168 2023-01-01 00:31:51.536823 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Messages.xml
+-rw-r--r--   0        0        0   756773 2023-01-01 00:31:51.531647 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/MsgContents.xml
+-rw-r--r--   0        0        0     3904 2023-01-01 00:31:51.535286 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Sections.xml
+-rw-r--r--   0        0        0    24484 2023-01-01 00:31:51.551053 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Abbreviations.xml
+-rw-r--r--   0        0        0     8894 2023-01-01 00:31:51.551703 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Categories.xml
+-rw-r--r--   0        0        0    44411 2023-01-01 00:31:51.551318 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Components.xml
+-rw-r--r--   0        0        0    28426 2023-01-01 00:31:51.551513 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Datatypes.xml
+-rw-r--r--   0        0        0   521672 2023-01-01 00:31:51.548289 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Enums.xml
+-rw-r--r--   0        0        0   338818 2023-01-01 00:31:51.546461 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Fields.xml
+-rw-r--r--   0        0        0    58107 2023-01-01 00:31:51.551904 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Messages.xml
+-rw-r--r--   0        0        0   995798 2023-01-01 00:31:51.547586 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/MsgContents.xml
+-rw-r--r--   0        0        0     3904 2023-01-01 00:31:51.548607 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Sections.xml
+-rw-r--r--   0        0        0    27431 2023-01-01 00:31:51.496464 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Abbreviations.xml
+-rw-r--r--   0        0        0    11513 2023-01-01 00:31:51.497372 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Categories.xml
+-rw-r--r--   0        0        0    57935 2023-01-01 00:31:51.496761 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Components.xml
+-rw-r--r--   0        0        0    28526 2023-01-01 00:31:51.497060 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Datatypes.xml
+-rw-r--r--   0        0        0   587938 2023-01-01 00:31:51.495582 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Enums.xml
+-rw-r--r--   0        0        0   418638 2023-01-01 00:31:51.493356 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Fields.xml
+-rw-r--r--   0        0        0    63983 2023-01-01 00:31:51.497693 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Messages.xml
+-rw-r--r--   0        0        0  1159920 2023-01-01 00:31:51.494599 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/MsgContents.xml
+-rw-r--r--   0        0        0     4255 2023-01-01 00:31:51.496057 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Sections.xml
+-rw-r--r--   0        0        0    27448 2023-01-01 00:31:51.555806 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Abbreviations.xml
+-rw-r--r--   0        0        0    11792 2023-01-01 00:31:51.556707 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Categories.xml
+-rw-r--r--   0        0        0    68147 2023-01-01 00:31:51.556128 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Components.xml
+-rw-r--r--   0        0        0    28913 2023-01-01 00:31:51.556459 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Datatypes.xml
+-rw-r--r--   0        0        0   628553 2023-01-01 00:31:51.555024 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Enums.xml
+-rw-r--r--   0        0        0   447442 2023-01-01 00:31:51.552943 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Fields.xml
+-rw-r--r--   0        0        0    66728 2023-01-01 00:31:51.556978 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Messages.xml
+-rw-r--r--   0        0        0  1209212 2023-01-01 00:31:51.554173 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/MsgContents.xml
+-rw-r--r--   0        0        0     4255 2023-01-01 00:31:51.555474 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Sections.xml
+-rw-r--r--   0        0        0    23877 2023-01-01 00:31:51.490592 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Abbreviations.xml
+-rw-r--r--   0        0        0    11511 2023-01-01 00:31:51.491294 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Categories.xml
+-rw-r--r--   0        0        0     3810 2023-01-01 00:31:51.490847 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Components.xml
+-rw-r--r--   0        0        0    18885 2023-01-01 00:31:51.491072 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Datatypes.xml
+-rw-r--r--   0        0        0    13507 2023-01-01 00:31:51.490145 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Enums.xml
+-rw-r--r--   0        0        0    24625 2023-01-01 00:31:51.489652 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Fields.xml
+-rw-r--r--   0        0        0     6307 2023-01-01 00:31:51.491536 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Messages.xml
+-rw-r--r--   0        0        0    27964 2023-01-01 00:31:51.489892 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/MsgContents.xml
+-rw-r--r--   0        0        0     2906 2023-01-01 00:31:51.490362 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Sections.xml
+-rw-r--r--   0        0        0   115801 2023-01-01 00:31:51.516888 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.0_en_phrases.xml
+-rw-r--r--   0        0        0   184708 2023-01-01 00:31:51.519683 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.1_en_phrases.xml
+-rw-r--r--   0        0        0   413170 2023-01-01 00:31:51.529721 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.2_en_phrases.xml
+-rw-r--r--   0        0        0   657848 2023-01-01 00:31:51.522541 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.3_en_phrases.xml
+-rw-r--r--   0        0        0   960603 2023-01-01 00:31:51.527317 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.4_en_phrases.xml
+-rw-r--r--   0        0        0  1507477 2023-01-01 00:31:51.518751 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP1_en_phrases.xml
+-rw-r--r--   0        0        0  1577360 2023-01-01 00:31:51.528913 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP2_en_phrases.xml
+-rw-r--r--   0        0        0  1268783 2023-01-01 00:31:51.521548 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0_en_phrases.xml
+-rw-r--r--   0        0        0      521 2023-01-01 00:31:51.515126 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIXRepositoryMetadata.xml
+-rw-r--r--   0        0        0    78467 2023-01-01 00:31:51.498573 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIXT.1.1_en_phrases.xml
+-rw-r--r--   0        0        0  8197493 2023-01-01 00:31:51.506495 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FixRepository.xml
+-rw-r--r--   0        0        0      789 2023-01-01 00:31:51.520130 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FixRepositoryMeta.xsd
+-rw-r--r--   0        0        0     3057 2023-01-01 00:31:51.540544 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Abbreviations.xsd
+-rw-r--r--   0        0        0     3032 2023-01-01 00:31:51.541201 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Categories.xsd
+-rw-r--r--   0        0        0     2977 2023-01-01 00:31:51.540341 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Components.xsd
+-rw-r--r--   0        0        0     3076 2023-01-01 00:31:51.540149 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Datatypes.xsd
+-rw-r--r--   0        0        0     2962 2023-01-01 00:31:51.542811 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Enums.xsd
+-rw-r--r--   0        0        0     2965 2023-01-01 00:31:51.541651 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Fields.xsd
+-rw-r--r--   0        0        0     2971 2023-01-01 00:31:51.540973 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Messages.xsd
+-rw-r--r--   0        0        0     2980 2023-01-01 00:31:51.542242 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/MsgContents.xsd
+-rw-r--r--   0        0        0     3028 2023-01-01 00:31:51.542040 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Sections.xsd
+-rw-r--r--   0        0        0    30521 2023-01-01 00:31:51.542507 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/extensionpack.xsd
+-rw-r--r--   0        0        0    20738 2023-01-01 00:31:51.540770 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/repositorystructures.xsd
+-rw-r--r--   0        0        0    10175 2023-01-01 00:31:51.541418 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/repositorytypes.xsd
+-rw-r--r--   0        0        0     4514 2023-01-01 00:31:51.541851 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/versions.xsd
+-rw-r--r--   0        0        0     1564 2023-01-01 00:31:51.558935 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Abbreviations_2010_to_2009.xsl
+-rw-r--r--   0        0        0     2001 2023-01-01 00:31:51.557814 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Categories_2010_to_2009.xsl
+-rw-r--r--   0        0        0     1701 2023-01-01 00:31:51.557590 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Components_2010_to_2009.xsl
+-rw-r--r--   0        0        0     1591 2023-01-01 00:31:51.558239 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Datatypes_2010_to_2009.xsl
+-rw-r--r--   0        0        0     1609 2023-01-01 00:31:51.558754 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Enums_2010_to_2009.xsl
+-rw-r--r--   0        0        0     2293 2023-01-01 00:31:51.558574 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Fields_2010_to_2009.xsl
+-rw-r--r--   0        0        0     2176 2023-01-01 00:31:51.558402 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Messages_2010_to_2009.xsl
+-rw-r--r--   0        0        0     1661 2023-01-01 00:31:51.559273 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_MsgContents_2010_to_2009.xsl
+-rw-r--r--   0        0        0     1934 2023-01-01 00:31:51.558061 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Sections_2010_to_2009.xsl
+-rw-r--r--   0        0        0     2519 2023-01-01 00:31:51.559110 fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_support.xsl
+-rw-r--r--   0        0        0     2342 2023-02-06 23:35:54.250161 fixations-0.2.8/fixations/fix_store.py
+-rwxr-xr-x   0        0        0     4081 2023-01-02 01:38:25.424285 fixations-0.2.8/fixations/fix_tags.py
+-rw-r--r--   0        0        0    12289 2023-02-07 00:00:13.880829 fixations-0.2.8/fixations/fix_utils.py
+-rw-r--r--   0        0        0     1848 2023-02-05 03:52:04.760215 fixations-0.2.8/fixations/short_str_id.py
+-rw-r--r--   0        0        0    14042 2023-02-05 04:01:23.392749 fixations-0.2.8/fixations/templates/index.html
+-rwxr-xr-x   0        0        0     2079 2023-02-05 04:17:53.663548 fixations-0.2.8/fixations/webfix.py
+-rw-r--r--   0        0        0       79 2023-01-02 01:21:27.781766 fixations-0.2.8/fixations/wsgi.py
+-rw-r--r--   0        0        0      788 2023-02-07 00:13:31.013553 fixations-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 fixations-0.2.8/setup.py
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 fixations-0.2.8/PKG-INFO
```

### Comparing `fixations-0.2.7/README.md` & `fixations-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_parse_log.py` & `fixations-0.2.8/fixations/fix_parse_log.py`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/.DS_Store` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/.DS_Store`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.0/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.1/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/.DS_Store` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.2/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.3/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Abbreviations.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Abbreviations.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Categories.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Categories.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Sections.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.4.4/Base/Sections.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Abbreviations.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Abbreviations.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Categories.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Categories.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Sections.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0/Base/Sections.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Abbreviations.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Abbreviations.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Categories.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Categories.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Sections.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP1/Base/Sections.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Abbreviations.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Abbreviations.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Categories.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Categories.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Sections.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIX.5.0SP2/Base/Sections.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Abbreviations.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Abbreviations.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Categories.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Categories.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Components.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Components.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Datatypes.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Datatypes.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Enums.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Enums.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Fields.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Fields.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Messages.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Messages.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/MsgContents.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/MsgContents.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Sections.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/FIXT.1.1/Base/Sections.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.0_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.0_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.1_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.1_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.2_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.2_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.3_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.3_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.4_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.4.4_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP1_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP1_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP2_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0SP2_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIX.5.0_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIXRepositoryMetadata.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIXRepositoryMetadata.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FIXT.1.1_en_phrases.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FIXT.1.1_en_phrases.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FixRepository.xml` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FixRepository.xml`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/Unified/FixRepositoryMeta.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/Unified/FixRepositoryMeta.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Abbreviations.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Abbreviations.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Categories.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Categories.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Components.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Components.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Datatypes.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Datatypes.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Enums.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Enums.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Fields.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Fields.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Messages.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Messages.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/MsgContents.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/MsgContents.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/Sections.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/Sections.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/extensionpack.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/extensionpack.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/repositorystructures.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/repositorystructures.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/repositorytypes.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/repositorytypes.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/schema/versions.xsd` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/schema/versions.xsd`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Abbreviations_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Abbreviations_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Categories_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Categories_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Components_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Components_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Datatypes_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Datatypes_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Enums_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Enums_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Fields_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Fields_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Messages_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Messages_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_MsgContents_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_MsgContents_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Sections_2010_to_2009.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_Sections_2010_to_2009.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_repository_2010_edition_20200402/xsl/Translate_support.xsl` & `fixations-0.2.8/fixations/fix_repository_2010_edition_20200402/xsl/Translate_support.xsl`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_store.py` & `fixations-0.2.8/fixations/fix_store.py`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_tags.py` & `fixations-0.2.8/fixations/fix_tags.py`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/fix_utils.py` & `fixations-0.2.8/fixations/fix_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 def extract_elements_from_file_by_tag_name(fix_version, file, tag_name):
     fields_file = path_for_fix_path(fix_version, file)
     doc = parse(fields_file)
     elements = doc.getElementsByTagName(tag_name)
     return elements
 
 
-@cache
+# @cache
 def extract_tag_dict_for_fix_version(fix_version=DEFAULT_FIX_VERSION):
     versions = get_list_of_available_fix_versions()
     assert fix_version in versions, f"The specified FIX version:{fix_version} is not valid. Use one of these {versions}"
 
     # Extract all FIX tags from Fields XML file
     fields = extract_elements_from_file_by_tag_name(fix_version, "Fields.xml", "Field")
     tag_dict_by_id = {}
```

### Comparing `fixations-0.2.7/fixations/short_str_id.py` & `fixations-0.2.8/fixations/short_str_id.py`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/templates/index.html` & `fixations-0.2.8/fixations/templates/index.html`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/fixations/webfix.py` & `fixations-0.2.8/fixations/webfix.py`

 * *Files identical despite different names*

### Comparing `fixations-0.2.7/pyproject.toml` & `fixations-0.2.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "fixations"
-version = "0.2.7"
+version = "0.2.8"
 description = "This is a set of tools to look up / visualize FIX protocol data"
 authors = ["Jerome Provensal <jeromegit@provensal.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["fix", "fix-protocol"]
 homepage = "https://github.com/jeromegit/fixations"
 include = ["fix_repository_2010_edition_20200402"]
 
 [tool.poetry.scripts]
 fix_parse_log = 'fixations.fix_parse_log:main'
 fix_tags = 'fixations.fix_tags:main'
 webfix = 'fixations.webfix:main'
 
 [tool.poetry.dependencies]
-python = "^3.6.5"
+python = "^3.7"
 flask = "^2.2.2"
 gunicorn = "^20.1.0"
 tabulate = "^0.9.0"
 urwid = "^2.1.2"
 termcolor = "^2.1.1"
 dataclasses-json = "^0.5.7"
 pytest = "^7.2.0"
```

### Comparing `fixations-0.2.7/setup.py` & `fixations-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 entry_points = \
 {'console_scripts': ['fix_parse_log = fixations.fix_parse_log:main',
                      'fix_tags = fixations.fix_tags:main',
                      'webfix = fixations.webfix:main']}
 
 setup_kwargs = {
     'name': 'fixations',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'This is a set of tools to look up / visualize FIX protocol data',
     'long_description': '# FIXations!\n## A set of tools to handle FIX protocol data\n - **fix_tags** - _explore FIX tags and their associated values either as CLI output or a GUI-like textual interface_\n - **fix_parse_log** - _extract FIX lines from a (log) file and present them in a nicely formatted grid_\n - **webfix** - _present copy-n-paste\'d FIX lines into a nicely formatted grid_\n\n### Installation\n`pip3 install fixations`\n\n### Examples of running these applications\n#### fix_tags\n_Click on the link below since it was too small to asciicast in this page_\n[![asciicast](https://asciinema.org/a/551910.svg)](https://asciinema.org/a/551910?autoplay=1&t=2)\n\n#### fix_parse_log\n![fix_parse_log_demo](images/fix_parse_log_demo.gif)\n\n#### webfix\nWebfix needs to be used with either Flask (for dev purposes) \n```commandline\n$ python -m flask --app fixations.webfix run\n * Serving Flask app \'fixations.webfix\'\n * Debug mode: off\nWARNING: This is a development server. Do not use it in a production deployment. \nUse a production WSGI server instead.\n * Running on http://127.0.0.1:5000\nPress CTRL+C to quit\n```\n\nor something like gunicorn (or other WSGI servers) for production uses:\n```commandline\n$ gunicorn fixations.wsgi:app\n[2023-01-16 19:55:31 -0500] [3380019] [INFO] Starting gunicorn 20.1.0\n[2023-01-16 19:55:31 -0500] [3380019] [INFO] Listening at: http://127.0.0.1:8000 (3380019)\n[2023-01-16 19:55:31 -0500] [3380019] [INFO] Using worker: sync\n[2023-01-16 19:55:31 -0500] [3380028] [INFO] Booting worker with pid: 3380028\n```\n\n![webfix_session](images/webfix_session.png)\n\n\n## FIX reference data source\nThe data is extracted from the FIX specs available here: \n\n> https://www.fixtrading.org/packages/fix-repository-2010/ \n(see fix_repository_2010_edition_20200402.zip).\n\nNOTE: it requires the creation of a login/password to access it.\n\n## TODO:\n 1. create hyperlink to FIX specs for each tag based on FIX version\n 2. [DONE] add more info to README.md. Use rule80A and 47 as example for fix_args\n 3. add more example(s)\n 4. add some pytest to detect the FIX version for example\n 5. add "direction" to columns to show whether it\'s a request or a response\n 6. catch exceptions and display them into the webpage\n 7. deploy to https://vercel.com/\n 8. allow to create an ASCII table equivalent suitable to be cut-n-paste into a document for exanple\n 9. [DONE] add shortlink ala tinyurl and save it into a sqlite3 db store\n 10. black theme?\n 11. [DONE] allow to have no leading timestamp and use the timestamp FIX tags instead\n 12. add proper Logger\n 13. add DB stats\n 14. pypi.org can\'t display the ASCII screencast images. Need to reference github full path?\n\n',
     'author': 'Jerome Provensal',
     'author_email': 'jeromegit@provensal.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeromegit/fixations',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.5,<4.0.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fixations-0.2.7/PKG-INFO` & `fixations-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fixations
-Version: 0.2.7
+Version: 0.2.8
 Summary: This is a set of tools to look up / visualize FIX protocol data
 Home-page: https://github.com/jeromegit/fixations
 License: GPL-3.0-or-later
 Keywords: fix,fix-protocol
 Author: Jerome Provensal
 Author-email: jeromegit@provensal.com
-Requires-Python: >=3.6.5,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

