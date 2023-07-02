# Comparing `tmp/cikuu-2022.8.7.tar.gz` & `tmp/cikuu-2022.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cikuu-2022.8.7.tar", last modified: Sun Jul  2 09:59:02 2023, max compression
+gzip compressed data, was "cikuu-2022.8.8.tar", last modified: Sun Jul  2 10:24:49 2023, max compression
```

## Comparing `cikuu-2022.8.7.tar` & `cikuu-2022.8.8.tar`

### file list

```diff
@@ -1,384 +1,384 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.728407 cikuu-2022.8.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.7/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 09:59:02.728407 cikuu-2022.8.7/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.632407 cikuu-2022.8.7/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.7/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.7/api/c4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.7/api/chunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.7/api/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.7/api/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.7/api/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.7/api/feishu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.7/api/mynac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.7/api/sntjson-es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.7/api/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.7/api/wget.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.632407 cikuu-2022.8.7/app/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.7/app/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.632407 cikuu-2022.8.7/app/dmdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.7/app/dmdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.7/app/dmdsk/app_navbar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.636407 cikuu-2022.8.7/app/dmdsk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.7/app/dmdsk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.7/app/dmdsk/func/dim-awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.7/app/dmdsk/func/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.7/app/dmdsk/func/eidv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.7/app/dmdsk/func/feedback.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.7/app/dmdsk/func/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.7/app/dmdsk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.7/app/dmdsk/func/scores.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.7/app/dmdsk/func/sent.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.7/app/dmdsk/func/trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.7/app/dmdsk/index.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.636407 cikuu-2022.8.7/cikuu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 09:59:02.000000 cikuu-2022.8.7/cikuu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6426 2023-07-02 09:59:02.000000 cikuu-2022.8.7/cikuu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 09:59:02.000000 cikuu-2022.8.7/cikuu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 09:59:02.000000 cikuu-2022.8.7/cikuu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-02 09:59:02.000000 cikuu-2022.8.7/cikuu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.692407 cikuu-2022.8.7/dic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.7/dic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.7/dic/adjlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.7/dic/advlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.7/dic/bnc_wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.7/dic/confu_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/ecdic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/errants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/lemma_lex.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/lemma_mf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/lemma_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/lex_lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/mwe_disconj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/mwe_pv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/n_is_sb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/nounlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/nyt_wc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/oneself.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/orals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/poslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/propbank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/stoplist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/to_redislite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/verbform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/verblist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/verbtag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/vocab.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43159 2023-05-08 05:59:19.000000 cikuu-2022.8.7/dic/word_awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/word_bits.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/word_grade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/word_gsl1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/word_gsl2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.7/dic/word_idf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/word_oov.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/word_pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/word_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.7/dic/wordattr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/wordcnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.7/dic/wordlist_ed1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.7/dic/wordnet_verb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/wordpos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dic/words.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3470 2023-07-02 09:59:00.000000 cikuu-2022.8.7/dic/yulk.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.696407 cikuu-2022.8.7/dsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.7/dsk/dsk-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.7/dsk/dsk-req.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/dsk-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.7/dsk/dsk2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/dskapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/dskes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/dskmkf_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/dsktrain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/essaydm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/gears-xdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/gecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/innersim.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/json-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/kvrdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/mkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/mqconsume.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/pingyu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/sntsdims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/tok-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/uvidsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/wps-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.7/dsk/wps-xgec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11422 2023-05-11 14:49:06.000000 cikuu-2022.8.7/dsk/wps7000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/xessay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/xgecv1-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.7/dsk/xgecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.7/dsk/xmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/xsnt-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.7/dsk/xsnt-spacy.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.704407 cikuu-2022.8.7/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.7/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/annotate.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.704407 cikuu-2022.8.7/en/arc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/arc/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/arc/sntjson-innodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/arc/sntjson-naclite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/arc/sntjson-naclite0.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/arc/sntjson-nacp-20230206.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/arc/sntjson-nacp-20230207.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/c4-gram-upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-grams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/c4-postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4down.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/c4gram-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4gram-upsert.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4gramcl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/c4matcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4skenp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/c4tree.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/c4vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/clause.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/docfts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/docjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.7/en/en-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.7/en/es-index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/esbulk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/esfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/exchunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/exphrase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/extrp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/havc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/kpsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/lempostag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13757 2023-07-02 09:34:40.000000 cikuu-2022.8.7/en/nacp-kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.7/en/nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/nlp-lit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/nlp-lmdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/shav.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/silite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/snt-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-07-02 09:34:39.000000 cikuu-2022.8.7/en/snt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.7/en/sntjson-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.7/en/sntjson-kpsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/sntjson-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/sntjson-nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/sntjson-parse-snt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/sntjson-si.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/sntjson-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.7/en/sntjson-topk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.7/en/sntjson-tosnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/sntjson-trpx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/sntjson-vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/spacybs-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/spacybs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/spider-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/sqlsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/terms.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/verbnet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.7/en/xsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.7/en/zset-load.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.704407 cikuu-2022.8.7/gecdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.7/gecdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.7/gecdsk/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-11 08:23:32.000000 cikuu-2022.8.7/gecdsk/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      943 2023-05-11 09:20:53.000000 cikuu-2022.8.7/gecdsk/paravs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.708407 cikuu-2022.8.7/lit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.708407 cikuu-2022.8.7/lit/es/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.7/lit/es/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.7/lit/es/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.7/lit/essay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/filling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/fillmul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/hello-pages.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.7/lit/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/mock-scoring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.708407 cikuu-2022.8.7/lit/penly/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/penly/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/penly/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/penly-resend.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/redis-dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.7/lit/reorder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.7/lit/sntspolish.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/sntupgrade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/student-input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/teacher-admin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.708407 cikuu-2022.8.7/lit/yulk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/yulk/YULK.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/yulk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/yulk/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.712407 cikuu-2022.8.7/lit/yulk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/bipos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/cola.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/corpuslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/eshyb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/given-expect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/gramx-single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/lemvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/posvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/style-in-mul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/style.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/wcloud.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.7/lit/yulk/func/wordrank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.7/lit/yulk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.7/lit/yulk/lemma.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.712407 cikuu-2022.8.7/pipe/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.7/pipe/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.7/pipe/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.7/pipe/redisgec8180.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.7/pipe/xgecv1.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.712407 cikuu-2022.8.7/rabbitmq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.7/rabbitmq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.712407 cikuu-2022.8.7/redisr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.7/redisr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.7/redisr/glove-get.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.7/redisr/glove.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.7/redisr/sntvec-get.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.712407 cikuu-2022.8.7/sbert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.7/sbert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.7/sbert/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.7/sbert/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.7/sbert/redis-sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.7/sbert/sntvec-so.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.7/sbert/sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 09:59:02.728407 cikuu-2022.8.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2023-07-02 09:59:00.000000 cikuu-2022.8.7/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.716407 cikuu-2022.8.7/so/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32507 2023-06-05 12:14:25.000000 cikuu-2022.8.7/so/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.7/so/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4772 2023-05-18 10:12:50.000000 cikuu-2022.8.7/so/batch-dis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-05-19 02:35:35.000000 cikuu-2022.8.7/so/batch-sntspacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-11 14:51:44.000000 cikuu-2022.8.7/so/dis-bnc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1259 2023-05-11 14:51:44.000000 cikuu-2022.8.7/so/dis-eev.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.7/so/dis-essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.7/so/dis-folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-09 13:44:41.000000 cikuu-2022.8.7/so/dis-tosnts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.7/so/dsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1812 2023-05-22 02:37:54.000000 cikuu-2022.8.7/so/dump-pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-05-22 07:12:30.000000 cikuu-2022.8.7/so/dump-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.7/so/folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.7/so/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.7/so/loades.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-09 12:36:44.000000 cikuu-2022.8.7/so/tok-idf.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.716407 cikuu-2022.8.7/sqlite/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.7/sqlite/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.7/sqlite/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.720407 cikuu-2022.8.7/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-15 02:53:44.000000 cikuu-2022.8.7/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/annotate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/bcp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/c4data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/client-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/client-xwps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/clientx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/dsk-util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/fire-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/mq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/nldp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/pubsub-sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/pubsub2api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/sent-diff.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/spider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/sqlitedict-load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/wps-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/wps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/xfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/xgec-blpop120.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/xrange.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/xsnt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.7/util/xstream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.7/util/xtest-params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.7/util/xtest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.720407 cikuu-2022.8.7/uviapp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.7/uviapp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.724407 cikuu-2022.8.7/uvirun/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/Jinja2-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/c4es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/c4gramsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/cos_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.7/uvirun/demo_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23119 2023-05-11 08:35:49.000000 cikuu-2022.8.7/uvirun/dsk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/echart_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/elastic_fastapi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.724407 cikuu-2022.8.7/uvirun/errant/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/alignment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/errant/annotator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.724407 cikuu-2022.8.7/uvirun/errant/commands/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/commands/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/errant/commands/compare_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.7/uvirun/errant/commands/m2_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/commands/parallel_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/errant/edit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:59:02.724407 cikuu-2022.8.7/uvirun/errant/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.7/uvirun/errant/en/classifier.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/errant/en/lancaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/errant/en/merger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/errant_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/es1_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.7/uvirun/es_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/essay_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.7/uvirun/exchunk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/feishu_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/flair_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/fusion_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/gec_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/gec_fastapi_33000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/gensim_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.7/uvirun/gramx_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/hnswlib_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/kenlm_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/kpsi_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/kvr_dskdm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/kvr_dskdm1230.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/nldp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/nltk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/nsp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.7/uvirun/penlykvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.7/uvirun/sbert_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/single_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32688 2023-05-08 12:37:28.000000 cikuu-2022.8.7/uvirun/spacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4644 2023-05-10 06:34:51.000000 cikuu-2022.8.7/uvirun/textacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.7/uvirun/trans_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/unmasker_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.7/uvirun/util_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.7/uvirun/uviredis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.7/uvirun/yulk-nac.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.8/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 10:24:49.678426 cikuu-2022.8.8/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/c4.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/chunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.8/api/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/feishu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.8/api/mynac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/sntjson-es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/wget.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/dmdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/app_navbar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/dmdsk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/dim-awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/func/eidv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/feedback.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/func/scores.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/sent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/index.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/cikuu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6426 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.642426 cikuu-2022.8.8/dic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.8/dic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.8/dic/adjlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.8/dic/advlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.8/dic/bnc_wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.8/dic/confu_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/ecdic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/errants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_lex.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_mf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lex_lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/mwe_disconj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/mwe_pv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/n_is_sb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/nounlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/nyt_wc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/oneself.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/orals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/poslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/propbank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/stoplist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/to_redislite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/verbform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/verblist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/verbtag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/vocab.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43159 2023-05-08 05:59:19.000000 cikuu-2022.8.8/dic/word_awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_bits.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_grade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_gsl1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_gsl2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/word_idf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_oov.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/wordattr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordcnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/wordlist_ed1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/wordnet_verb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordpos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/words.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3636 2023-07-02 10:24:46.000000 cikuu-2022.8.8/dic/yulk.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.646426 cikuu-2022.8.8/dsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.8/dsk/dsk-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.8/dsk/dsk-req.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dsk-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.8/dsk/dsk2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dskapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskmkf_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dsktrain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/essaydm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/gears-xdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/gecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/innersim.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/json-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/kvrdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/mkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/mqconsume.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/pingyu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/score.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/sntsdims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/tok-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/uvidsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/wps-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.8/dsk/wps-xgec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11422 2023-05-11 14:49:06.000000 cikuu-2022.8.8/dsk/wps7000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xessay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xgecv1-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.8/dsk/xgecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/xmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xsnt-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xsnt-spacy.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.8/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/annotate.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/en/arc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-innodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-naclite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/arc/sntjson-naclite0.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-nacp-20230206.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-nacp-20230207.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4-gram-upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-grams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4-postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4down.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4gram-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gram-upsert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gramcl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4matcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4skenp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4tree.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/clause.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/docfts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/docjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.8/en/en-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.8/en/es-index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/esbulk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/esfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/exchunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/exphrase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/extrp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/havc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/kpsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/lempostag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13757 2023-07-02 09:34:40.000000 cikuu-2022.8.8/en/nacp-kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/nlp-lit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/nlp-lmdb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/shav.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/silite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/snt-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-07-02 09:34:39.000000 cikuu-2022.8.8/en/snt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/sntjson-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/sntjson-kpsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-parse-snt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sntjson-si.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.8/en/sntjson-topk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.8/en/sntjson-tosnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-trpx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sntjson-vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spacybs-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spacybs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spider-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sqlsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/terms.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/verbnet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/xsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/zset-load.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/gecdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.8/gecdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.8/gecdsk/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-11 08:23:32.000000 cikuu-2022.8.8/gecdsk/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      943 2023-05-11 09:20:53.000000 cikuu-2022.8.8/gecdsk/paravs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/es/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.8/lit/es/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.8/lit/es/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/essay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/filling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/fillmul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/hello-pages.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/mock-scoring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/penly/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/penly/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/penly/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/penly-resend.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/redis-dump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/reorder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/restore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/scoring.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/sntspolish.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/sntupgrade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/student-input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/teacher-admin.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/lit/yulk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/YULK.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/lit/yulk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/bipos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/cola.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/corpuslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/eshyb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/given-expect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/gramx-single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/lemvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/posvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/style-in-mul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/style.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/wcloud.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/wordrank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/yulk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/lemma.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/pipe/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.8/pipe/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.8/pipe/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.8/pipe/redisgec8180.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.8/pipe/xgecv1.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/rabbitmq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.8/rabbitmq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/redisr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.8/redisr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.8/redisr/glove-get.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.8/redisr/glove.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.8/redisr/sntvec-get.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/sbert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.8/sbert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.8/sbert/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.8/sbert/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.8/sbert/redis-sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.8/sbert/sntvec-so.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.8/sbert/sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 10:24:49.678426 cikuu-2022.8.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2023-07-02 10:24:46.000000 cikuu-2022.8.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/so/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32507 2023-06-05 12:14:25.000000 cikuu-2022.8.8/so/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.8/so/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4772 2023-05-18 10:12:50.000000 cikuu-2022.8.8/so/batch-dis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-05-19 02:35:35.000000 cikuu-2022.8.8/so/batch-sntspacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-11 14:51:44.000000 cikuu-2022.8.8/so/dis-bnc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1259 2023-05-11 14:51:44.000000 cikuu-2022.8.8/so/dis-eev.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.8/so/dis-essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.8/so/dis-folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-09 13:44:41.000000 cikuu-2022.8.8/so/dis-tosnts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.8/so/dsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1812 2023-05-22 02:37:54.000000 cikuu-2022.8.8/so/dump-pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-05-22 07:12:30.000000 cikuu-2022.8.8/so/dump-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.8/so/folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.8/so/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.8/so/loades.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-09 12:36:44.000000 cikuu-2022.8.8/so/tok-idf.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/sqlite/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.8/sqlite/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.8/sqlite/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.670426 cikuu-2022.8.8/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-15 02:53:44.000000 cikuu-2022.8.8/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/annotate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/bcp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/c4data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/client-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/client-xwps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/clientx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/dsk-util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/fire-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/mq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/nldp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/pubsub-sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/pubsub2api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/sent-diff.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/spider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/sqlitedict-load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/wps-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/wps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/xfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/xgec-blpop120.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xrange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xsnt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/xstream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/xtest-params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xtest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.670426 cikuu-2022.8.8/uviapp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.8/uviapp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.674426 cikuu-2022.8.8/uvirun/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/Jinja2-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/c4es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/c4gramsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/cos_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.8/uvirun/demo_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23119 2023-05-11 08:35:49.000000 cikuu-2022.8.8/uvirun/dsk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/echart_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/elastic_fastapi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.674426 cikuu-2022.8.8/uvirun/errant/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/alignment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/annotator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/uvirun/errant/commands/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/commands/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/errant/commands/compare_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.8/uvirun/errant/commands/m2_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/commands/parallel_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/edit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/uvirun/errant/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/en/classifier.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/en/lancaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/en/merger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/errant_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/es1_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.8/uvirun/es_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/essay_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.8/uvirun/exchunk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/feishu_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/flair_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/fusion_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/gec_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/gec_fastapi_33000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/gensim_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.8/uvirun/gramx_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/hnswlib_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/kenlm_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/kpsi_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/kvr_dskdm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/kvr_dskdm1230.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/nldp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/nltk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/nsp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.8/uvirun/penlykvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.8/uvirun/sbert_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/single_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32688 2023-05-08 12:37:28.000000 cikuu-2022.8.8/uvirun/spacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4644 2023-05-10 06:34:51.000000 cikuu-2022.8.8/uvirun/textacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/trans_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/unmasker_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/util_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/uviredis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.8/uvirun/yulk-nac.py
```

### Comparing `cikuu-2022.8.7/api/c4.py` & `cikuu-2022.8.8/api/c4.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/chunk.py` & `cikuu-2022.8.8/api/chunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/common.py` & `cikuu-2022.8.8/api/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/dm.py` & `cikuu-2022.8.8/api/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/es.py` & `cikuu-2022.8.8/api/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/feishu.py` & `cikuu-2022.8.8/api/feishu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/mynac.py` & `cikuu-2022.8.8/api/mynac.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/sntjson-es.py` & `cikuu-2022.8.8/api/sntjson-es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/api/wget.py` & `cikuu-2022.8.8/api/wget.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/app/dmdsk/__init__.py` & `cikuu-2022.8.8/app/dmdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/app/dmdsk/app_navbar.py` & `cikuu-2022.8.8/app/dmdsk/app_navbar.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/app/dmdsk/func/lemma.py` & `cikuu-2022.8.8/app/dmdsk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/app/dmdsk/func/trp.py` & `cikuu-2022.8.8/app/dmdsk/func/trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/app/dmdsk/index.py` & `cikuu-2022.8.8/app/dmdsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/cikuu.egg-info/SOURCES.txt` & `cikuu-2022.8.8/cikuu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/__init__.py` & `cikuu-2022.8.8/dic/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/adjlist.py` & `cikuu-2022.8.8/dic/adjlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/advlist.py` & `cikuu-2022.8.8/dic/advlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/bnc_wordlist.py` & `cikuu-2022.8.8/dic/bnc_wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/confu_set.py` & `cikuu-2022.8.8/dic/confu_set.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/ecdic.py` & `cikuu-2022.8.8/dic/ecdic.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/errants.py` & `cikuu-2022.8.8/dic/errants.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/essays.py` & `cikuu-2022.8.8/dic/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/frame.py` & `cikuu-2022.8.8/dic/frame.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/lemma_lex.py` & `cikuu-2022.8.8/dic/lemma_lex.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/lemma_mf.py` & `cikuu-2022.8.8/dic/lemma_mf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/lemma_scale.py` & `cikuu-2022.8.8/dic/lemma_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/lex_lemma.py` & `cikuu-2022.8.8/dic/lex_lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/mwe_disconj.py` & `cikuu-2022.8.8/dic/mwe_disconj.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/mwe_pv.py` & `cikuu-2022.8.8/dic/mwe_pv.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/n_is_sb.py` & `cikuu-2022.8.8/dic/n_is_sb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/nounlist.py` & `cikuu-2022.8.8/dic/nounlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/nyt_wc.py` & `cikuu-2022.8.8/dic/nyt_wc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/orals.py` & `cikuu-2022.8.8/dic/orals.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/propbank.py` & `cikuu-2022.8.8/dic/propbank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/stoplist.py` & `cikuu-2022.8.8/dic/stoplist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/to_redislite.py` & `cikuu-2022.8.8/dic/to_redislite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/verbform.py` & `cikuu-2022.8.8/dic/verbform.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/verblist.py` & `cikuu-2022.8.8/dic/verblist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/verbtag.py` & `cikuu-2022.8.8/dic/verbtag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/vocab.py` & `cikuu-2022.8.8/dic/vocab.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_awl.py` & `cikuu-2022.8.8/dic/word_awl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_bits.py` & `cikuu-2022.8.8/dic/word_bits.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_grade.py` & `cikuu-2022.8.8/dic/word_grade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_gsl1.py` & `cikuu-2022.8.8/dic/word_gsl1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_gsl2.py` & `cikuu-2022.8.8/dic/word_gsl2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_idf.py` & `cikuu-2022.8.8/dic/word_idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_oov.py` & `cikuu-2022.8.8/dic/word_oov.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_pos.py` & `cikuu-2022.8.8/dic/word_pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/word_scale.py` & `cikuu-2022.8.8/dic/word_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordattr.py` & `cikuu-2022.8.8/dic/wordattr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordcnt.py` & `cikuu-2022.8.8/dic/wordcnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordlist.py` & `cikuu-2022.8.8/dic/wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordlist_ed1.py` & `cikuu-2022.8.8/dic/wordlist_ed1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordnet_verb.py` & `cikuu-2022.8.8/dic/wordnet_verb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/wordpos.py` & `cikuu-2022.8.8/dic/wordpos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/words.py` & `cikuu-2022.8.8/dic/words.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dic/yulk.py` & `cikuu-2022.8.8/dic/yulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import json, traceback,sys, time,  fileinput, os, fire,pathlib, platform, redis, spacy
 
 snthost = os.getenv('snthost', 'snt.jukuu.com:6206') #  snt => tx98
 if not hasattr(spacy, 'nlp'):
 	spacy.nlp		= spacy.load(os.getenv('spacy_model','en_core_web_sm')) # 3.4.1
 	spacy.from_json = lambda arr: spacy.tokens.Doc(spacy.nlp.vocab).from_json(arr) # added 2022.8.19
 
+def rcon():
+	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True)
+	return redis.r 
+
 def docs(name:str='gzjc'):
 	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True)
 	for k in redis.r.keys(f"snt-spacy:{name}:*"):
 		v = redis.r.get(k)  #redis.r.hget(k, 'spacy')
 		if not v: continue 
 		arr = json.loads(v.strip()) 
 		doc = spacy.from_json(arr)
```

### Comparing `cikuu-2022.8.7/dsk/__init__.py` & `cikuu-2022.8.8/dsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/__main__.py` & `cikuu-2022.8.8/dsk/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/common.py` & `cikuu-2022.8.8/dsk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dm.py` & `cikuu-2022.8.8/dsk/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dsk-hello.py` & `cikuu-2022.8.8/dsk/dsk-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dsk-to-dskmkf.py` & `cikuu-2022.8.8/dsk/dsk-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dsk2023.py` & `cikuu-2022.8.8/dsk/dsk2023.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dskapi.py` & `cikuu-2022.8.8/dsk/dskapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dskes.py` & `cikuu-2022.8.8/dsk/dskes.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dskmkf.py` & `cikuu-2022.8.8/dsk/dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dskmkf_fastapi.py` & `cikuu-2022.8.8/dsk/dskmkf_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/dsktrain.py` & `cikuu-2022.8.8/dsk/dsktrain.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/essaydm.py` & `cikuu-2022.8.8/dsk/essaydm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/gears-xdsk.py` & `cikuu-2022.8.8/dsk/gears-xdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/gecv1.py` & `cikuu-2022.8.8/dsk/gecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/index.py` & `cikuu-2022.8.8/dsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/innersim.py` & `cikuu-2022.8.8/dsk/innersim.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/json-to-dskmkf.py` & `cikuu-2022.8.8/dsk/json-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/kvrdsk.py` & `cikuu-2022.8.8/dsk/kvrdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/load.py` & `cikuu-2022.8.8/dsk/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/mkf.py` & `cikuu-2022.8.8/dsk/mkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/mqconsume.py` & `cikuu-2022.8.8/dsk/mqconsume.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/pingyu.py` & `cikuu-2022.8.8/dsk/pingyu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/score.py` & `cikuu-2022.8.8/dsk/score.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/sntsdims.py` & `cikuu-2022.8.8/dsk/sntsdims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/test.py` & `cikuu-2022.8.8/dsk/test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/tok-hello.py` & `cikuu-2022.8.8/dsk/tok-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/uvidsk.py` & `cikuu-2022.8.8/dsk/uvidsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/wps-gec.py` & `cikuu-2022.8.8/dsk/wps-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/wps-xgec.py` & `cikuu-2022.8.8/dsk/wps-xgec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/wps7000.py` & `cikuu-2022.8.8/dsk/wps7000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xessay.py` & `cikuu-2022.8.8/dsk/xessay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xgecv1-test.py` & `cikuu-2022.8.8/dsk/xgecv1-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xgecv1.py` & `cikuu-2022.8.8/dsk/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xmkf.py` & `cikuu-2022.8.8/dsk/xmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xsnt-gec.py` & `cikuu-2022.8.8/dsk/xsnt-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/dsk/xsnt-spacy.py` & `cikuu-2022.8.8/dsk/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/__init__.py` & `cikuu-2022.8.8/en/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/__main__.py` & `cikuu-2022.8.8/en/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/annotate.py` & `cikuu-2022.8.8/en/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/__init__.py` & `cikuu-2022.8.8/en/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/sntjson-innodb.py` & `cikuu-2022.8.8/en/arc/sntjson-innodb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/sntjson-naclite.py` & `cikuu-2022.8.8/en/arc/sntjson-naclite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/sntjson-naclite0.py` & `cikuu-2022.8.8/en/arc/sntjson-naclite0.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/sntjson-nacp-20230206.py` & `cikuu-2022.8.8/en/arc/sntjson-nacp-20230206.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/arc/sntjson-nacp-20230207.py` & `cikuu-2022.8.8/en/arc/sntjson-nacp-20230207.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-cl.py` & `cikuu-2022.8.8/en/c4-cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-fts.py` & `cikuu-2022.8.8/en/c4-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-gram-upload.py` & `cikuu-2022.8.8/en/c4-gram-upload.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-gram.py` & `cikuu-2022.8.8/en/c4-gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-grams.py` & `cikuu-2022.8.8/en/c4-grams.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-np.py` & `cikuu-2022.8.8/en/c4-np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4-trp.py` & `cikuu-2022.8.8/en/c4-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4cl.py` & `cikuu-2022.8.8/en/c4cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4gram-mysql.py` & `cikuu-2022.8.8/en/c4gram-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4gram-upsert.py` & `cikuu-2022.8.8/en/c4gram-upsert.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4gram.py` & `cikuu-2022.8.8/en/c4gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4gramcl.py` & `cikuu-2022.8.8/en/c4gramcl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4matcher.py` & `cikuu-2022.8.8/en/c4matcher.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4np.py` & `cikuu-2022.8.8/en/c4np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4postag.py` & `cikuu-2022.8.8/en/c4postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4skenp.py` & `cikuu-2022.8.8/en/c4skenp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4tree.py` & `cikuu-2022.8.8/en/c4tree.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4trp.py` & `cikuu-2022.8.8/en/c4trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/c4vp.py` & `cikuu-2022.8.8/en/c4vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/clause.py` & `cikuu-2022.8.8/en/clause.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/dims.py` & `cikuu-2022.8.8/en/dims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/docfts.py` & `cikuu-2022.8.8/en/docfts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/docjson.py` & `cikuu-2022.8.8/en/docjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/es-index.py` & `cikuu-2022.8.8/en/es-index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/esbulk.py` & `cikuu-2022.8.8/en/esbulk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/esfile.py` & `cikuu-2022.8.8/en/esfile.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/esjson.py` & `cikuu-2022.8.8/en/esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/exchunk.py` & `cikuu-2022.8.8/en/exchunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/exphrase.py` & `cikuu-2022.8.8/en/exphrase.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/extrp.py` & `cikuu-2022.8.8/en/extrp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/havc.py` & `cikuu-2022.8.8/en/havc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/kpsi.py` & `cikuu-2022.8.8/en/kpsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/lempostag.py` & `cikuu-2022.8.8/en/lempostag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/nacp-kvr.py` & `cikuu-2022.8.8/en/nacp-kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/nacp.py` & `cikuu-2022.8.8/en/nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/nlp-lit.py` & `cikuu-2022.8.8/en/nlp-lit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/nlp-lmdb.py` & `cikuu-2022.8.8/en/nlp-lmdb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/postag.py` & `cikuu-2022.8.8/en/postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/shav.py` & `cikuu-2022.8.8/en/shav.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/silite.py` & `cikuu-2022.8.8/en/silite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/snt-esjson.py` & `cikuu-2022.8.8/en/snt-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/snt-spacy.py` & `cikuu-2022.8.8/en/snt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-fts.py` & `cikuu-2022.8.8/en/sntjson-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-kpsnt.py` & `cikuu-2022.8.8/en/sntjson-kpsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-mysql.py` & `cikuu-2022.8.8/en/sntjson-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-nacp.py` & `cikuu-2022.8.8/en/sntjson-nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-parse-snt.py` & `cikuu-2022.8.8/en/sntjson-parse-snt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-si.py` & `cikuu-2022.8.8/en/sntjson-si.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-spacy.py` & `cikuu-2022.8.8/en/sntjson-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-topk.py` & `cikuu-2022.8.8/en/sntjson-topk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-tosnt.py` & `cikuu-2022.8.8/en/sntjson-tosnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-trpx.py` & `cikuu-2022.8.8/en/sntjson-trpx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sntjson-vp.py` & `cikuu-2022.8.8/en/sntjson-vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/spacybs-esjson.py` & `cikuu-2022.8.8/en/spacybs-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/spacybs.py` & `cikuu-2022.8.8/en/spacybs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/spider-esjson.py` & `cikuu-2022.8.8/en/spider-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/sqlsi.py` & `cikuu-2022.8.8/en/sqlsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/terms.py` & `cikuu-2022.8.8/en/terms.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/verbnet.py` & `cikuu-2022.8.8/en/verbnet.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/xsnt.py` & `cikuu-2022.8.8/en/xsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/en/zset-load.py` & `cikuu-2022.8.8/en/zset-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/gecdsk/__init__.py` & `cikuu-2022.8.8/gecdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/gecdsk/essays.py` & `cikuu-2022.8.8/gecdsk/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/gecdsk/paravs.py` & `cikuu-2022.8.8/gecdsk/paravs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/__init__.py` & `cikuu-2022.8.8/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/common.py` & `cikuu-2022.8.8/lit/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/es/__init__.py` & `cikuu-2022.8.8/lit/es/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/es/index.py` & `cikuu-2022.8.8/lit/es/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/essay.py` & `cikuu-2022.8.8/lit/essay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/fillmul.py` & `cikuu-2022.8.8/lit/fillmul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/hello-pages.py` & `cikuu-2022.8.8/lit/hello-pages.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/index.py` & `cikuu-2022.8.8/lit/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/mock-scoring.py` & `cikuu-2022.8.8/lit/mock-scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/penly/index.py` & `cikuu-2022.8.8/lit/penly/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/penly-resend.py` & `cikuu-2022.8.8/lit/penly-resend.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/redis-dump.py` & `cikuu-2022.8.8/lit/redis-dump.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/reorder.py` & `cikuu-2022.8.8/lit/reorder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/restore.py` & `cikuu-2022.8.8/lit/restore.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/scoring.py` & `cikuu-2022.8.8/lit/scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/single.py` & `cikuu-2022.8.8/lit/single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/sntspolish.py` & `cikuu-2022.8.8/lit/sntspolish.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/sntupgrade.py` & `cikuu-2022.8.8/lit/sntupgrade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/student-input.py` & `cikuu-2022.8.8/lit/student-input.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/teacher-admin.py` & `cikuu-2022.8.8/lit/teacher-admin.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/YULK.py` & `cikuu-2022.8.8/lit/yulk/YULK.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/common.py` & `cikuu-2022.8.8/lit/yulk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/bipos.py` & `cikuu-2022.8.8/lit/yulk/func/bipos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/cola.py` & `cikuu-2022.8.8/lit/yulk/func/cola.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/common.py` & `cikuu-2022.8.8/lit/yulk/func/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/corpuslist.py` & `cikuu-2022.8.8/lit/yulk/func/corpuslist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/es.py` & `cikuu-2022.8.8/lit/yulk/func/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/given-expect.py` & `cikuu-2022.8.8/lit/yulk/func/given-expect.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/gramx-single.py` & `cikuu-2022.8.8/lit/yulk/func/gramx-single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/lemma.py` & `cikuu-2022.8.8/lit/yulk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/lemvs.py` & `cikuu-2022.8.8/lit/yulk/func/lemvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/pos.py` & `cikuu-2022.8.8/lit/yulk/func/pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/posvs.py` & `cikuu-2022.8.8/lit/yulk/func/posvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/style-in-mul.py` & `cikuu-2022.8.8/lit/yulk/func/style-in-mul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/func/wordrank.py` & `cikuu-2022.8.8/lit/yulk/func/wordrank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/index.py` & `cikuu-2022.8.8/lit/yulk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/lit/yulk/lemma.py` & `cikuu-2022.8.8/lit/yulk/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/pipe/__init__.py` & `cikuu-2022.8.8/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/pipe/__main__.py` & `cikuu-2022.8.8/pipe/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/pipe/redisgec8180.py` & `cikuu-2022.8.8/pipe/redisgec8180.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/pipe/xgecv1.py` & `cikuu-2022.8.8/pipe/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/rabbitmq/__init__.py` & `cikuu-2022.8.8/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/redisr/__init__.py` & `cikuu-2022.8.8/redisr/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/redisr/glove-get.py` & `cikuu-2022.8.8/redisr/glove-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/redisr/glove.py` & `cikuu-2022.8.8/redisr/glove.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/redisr/sntvec-get.py` & `cikuu-2022.8.8/redisr/sntvec-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sbert/__main__.py` & `cikuu-2022.8.8/sbert/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sbert/hello.py` & `cikuu-2022.8.8/sbert/hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sbert/redis-sntvec.py` & `cikuu-2022.8.8/sbert/redis-sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sbert/sntvec-so.py` & `cikuu-2022.8.8/sbert/sntvec-so.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sbert/sntvec.py` & `cikuu-2022.8.8/sbert/sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/setup.py` & `cikuu-2022.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time: 2022-2-13
 #############################################
  
 from setuptools import setup, find_packages
  
 setup(
   name = "cikuu",
-  version = "2022.8.7",
+  version = "2022.8.8",
   keywords = ("pip"),
   description = "cikuu tools",
   long_description = "add replace into soinit",
   license = "MIT Licence",
  
   url = "http://www.cikuu.com",
   author = "cikuu",
```

### Comparing `cikuu-2022.8.7/so/__init__.py` & `cikuu-2022.8.8/so/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/__main__.py` & `cikuu-2022.8.8/so/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/batch-dis.py` & `cikuu-2022.8.8/so/batch-dis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/batch-sntspacy.py` & `cikuu-2022.8.8/so/batch-sntspacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dis-bnc.py` & `cikuu-2022.8.8/so/dis-bnc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dis-eev.py` & `cikuu-2022.8.8/so/dis-eev.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dis-essays.py` & `cikuu-2022.8.8/so/dis-essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dis-folder.py` & `cikuu-2022.8.8/so/dis-folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dis-tosnts.py` & `cikuu-2022.8.8/so/dis-tosnts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dsk.py` & `cikuu-2022.8.8/so/dsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dump-pos.py` & `cikuu-2022.8.8/so/dump-pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/dump-trp.py` & `cikuu-2022.8.8/so/dump-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/folder.py` & `cikuu-2022.8.8/so/folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/load.py` & `cikuu-2022.8.8/so/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/loades.py` & `cikuu-2022.8.8/so/loades.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/so/tok-idf.py` & `cikuu-2022.8.8/so/tok-idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/sqlite/__init__.py` & `cikuu-2022.8.8/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/__init__.py` & `cikuu-2022.8.8/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/__main__.py` & `cikuu-2022.8.8/util/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/annotate.py` & `cikuu-2022.8.8/util/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/bcp.py` & `cikuu-2022.8.8/util/bcp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/c4data.py` & `cikuu-2022.8.8/util/c4data.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/client-blpop.py` & `cikuu-2022.8.8/util/client-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/client-xwps.py` & `cikuu-2022.8.8/util/client-xwps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/clientx.py` & `cikuu-2022.8.8/util/clientx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/dsk-util.py` & `cikuu-2022.8.8/util/dsk-util.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/kvr.py` & `cikuu-2022.8.8/util/kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/mq.py` & `cikuu-2022.8.8/util/mq.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/nldp.py` & `cikuu-2022.8.8/util/nldp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/pubsub-sync.py` & `cikuu-2022.8.8/util/pubsub-sync.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/pubsub2api.py` & `cikuu-2022.8.8/util/pubsub2api.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/spider.py` & `cikuu-2022.8.8/util/spider.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/sqlitedict-load.py` & `cikuu-2022.8.8/util/sqlitedict-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/wps-blpop.py` & `cikuu-2022.8.8/util/wps-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/wps.py` & `cikuu-2022.8.8/util/wps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/xsnt-spacy.py` & `cikuu-2022.8.8/util/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/xstream.py` & `cikuu-2022.8.8/util/xstream.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/xtest-params.py` & `cikuu-2022.8.8/util/xtest-params.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/util/xtest.py` & `cikuu-2022.8.8/util/xtest.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uviapp/__init__.py` & `cikuu-2022.8.8/uviapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/Jinja2-test.py` & `cikuu-2022.8.8/uvirun/Jinja2-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/__init__.py` & `cikuu-2022.8.8/uvirun/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/__main__.py` & `cikuu-2022.8.8/uvirun/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/c4es.py` & `cikuu-2022.8.8/uvirun/c4es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/c4gramsi.py` & `cikuu-2022.8.8/uvirun/c4gramsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/cos_fastapi.py` & `cikuu-2022.8.8/uvirun/cos_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/demo_fastapi.py` & `cikuu-2022.8.8/uvirun/demo_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/dsk_fastapi.py` & `cikuu-2022.8.8/uvirun/dsk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/echart_fastapi.py` & `cikuu-2022.8.8/uvirun/echart_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/elastic_fastapi.py` & `cikuu-2022.8.8/uvirun/elastic_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/__init__.py` & `cikuu-2022.8.8/uvirun/errant/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/alignment.py` & `cikuu-2022.8.8/uvirun/errant/alignment.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/annotator.py` & `cikuu-2022.8.8/uvirun/errant/annotator.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/commands/compare_m2.py` & `cikuu-2022.8.8/uvirun/errant/commands/compare_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/commands/m2_to_m2.py` & `cikuu-2022.8.8/uvirun/errant/commands/m2_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/commands/parallel_to_m2.py` & `cikuu-2022.8.8/uvirun/errant/commands/parallel_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/edit.py` & `cikuu-2022.8.8/uvirun/errant/edit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/en/classifier.py` & `cikuu-2022.8.8/uvirun/errant/en/classifier.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/en/lancaster.py` & `cikuu-2022.8.8/uvirun/errant/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant/en/merger.py` & `cikuu-2022.8.8/uvirun/errant/en/merger.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/errant_fastapi.py` & `cikuu-2022.8.8/uvirun/errant_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/es1_fastapi.py` & `cikuu-2022.8.8/uvirun/es1_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/es_fastapi.py` & `cikuu-2022.8.8/uvirun/es_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/essay_fastapi.py` & `cikuu-2022.8.8/uvirun/essay_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/exchunk_fastapi.py` & `cikuu-2022.8.8/uvirun/exchunk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/feishu_fastapi.py` & `cikuu-2022.8.8/uvirun/feishu_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/flair_fastapi.py` & `cikuu-2022.8.8/uvirun/flair_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/ftp.py` & `cikuu-2022.8.8/uvirun/ftp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/fusion_fastapi.py` & `cikuu-2022.8.8/uvirun/fusion_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/gec_fastapi.py` & `cikuu-2022.8.8/uvirun/gec_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/gec_fastapi_33000.py` & `cikuu-2022.8.8/uvirun/gec_fastapi_33000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/gensim_fastapi.py` & `cikuu-2022.8.8/uvirun/gensim_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/gramx_fastapi.py` & `cikuu-2022.8.8/uvirun/gramx_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/hnswlib_fastapi.py` & `cikuu-2022.8.8/uvirun/hnswlib_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/kenlm_fastapi.py` & `cikuu-2022.8.8/uvirun/kenlm_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/kpsi_fastapi.py` & `cikuu-2022.8.8/uvirun/kpsi_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/kvr_dskdm.py` & `cikuu-2022.8.8/uvirun/kvr_dskdm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/kvr_dskdm1230.py` & `cikuu-2022.8.8/uvirun/kvr_dskdm1230.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/nldp_fastapi.py` & `cikuu-2022.8.8/uvirun/nldp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/nltk_fastapi.py` & `cikuu-2022.8.8/uvirun/nltk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/nsp_fastapi.py` & `cikuu-2022.8.8/uvirun/nsp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/penlykvr.py` & `cikuu-2022.8.8/uvirun/penlykvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/sbert_fastapi.py` & `cikuu-2022.8.8/uvirun/sbert_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/spacy_fastapi.py` & `cikuu-2022.8.8/uvirun/spacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/textacy_fastapi.py` & `cikuu-2022.8.8/uvirun/textacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/trans_fastapi.py` & `cikuu-2022.8.8/uvirun/trans_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/unmasker_fastapi.py` & `cikuu-2022.8.8/uvirun/unmasker_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/util_fastapi.py` & `cikuu-2022.8.8/uvirun/util_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/uviredis.py` & `cikuu-2022.8.8/uvirun/uviredis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.7/uvirun/yulk-nac.py` & `cikuu-2022.8.8/uvirun/yulk-nac.py`

 * *Files identical despite different names*

