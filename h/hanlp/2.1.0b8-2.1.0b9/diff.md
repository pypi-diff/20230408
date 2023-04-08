# Comparing `tmp/hanlp-2.1.0b8.tar.gz` & `tmp/hanlp-2.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hanlp-2.1.0b8.tar", last modified: Wed Feb  2 00:16:39 2022, max compression
+gzip compressed data, was "hanlp-2.1.0b9.tar", last modified: Wed Feb  2 01:14:51 2022, max compression
```

## Comparing `hanlp-2.1.0b8.tar` & `hanlp-2.1.0b9.tar`

### file list

```diff
@@ -1,407 +1,407 @@
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.415731 hanlp-2.1.0b8/
--rw-r--r--   0 runner    (1000) docker     (121)    13518 2022-02-02 00:16:39.415731 hanlp-2.1.0b8/PKG-INFO
--rw-r--r--   0 runner    (1000) docker     (121)    10997 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/README.md
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.379730 hanlp-2.1.0b8/hanlp/
--rw-r--r--   0 runner    (1000) docker     (121)     2073 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.379730 hanlp-2.1.0b8/hanlp/callbacks/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/callbacks/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2613 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/callbacks/fine_csv_logger.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/common/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1004 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/component.py
--rw-r--r--   0 runner    (1000) docker     (121)    34141 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/dataset.py
--rw-r--r--   0 runner    (1000) docker     (121)    24437 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/keras_component.py
--rw-r--r--   0 runner    (1000) docker     (121)     2454 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/structure.py
--rw-r--r--   0 runner    (1000) docker     (121)    25984 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/torch_component.py
--rw-r--r--   0 runner    (1000) docker     (121)    15235 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/transform.py
--rw-r--r--   0 runner    (1000) docker     (121)    11225 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/transform_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    16012 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/vocab.py
--rw-r--r--   0 runner    (1000) docker     (121)     8615 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/common/vocab_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/
--rw-r--r--   0 runner    (1000) docker     (121)       95 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/amr/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/
--rw-r--r--   0 runner    (1000) docker     (121)      995 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/IO.py
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     9017 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/dataset.py
--rw-r--r--   0 runner    (1000) docker     (121)    13590 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/linearization.py
--rw-r--r--   0 runner    (1000) docker     (121)     1916 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/penman.py
--rw-r--r--   0 runner    (1000) docker     (121)    22677 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/postprocessing.py
--rw-r--r--   0 runner    (1000) docker     (121)    26401 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/tokenization_bart.py
--rw-r--r--   0 runner    (1000) docker     (121)    26307 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/tokenization_t5.py
--rw-r--r--   0 runner    (1000) docker     (121)      592 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/evaluation.py
--rw-r--r--   0 runner    (1000) docker     (121)     4368 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/optim.py
--rw-r--r--   0 runner    (1000) docker     (121)    23026 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/amr/seq2seq/seq2seq_amr_parser.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/classifiers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/classifiers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    17241 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/classifiers/transformer_classifier.py
--rw-r--r--   0 runner    (1000) docker     (121)     9668 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/classifiers/transformer_classifier_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/distillation/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/distillation/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2084 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/distillation/distillable_component.py
--rw-r--r--   0 runner    (1000) docker     (121)    15061 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/distillation/losses.py
--rw-r--r--   0 runner    (1000) docker     (121)     3585 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/distillation/schedulers.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/eos/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/eos/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    12206 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/eos/ngram.py
--rw-r--r--   0 runner    (1000) docker     (121)      946 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/lambda_wrapper.py
--rw-r--r--   0 runner    (1000) docker     (121)     1588 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/lemmatizer.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/lm/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/lm/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     4729 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/lm/mlm.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.383730 hanlp-2.1.0b8/hanlp/components/mtl/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    38042 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/multi_task_learning.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/mtl/tasks/
--rw-r--r--   0 runner    (1000) docker     (121)    11771 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     8216 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/amr.py
--rw-r--r--   0 runner    (1000) docker     (121)     7783 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/constituency.py
--rw-r--r--   0 runner    (1000) docker     (121)     8240 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/dep.py
--rw-r--r--   0 runner    (1000) docker     (121)     5219 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/dep_2nd.py
--rw-r--r--   0 runner    (1000) docker     (121)     6308 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/lem.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5752 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/biaffine_ner.py
--rw-r--r--   0 runner    (1000) docker     (121)     8900 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/tag_ner.py
--rw-r--r--   0 runner    (1000) docker     (121)     7953 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/pos.py
--rw-r--r--   0 runner    (1000) docker     (121)     8727 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/sdp.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5880 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/bio_srl.py
--rw-r--r--   0 runner    (1000) docker     (121)     6579 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/rank_srl.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5250 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/reg_tok.py
--rw-r--r--   0 runner    (1000) docker     (121)    10190 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/tag_tok.py
--rw-r--r--   0 runner    (1000) docker     (121)     7542 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/mtl/tasks/ud.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/ner/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    17717 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/biaffine_ner.py
--rw-r--r--   0 runner    (1000) docker     (121)     6168 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/biaffine_ner_model.py
--rw-r--r--   0 runner    (1000) docker     (121)     4028 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/ner_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     2957 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/rnn_ner.py
--rw-r--r--   0 runner    (1000) docker     (121)    11404 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/ner/transformer_ner.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/parsers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    29627 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/alg.py
--rw-r--r--   0 runner    (1000) docker     (121)    10513 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/alg_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.387730 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3526 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine.py
--rw-r--r--   0 runner    (1000) docker     (121)    11513 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_2nd_dep.py
--rw-r--r--   0 runner    (1000) docker     (121)    26465 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_dep.py
--rw-r--r--   0 runner    (1000) docker     (121)    10518 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_model.py
--rw-r--r--   0 runner    (1000) docker     (121)     8478 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_sdp.py
--rw-r--r--   0 runner    (1000) docker     (121)     2784 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/mlp.py
--rw-r--r--   0 runner    (1000) docker     (121)    10453 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/structual_attention.py
--rw-r--r--   0 runner    (1000) docker     (121)     9708 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine/variationalbilstm.py
--rw-r--r--   0 runner    (1000) docker     (121)    38285 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_parser_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    10513 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/alg.py
--rw-r--r--   0 runner    (1000) docker     (121)     6893 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/layers.py
--rw-r--r--   0 runner    (1000) docker     (121)    11580 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/model.py
--rw-r--r--   0 runner    (1000) docker     (121)    10923 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/chu_liu_edmonds.py
--rw-r--r--   0 runner    (1000) docker     (121)     2534 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/conll.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/parsers/constituency/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/constituency/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     9086 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/constituency/crf_constituency_model.py
--rw-r--r--   0 runner    (1000) docker     (121)    13350 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/constituency/crf_constituency_parser.py
--rw-r--r--   0 runner    (1000) docker     (121)    16923 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/constituency/treecrf.py
--rw-r--r--   0 runner    (1000) docker     (121)    10912 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/parse_alg.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/parsers/ud/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     4317 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/lemma_edit.py
--rw-r--r--   0 runner    (1000) docker     (121)     5766 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/tag_decoder.py
--rw-r--r--   0 runner    (1000) docker     (121)     5198 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/ud_model.py
--rw-r--r--   0 runner    (1000) docker     (121)    15674 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/ud_parser.py
--rw-r--r--   0 runner    (1000) docker     (121)    15298 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/udify_util.py
--rw-r--r--   0 runner    (1000) docker     (121)      955 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/parsers/ud/util.py
--rw-r--r--   0 runner    (1000) docker     (121)     6359 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/pipeline.py
--rw-r--r--   0 runner    (1000) docker     (121)     3573 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/rnn_language_model_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/srl/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/srl/span_bio/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_bio/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2306 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_bio/baffine_tagging.py
--rw-r--r--   0 runner    (1000) docker     (121)    16094 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_bio/span_bio.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/srl/span_rank/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    12805 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/highway_variational_lstm.py
--rw-r--r--   0 runner    (1000) docker     (121)    10363 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/inference_utils.py
--rw-r--r--   0 runner    (1000) docker     (121)    16572 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/layer.py
--rw-r--r--   0 runner    (1000) docker     (121)    18091 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/span_rank.py
--rw-r--r--   0 runner    (1000) docker     (121)    27835 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/span_ranking_srl_model.py
--rw-r--r--   0 runner    (1000) docker     (121)    11077 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/srl_eval_utils.py
--rw-r--r--   0 runner    (1000) docker     (121)      387 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/srl/span_rank/util.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/sts/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/sts/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    11294 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/sts/transformer_sts.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/taggers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     4928 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/cnn_tagger_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/taggers/ngram_conv/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/ngram_conv/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     8043 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/ngram_conv/ngram_conv_tagger.py
--rw-r--r--   0 runner    (1000) docker     (121)      301 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/pos_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.391730 hanlp-2.1.0b8/hanlp/components/taggers/rnn/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/rnn/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3411 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/rnn/rnntaggingmodel.py
--rw-r--r--   0 runner    (1000) docker     (121)     8415 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/rnn_tagger.py
--rw-r--r--   0 runner    (1000) docker     (121)     4190 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/rnn_tagger_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     9824 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/tagger.py
--rw-r--r--   0 runner    (1000) docker     (121)     1617 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/tagger_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/components/taggers/transformers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/transformers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      507 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/transformers/metrics_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    10807 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_tagger.py
--rw-r--r--   0 runner    (1000) docker     (121)     4176 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_tagger_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     6373 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_transform_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)      710 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/taggers/util.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/components/tokenizers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/tokenizers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     4333 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/tokenizers/multi_criteria_cws_transformer.py
--rw-r--r--   0 runner    (1000) docker     (121)     2041 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/tokenizers/tok.py
--rw-r--r--   0 runner    (1000) docker     (121)     5007 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/tokenizers/tok_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    13014 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/components/tokenizers/transformer.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/classification/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/classification/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      340 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/classification/sentiment.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/coref/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/coref/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/coref/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/coref/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3517 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/coref/loaders/conll12coref.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/eos/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/eos/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3939 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/eos/eos.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/eos/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/eos/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1233 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/eos/loaders/nn_eos.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/lm/
--rw-r--r--   0 runner    (1000) docker     (121)      452 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/lm/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/lm/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/lm/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5025 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/lm/loaders/lm_dataset.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/lu/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/lu/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      835 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/lu/glue.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/ner/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      565 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/conll03.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/ner/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5821 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/loaders/json_ner.py
--rw-r--r--   0 runner    (1000) docker     (121)     3588 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/loaders/tsv.py
--rw-r--r--   0 runner    (1000) docker     (121)     2270 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/msra.py
--rw-r--r--   0 runner    (1000) docker     (121)      593 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/resume.py
--rw-r--r--   0 runner    (1000) docker     (121)      584 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/ner/weibo.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.395731 hanlp-2.1.0b8/hanlp/datasets/parsing/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    16531 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/amr.py
--rw-r--r--   0 runner    (1000) docker     (121)      554 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ctb5.py
--rw-r--r--   0 runner    (1000) docker     (121)      421 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ctb7.py
--rw-r--r--   0 runner    (1000) docker     (121)     2001 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ctb8.py
--rw-r--r--   0 runner    (1000) docker     (121)     2422 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ctb9.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    11080 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/_ctb_utils.py
--rw-r--r--   0 runner    (1000) docker     (121)     3931 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/conll_dataset.py
--rw-r--r--   0 runner    (1000) docker     (121)     7321 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/constituency_dataset.py
--rw-r--r--   0 runner    (1000) docker     (121)     1791 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ptb.py
--rw-r--r--   0 runner    (1000) docker     (121)     2165 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/semeval15.py
--rw-r--r--   0 runner    (1000) docker     (121)     2969 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/semeval16.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/
--rw-r--r--   0 runner    (1000) docker     (121)     1130 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    26967 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud23.py
--rw-r--r--   0 runner    (1000) docker     (121)      466 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud23m.py
--rw-r--r--   0 runner    (1000) docker     (121)    49930 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud27.py
--rw-r--r--   0 runner    (1000) docker     (121)      719 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud27m.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/pos/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/pos/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      356 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/pos/ctb5.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/qa/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/qa/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     6170 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/qa/hotpotqa.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/srl/
--rw-r--r--   0 runner    (1000) docker     (121)       67 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/srl/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     8505 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/loaders/conll2012.py
--rw-r--r--   0 runner    (1000) docker     (121)    27116 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/loaders/ontonotes_loader.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/
--rw-r--r--   0 runner    (1000) docker     (121)      220 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    25112 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/_utils.py
--rw-r--r--   0 runner    (1000) docker     (121)     6212 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/chinese.py
--rw-r--r--   0 runner    (1000) docker     (121)     5237 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/english.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/sts/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/sts/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1412 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/sts/stsb.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/tokenization/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      330 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/ctb6.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2065 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/chunking_dataset.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/multi_criteria_cws/
--rw-r--r--   0 runner    (1000) docker     (121)     1027 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/multi_criteria_cws/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3860 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/multi_criteria_cws/mcws_dataset.py
--rw-r--r--   0 runner    (1000) docker     (121)     5133 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/txt.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/
--rw-r--r--   0 runner    (1000) docker     (121)      862 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      806 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/as_.py
--rw-r--r--   0 runner    (1000) docker     (121)      839 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/cityu.py
--rw-r--r--   0 runner    (1000) docker     (121)      813 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/msr.py
--rw-r--r--   0 runner    (1000) docker     (121)      813 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/pku.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/layers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     5711 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/cnn_encoder.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.399731 hanlp-2.1.0b8/hanlp/layers/crf/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/crf/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    15514 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/crf/crf.py
--rw-r--r--   0 runner    (1000) docker     (121)     7242 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/crf/crf_layer_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    19677 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/crf/crf_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     5436 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/dropout.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/layers/embeddings/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     7434 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/char_cnn.py
--rw-r--r--   0 runner    (1000) docker     (121)     3603 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/char_cnn_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     3920 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/char_rnn.py
--rw-r--r--   0 runner    (1000) docker     (121)     2837 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/char_rnn_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     2064 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/concat_embedding.py
--rw-r--r--   0 runner    (1000) docker     (121)     8591 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_string_embedding.py
--rw-r--r--   0 runner    (1000) docker     (121)     4988 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_string_embedding_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     9795 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_word_embedding.py
--rw-r--r--   0 runner    (1000) docker     (121)     3986 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/embedding.py
--rw-r--r--   0 runner    (1000) docker     (121)     5697 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/fast_text.py
--rw-r--r--   0 runner    (1000) docker     (121)     3925 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/fast_text_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     4037 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/util.py
--rw-r--r--   0 runner    (1000) docker     (121)     4214 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/util_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    15031 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/word2vec.py
--rw-r--r--   0 runner    (1000) docker     (121)     8343 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/embeddings/word2vec_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)      571 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/feed_forward.py
--rw-r--r--   0 runner    (1000) docker     (121)     4141 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/feedforward.py
--rw-r--r--   0 runner    (1000) docker     (121)     7080 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/scalar_mix.py
--rw-r--r--   0 runner    (1000) docker     (121)     2549 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/time_distributed.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/layers/transformers/
--rw-r--r--   0 runner    (1000) docker     (121)      623 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     6056 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/encoder.py
--rw-r--r--   0 runner    (1000) docker     (121)     1214 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/loader_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     3398 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/pt_imports.py
--rw-r--r--   0 runner    (1000) docker     (121)    11300 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/relative_transformer.py
--rw-r--r--   0 runner    (1000) docker     (121)     1306 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/resource.py
--rw-r--r--   0 runner    (1000) docker     (121)      331 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/tf_imports.py
--rw-r--r--   0 runner    (1000) docker     (121)    17023 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/utils.py
--rw-r--r--   0 runner    (1000) docker     (121)     7861 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/transformers/utils_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     7778 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/layers/weight_normalization.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/losses/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/losses/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2395 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/losses/sparse_categorical_crossentropy.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/metrics/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     9609 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/accuracy.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/metrics/amr/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/amr/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     3589 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/amr/smatch_eval.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.403731 hanlp-2.1.0b8/hanlp/metrics/chunking/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1223 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/binary_chunking_f1.py
--rw-r--r--   0 runner    (1000) docker     (121)     1578 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/bmes_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     5354 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/chunking_f1.py
--rw-r--r--   0 runner    (1000) docker     (121)     2490 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/chunking_f1_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    11543 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/conlleval.py
--rw-r--r--   0 runner    (1000) docker     (121)      984 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/iobes_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    14144 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/chunking/sequence_labeling.py
--rw-r--r--   0 runner    (1000) docker     (121)     1561 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/f1.py
--rw-r--r--   0 runner    (1000) docker     (121)      834 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/metric.py
--rw-r--r--   0 runner    (1000) docker     (121)     1389 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/mtl.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/metrics/parsing/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     2433 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/attachmentscore.py
--rw-r--r--   0 runner    (1000) docker     (121)     2417 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/conllx_eval.py
--rw-r--r--   0 runner    (1000) docker     (121)     2727 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_f1.py
--rw-r--r--   0 runner    (1000) docker     (121)     2854 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_f1_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     1457 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_score.py
--rw-r--r--   0 runner    (1000) docker     (121)     5188 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/semdep_eval.py
--rw-r--r--   0 runner    (1000) docker     (121)     3222 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/parsing/span.py
--rw-r--r--   0 runner    (1000) docker     (121)     2885 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/spearman_correlation.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/metrics/srl/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/srl/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1701 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/metrics/srl/srlconll.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/optimizers/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/optimizers/adamw/
--rw-r--r--   0 runner    (1000) docker     (121)     2484 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/optimizers/adamw/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     8555 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/optimizers/adamw/optimization.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/pretrained/
--rw-r--r--   0 runner    (1000) docker     (121)      636 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1333 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/amr.py
--rw-r--r--   0 runner    (1000) docker     (121)      308 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/classifiers.py
--rw-r--r--   0 runner    (1000) docker     (121)      746 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/constituency.py
--rw-r--r--   0 runner    (1000) docker     (121)      524 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/dep.py
--rw-r--r--   0 runner    (1000) docker     (121)      307 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/eos.py
--rw-r--r--   0 runner    (1000) docker     (121)     1026 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/fasttext.py
--rw-r--r--   0 runner    (1000) docker     (121)      981 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/glove.py
--rw-r--r--   0 runner    (1000) docker     (121)     2469 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/mtl.py
--rw-r--r--   0 runner    (1000) docker     (121)      801 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/ner.py
--rw-r--r--   0 runner    (1000) docker     (121)     1706 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/pos.py
--rw-r--r--   0 runner    (1000) docker     (121)      658 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/rnnlm.py
--rw-r--r--   0 runner    (1000) docker     (121)      914 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/sdp.py
--rw-r--r--   0 runner    (1000) docker     (121)      286 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/srl.py
--rw-r--r--   0 runner    (1000) docker     (121)      299 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/sts.py
--rw-r--r--   0 runner    (1000) docker     (121)     1513 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/tok.py
--rw-r--r--   0 runner    (1000) docker     (121)     2942 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/pretrained/word2vec.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.407731 hanlp-2.1.0b8/hanlp/transform/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    39429 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/conll_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     1461 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/glue_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     3961 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/table_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     4510 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/tacred_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     3605 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/text_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)    35532 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/transformer_tokenizer.py
--rw-r--r--   0 runner    (1000) docker     (121)     5960 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/tsv_tf.py
--rw-r--r--   0 runner    (1000) docker     (121)     8326 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/transform/txt_tf.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.411731 hanlp-2.1.0b8/hanlp/utils/
--rw-r--r--   0 runner    (1000) docker     (121)      639 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     9399 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/component_util.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.411731 hanlp-2.1.0b8/hanlp/utils/file_read_backwards/
--rwxr-xr-x   0 runner    (1000) docker     (121)      182 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/file_read_backwards/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     6248 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/file_read_backwards/buffer_work_space.py
--rw-r--r--   0 runner    (1000) docker     (121)     4148 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/file_read_backwards/file_read_backwards.py
--rw-r--r--   0 runner    (1000) docker     (121)      393 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/init_util.py
--rw-r--r--   0 runner    (1000) docker     (121)    25083 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/io_util.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.411731 hanlp-2.1.0b8/hanlp/utils/lang/
--rw-r--r--   0 runner    (1000) docker     (121)      138 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.411731 hanlp-2.1.0b8/hanlp/utils/lang/en/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/en/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)    13792 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/en/english_tokenizer.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.411731 hanlp-2.1.0b8/hanlp/utils/lang/ja/
--rw-r--r--   0 runner    (1000) docker     (121)       65 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/ja/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     4281 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/ja/bert_tok.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.415731 hanlp-2.1.0b8/hanlp/utils/lang/zh/
--rw-r--r--   0 runner    (1000) docker     (121)       64 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/zh/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     1350 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/zh/char_table.py
--rw-r--r--   0 runner    (1000) docker     (121)     2318 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/lang/zh/localization.py
--rw-r--r--   0 runner    (1000) docker     (121)     5512 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/log_util.py
--rw-r--r--   0 runner    (1000) docker     (121)     1363 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/rules.py
--rw-r--r--   0 runner    (1000) docker     (121)    26998 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/span_util.py
--rw-r--r--   0 runner    (1000) docker     (121)     3257 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/string_util.py
--rw-r--r--   0 runner    (1000) docker     (121)     5648 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/tf_util.py
--rw-r--r--   0 runner    (1000) docker     (121)     6719 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/time_util.py
--rw-r--r--   0 runner    (1000) docker     (121)     9299 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/utils/torch_util.py
--rw-r--r--   0 runner    (1000) docker     (121)      158 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/hanlp/version.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-02 00:16:39.379730 hanlp-2.1.0b8/hanlp.egg-info/
--rw-r--r--   0 runner    (1000) docker     (121)    13518 2022-02-02 00:16:39.000000 hanlp-2.1.0b8/hanlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker     (121)    12222 2022-02-02 00:16:39.000000 hanlp-2.1.0b8/hanlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker     (121)        1 2022-02-02 00:16:39.000000 hanlp-2.1.0b8/hanlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker     (121)      211 2022-02-02 00:16:39.000000 hanlp-2.1.0b8/hanlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker     (121)        6 2022-02-02 00:16:39.000000 hanlp-2.1.0b8/hanlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker     (121)       38 2022-02-02 00:16:39.415731 hanlp-2.1.0b8/setup.cfg
--rw-r--r--   0 runner    (1000) docker     (121)     2045 2022-02-02 00:16:32.000000 hanlp-2.1.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/
+-rw-r--r--   0 runner    (1001) docker     (121)    13518 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10997 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/
+-rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/callbacks/fine_csv_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/common/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/component.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34141 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24437 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/keras_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25984 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/torch_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15235 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11225 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/transform_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16012 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/vocab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8615 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/common/vocab_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/components/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/components/amr/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/IO.py
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9017 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13590 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/penman.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22677 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26401 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/tokenization_bart.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26307 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/tokenization_t5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/optim.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23026 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/amr/seq2seq/seq2seq_amr_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp/components/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17241 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/classifiers/transformer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9668 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/classifiers/transformer_classifier_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/distillation/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/distillation/distillable_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15061 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/distillation/losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/distillation/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/eos/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12206 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/eos/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/lemmatizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/lm/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/lm/mlm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/mtl/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38042 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/multi_task_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/mtl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)    11771 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8216 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/amr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/constituency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8240 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/dep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/dep_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6308 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/lem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5752 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/biaffine_ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8900 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/tag_ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/pos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8727 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/sdp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5880 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/bio_srl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/rank_srl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/reg_tok.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10190 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/tag_tok.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7542 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/mtl/tasks/ud.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/ner/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17717 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/biaffine_ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/biaffine_ner_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/ner_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/rnn_ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11404 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/ner/transformer_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.980721 hanlp-2.1.0b9/hanlp/components/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29627 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/alg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10513 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/alg_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11513 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_2nd_dep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26465 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_dep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10518 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_sdp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10453 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/structual_attention.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9708 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine/variationalbilstm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29559 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_parser_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10513 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/alg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7725 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10923 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/chu_liu_edmonds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/conll.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/parsers/constituency/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/constituency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9086 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/constituency/crf_constituency_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13350 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/constituency/crf_constituency_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16923 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/constituency/treecrf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10912 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/parse_alg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/parsers/ud/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/lemma_edit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5766 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/tag_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/ud_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15674 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/ud_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15298 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/udify_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/parsers/ud/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/rnn_language_model_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/srl/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/srl/span_bio/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_bio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_bio/baffine_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16094 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_bio/span_bio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/srl/span_rank/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12805 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/highway_variational_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10363 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/inference_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16572 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18091 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/span_rank.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27835 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/span_ranking_srl_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11077 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/srl_eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/srl/span_rank/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/sts/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11294 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/sts/transformer_sts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/taggers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/cnn_tagger_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/taggers/ngram_conv/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/ngram_conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8043 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/ngram_conv/ngram_conv_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/pos_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.984721 hanlp-2.1.0b9/hanlp/components/taggers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/rnn/rnntaggingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8415 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/rnn_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/rnn_tagger_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9824 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/tagger_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/components/taggers/transformers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/transformers/metrics_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10807 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4176 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_tagger_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6373 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_transform_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/taggers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/components/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/tokenizers/multi_criteria_cws_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/tokenizers/tok.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5007 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/tokenizers/tok_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13014 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/components/tokenizers/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/classification/sentiment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/coref/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/coref/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/coref/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/coref/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3517 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/coref/loaders/conll12coref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/eos/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/eos/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/eos/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/eos/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/eos/loaders/nn_eos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/lm/
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/lm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/lm/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/lm/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/lm/loaders/lm_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/lu/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/lu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/lu/glue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/ner/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/conll03.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/ner/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/loaders/json_ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/loaders/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/msra.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/resume.py
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/ner/weibo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16531 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/amr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ctb5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ctb7.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ctb8.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ctb9.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/_ctb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/conll_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7321 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/constituency_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ptb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/semeval15.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/semeval16.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26967 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud23.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud23m.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49930 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud27.py
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud27m.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.988721 hanlp-2.1.0b9/hanlp/datasets/pos/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/pos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/pos/ctb5.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/qa/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6170 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/qa/hotpotqa.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/srl/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/srl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8505 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/loaders/conll2012.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27116 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/loaders/ontonotes_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25112 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6212 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/chinese.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5237 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/english.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/sts/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/sts/stsb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/ctb6.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/chunking_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/multi_criteria_cws/
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/multi_criteria_cws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3860 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/multi_criteria_cws/mcws_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/as_.py
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/cityu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/msr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/pku.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/cnn_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.992722 hanlp-2.1.0b9/hanlp/layers/crf/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15514 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/crf/crf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7242 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/crf/crf_layer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19677 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/crf/crf_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7434 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/char_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/char_cnn_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/char_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/char_rnn_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/concat_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8591 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_string_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_string_embedding_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9795 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_word_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/fast_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/fast_text_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4037 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4214 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/util_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15031 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/word2vec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8343 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/embeddings/word2vec_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/scalar_mix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/layers/transformers/
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6056 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/loader_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/pt_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11300 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/relative_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/tf_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17023 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7861 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/transformers/utils_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7778 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/layers/weight_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/losses/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/losses/sparse_categorical_crossentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9609 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/accuracy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/metrics/amr/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/amr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/amr/smatch_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/metrics/chunking/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/binary_chunking_f1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/bmes_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/chunking_f1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/chunking_f1_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11543 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/conlleval.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/iobes_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14144 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/chunking/sequence_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/f1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/mtl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/metrics/parsing/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/attachmentscore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/conllx_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_f1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_f1_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_score.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/semdep_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/parsing/span.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/spearman_correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/metrics/srl/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/srl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/metrics/srl/srlconll.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.996722 hanlp-2.1.0b9/hanlp/optimizers/adamw/
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/optimizers/adamw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8555 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/optimizers/adamw/optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/amr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/constituency.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/dep.py
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/eos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/glove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/pos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/rnnlm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/sdp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/srl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/sts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/tok.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/pretrained/word2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/transform/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39429 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/conll_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/glue_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/table_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/tacred_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3605 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/text_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35532 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/transformer_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/tsv_tf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8326 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/transform/txt_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9399 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/component_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/file_read_backwards/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      182 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/file_read_backwards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6248 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/file_read_backwards/buffer_work_space.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/file_read_backwards/file_read_backwards.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/init_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25083 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/io_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/lang/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/lang/en/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/en/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13792 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/en/english_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/lang/ja/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/ja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/ja/bert_tok.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/hanlp/utils/lang/zh/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/zh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/zh/char_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/lang/zh/localization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5512 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/log_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26998 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/span_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6719 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9299 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/utils/torch_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/hanlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 01:14:50.976720 hanlp-2.1.0b9/hanlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13518 2022-02-02 01:14:50.000000 hanlp-2.1.0b9/hanlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12222 2022-02-02 01:14:50.000000 hanlp-2.1.0b9/hanlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 01:14:50.000000 hanlp-2.1.0b9/hanlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-02-02 01:14:50.000000 hanlp-2.1.0b9/hanlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-02 01:14:50.000000 hanlp-2.1.0b9/hanlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-02 01:14:51.000723 hanlp-2.1.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-02-02 01:14:43.000000 hanlp-2.1.0b9/setup.py
```

### Comparing `hanlp-2.1.0b8/PKG-INFO` & `hanlp-2.1.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hanlp
-Version: 2.1.0b8
+Version: 2.1.0b9
 Summary: HanLP: Han Language Processing
 Home-page: https://github.com/hankcs/HanLP
 Author: hankcs
 Author-email: hankcshe@gmail.com
 License: Apache License 2.0
 Description: <div align="center"><img src="https://file.hankcs.com/img/hanlp-github-banner.png" height="100px"/></div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hanlp Version: 2.1.0b8 Summary: HanLP: Han Language
+Metadata-Version: 2.1 Name: hanlp Version: 2.1.0b9 Summary: HanLP: Han Language
 Processing Home-page: https://github.com/hankcs/HanLP Author: hankcs Author-
 email: hankcshe@gmail.com License: Apache License 2.0 Description:
              [https://file.hankcs.com/img/hanlp-github-banner.png]
                   ***** HanLP: Han Language Processing *****
    [Run_Tests] [PyPI_Version] [Python_Versions] [Downloads] [Open_In_Colab]
                    *** ä¸­æ | æ¥æ¬èª | Docs | Forum ***
 The multilingual NLP library for researchers and companies, built on PyTorch
```

### Comparing `hanlp-2.1.0b8/README.md` & `hanlp-2.1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/__init__.py` & `hanlp-2.1.0b9/hanlp/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/callbacks/fine_csv_logger.py` & `hanlp-2.1.0b9/hanlp/callbacks/fine_csv_logger.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/component.py` & `hanlp-2.1.0b9/hanlp/common/component.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/dataset.py` & `hanlp-2.1.0b9/hanlp/common/dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/keras_component.py` & `hanlp-2.1.0b9/hanlp/common/keras_component.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/structure.py` & `hanlp-2.1.0b9/hanlp/common/structure.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/torch_component.py` & `hanlp-2.1.0b9/hanlp/common/torch_component.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/transform.py` & `hanlp-2.1.0b9/hanlp/common/transform.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/transform_tf.py` & `hanlp-2.1.0b9/hanlp/common/transform_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/vocab.py` & `hanlp-2.1.0b9/hanlp/common/vocab.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/common/vocab_tf.py` & `hanlp-2.1.0b9/hanlp/common/vocab_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/IO.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/IO.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/dataset.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/linearization.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/linearization.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/penman.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/penman.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/postprocessing.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/postprocessing.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/tokenization_bart.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/tokenization_bart.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/dataset/tokenization_t5.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/dataset/tokenization_t5.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/evaluation.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/evaluation.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/optim.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/optim.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/amr/seq2seq/seq2seq_amr_parser.py` & `hanlp-2.1.0b9/hanlp/components/amr/seq2seq/seq2seq_amr_parser.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/classifiers/transformer_classifier.py` & `hanlp-2.1.0b9/hanlp/components/classifiers/transformer_classifier.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/classifiers/transformer_classifier_tf.py` & `hanlp-2.1.0b9/hanlp/components/classifiers/transformer_classifier_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/distillation/distillable_component.py` & `hanlp-2.1.0b9/hanlp/components/distillation/distillable_component.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/distillation/losses.py` & `hanlp-2.1.0b9/hanlp/components/distillation/losses.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/distillation/schedulers.py` & `hanlp-2.1.0b9/hanlp/components/distillation/schedulers.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/eos/ngram.py` & `hanlp-2.1.0b9/hanlp/components/eos/ngram.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/lambda_wrapper.py` & `hanlp-2.1.0b9/hanlp/components/lambda_wrapper.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/lemmatizer.py` & `hanlp-2.1.0b9/hanlp/components/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/lm/mlm.py` & `hanlp-2.1.0b9/hanlp/components/lm/mlm.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/multi_task_learning.py` & `hanlp-2.1.0b9/hanlp/components/mtl/multi_task_learning.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/__init__.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/amr.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/amr.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/constituency.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/constituency.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/dep.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/dep.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/dep_2nd.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/dep_2nd.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/lem.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/lem.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/biaffine_ner.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/biaffine_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/ner/tag_ner.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/ner/tag_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/pos.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/pos.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/sdp.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/sdp.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/bio_srl.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/bio_srl.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/srl/rank_srl.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/srl/rank_srl.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/reg_tok.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/reg_tok.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/tok/tag_tok.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/tok/tag_tok.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/mtl/tasks/ud.py` & `hanlp-2.1.0b9/hanlp/components/mtl/tasks/ud.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/biaffine_ner.py` & `hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/biaffine_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/ner/biaffine_ner/biaffine_ner_model.py` & `hanlp-2.1.0b9/hanlp/components/ner/biaffine_ner/biaffine_ner_model.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/ner/ner_tf.py` & `hanlp-2.1.0b9/hanlp/components/ner/ner_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/ner/rnn_ner.py` & `hanlp-2.1.0b9/hanlp/components/ner/rnn_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/ner/transformer_ner.py` & `hanlp-2.1.0b9/hanlp/components/ner/transformer_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/alg.py` & `hanlp-2.1.0b9/hanlp/components/parsers/alg.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/alg_tf.py` & `hanlp-2.1.0b9/hanlp/components/parsers/alg_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_2nd_dep.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_2nd_dep.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_dep.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_dep.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_model.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_model.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/biaffine_sdp.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/biaffine_sdp.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/mlp.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/mlp.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/structual_attention.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/structual_attention.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine/variationalbilstm.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine/variationalbilstm.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine_parser_tf.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine_parser_tf.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import tensorflow as tf
 
 from hanlp.components.parsers.parse_alg import unique_root, adjust_root_score, chu_liu_edmonds
 from hanlp.layers.transformers.loader_tf import build_transformer
 
 from hanlp.common.keras_component import KerasComponent
 from hanlp.components.parsers.alg_tf import tarjan
-from hanlp.components.parsers.biaffine_tf.model import BiaffineModelTF, StructuralAttentionModel
+from hanlp.components.parsers.biaffine_tf.model import BiaffineModelTF
 from hanlp.transform.conll_tf import CoNLL_DEP_Transform, CoNLL_Transformer_Transform, CoNLL_SDP_Transform
 from hanlp.layers.embeddings.util_tf import build_embedding
 from hanlp.layers.transformers.tf_imports import PreTrainedTokenizer, TFAutoModel, TFPreTrainedModel, AutoTokenizer, \
     TFAutoModelWithLMHead, BertTokenizerFast, AlbertConfig, BertTokenizer, TFBertModel
 from hanlp.layers.transformers.utils_tf import build_adamw_optimizer
 from hanlp.metrics.parsing.labeled_f1_tf import LabeledF1TF
 from hanlp.metrics.parsing.labeled_score import LabeledScore
@@ -560,166 +560,7 @@
             max_samples_per_batch=None, epochs=100, tree=False, punct=False, token_mapping=None, enhanced_only=False,
             run_eagerly=False,
             logger=None, verbose=True, **kwargs):
         return super().fit(**merge_locals_kwargs(locals(), kwargs))
 
     def decode(self, arc_scores, rel_scores, mask):
         return BiaffineSemanticDependencyParserTF.decode(self, arc_scores, rel_scores, mask)
-
-
-class StructuralAttentionDependencyParserTF(BiaffineTransformerDependencyParserTF):
-
-    def build_model(self, transformer, training, masked_lm_embed=None, **kwargs) -> tf.keras.Model:
-        transformer = self.build_transformer(training, transformer)
-        self.config.num_heads = len(self.transform.rel_vocab)
-        if self.config.get('use_pos', None):
-            self.config.n_pos = len(self.transform.cpos_vocab)
-        if masked_lm_embed:
-            masked_lm_embed = build_embedding(masked_lm_embed, self.transform.form_vocab, self.transform)
-            masked_lm_embed(tf.constant(0))  # build it with sample data
-            masked_lm_embed = tf.transpose(masked_lm_embed._embeddings)
-        return StructuralAttentionModel(self.config, transformer, masked_lm_embed)
-
-    def fit(self, trn_data, dev_data, save_dir, transformer, max_seq_length=256, transformer_dropout=.33,
-            d_positional=None, mask_p=.15, masked_lm_dropout=None, masked_lm_embed=None, joint_pos=False, alpha=0.1,
-            sa_dim=None,
-            num_decoder_layers=1,
-            n_mlp_arc=500,
-            n_mlp_rel=100,
-            mlp_dropout=.33,
-            optimizer='adamw',
-            learning_rate=5e-5,
-            learning_rate_transformer=None, weight_decay_rate=0, epsilon=1e-8, clipnorm=None, fp16=False,
-            warmup_steps_ratio=0, arc_loss='sparse_categorical_crossentropy',
-            rel_loss='sparse_categorical_crossentropy', metrics=('UAS', 'LAS'), batch_size=3000, samples_per_batch=150,
-            epochs=100, tree=False, punct=False, token_mapping=None, run_eagerly=False, logger=None, verbose=True,
-            **kwargs):
-        return super().fit(**merge_locals_kwargs(locals(), kwargs))
-
-    def train_loop(self, trn_data, dev_data, epochs, num_examples, train_steps_per_epoch, dev_steps, model, optimizer,
-                   loss, metrics, callbacks, logger: logging.Logger, arc_loss, rel_loss, **kwargs):
-        arc_loss, rel_loss = loss
-        # because we are customizing batching
-        train_steps_per_epoch = len(list(iter(trn_data)))
-        # progbar: tf.keras.callbacks.ProgbarLogger = callbacks[-1]
-        c: tf.keras.callbacks.Callback = None
-        metrics = self._build_metrics()
-        acc: tf.keras.metrics.SparseCategoricalAccuracy = metrics[1]
-        for c in callbacks:
-            if not hasattr(c, 'params'):
-                c.params = {}
-            c.params['epochs'] = epochs
-            c.params['trn_data'] = trn_data
-            c.params['metrics'] = ['loss'] + self.config.metrics + [acc.name]
-            c.params['metrics'] = c.params['metrics'] + [f'val_{k}' for k in c.params['metrics']]
-            c.on_train_begin()
-        for epoch in range(epochs):
-            for metric in metrics:
-                metric.reset_states()
-            for c in callbacks:
-                c.params['steps'] = train_steps_per_epoch
-                c.on_epoch_begin(epoch)
-            for idx, ((words, feats), (arcs, rels, offsets)) in enumerate(iter(trn_data)):
-                logs = {}
-                for c in callbacks:
-                    c.on_batch_begin(idx, logs)
-                mask = tf.not_equal(words, self.config.pad_index) & tf.not_equal(words, self.config.bos_index)
-                loss, arc_scores, rel_scores, lm_ids = self.train_batch(words, feats, arcs, rels, offsets, mask,
-                                                                        optimizer, arc_loss, rel_loss, acc)
-                self.run_metrics(arcs, rels, arc_scores, rel_scores, words, mask, metrics[0])
-                logs['loss'] = loss
-                logs.update(metrics[0].to_dict())
-                logs[acc.name] = acc.result()
-                if epoch == epochs - 1:
-                    self.model.stop_training = True
-                for c in callbacks:
-                    c.on_batch_end(idx, logs)
-            # evaluate on dev
-            for metric in metrics:
-                metric.reset_states()
-            logs = {}
-            for idx, ((words, feats), (arcs, rels, offsets)) in enumerate(iter(dev_data)):
-                arc_scores, rel_scores, loss, mask, arc_preds, rel_preds = self.evaluate_batch(words, feats, arcs, rels,
-                                                                                               arc_loss, rel_loss,
-                                                                                               metrics[0])
-                logs['val_loss'] = loss
-                logs.update((f'val_{k}', v) for k, v in metrics[0].to_dict().items())
-
-            for c in callbacks:
-                c.on_epoch_end(epoch, logs)
-            if getattr(self.model, 'stop_training', None):
-                break
-
-        for c in callbacks:
-            c.on_train_end()
-
-    # noinspection PyMethodOverriding
-    def train_batch(self, words, feats, arcs, rels, ids, mask, optimizer, arc_loss, rel_loss, metric):
-        with tf.GradientTape() as tape:
-            arc_scores, rel_scores, lm_ids = self.model((words, feats), training=True)
-            loss = self.get_total_loss(words, feats, arcs, rels, arc_scores, rel_scores, arc_loss, rel_loss, ids,
-                                       lm_ids, mask,
-                                       metric)
-        grads = tape.gradient(loss, self.model.trainable_variables)
-        accum_grads = self.params['accum_grads']
-        for i, grad in enumerate(grads):
-            if grad is not None:
-                accum_grads[i].assign_add(grad)
-        self.params['trained_samples'] += tf.shape(words)[0]
-        if self.params['trained_samples'] >= self.config.samples_per_batch:
-            self._apply_grads(accum_grads)
-        return loss, arc_scores, rel_scores, lm_ids
-
-    def get_total_loss(self, words, feats, arcs, rels, arc_scores, rel_scores, arc_loss, rel_loss, gold_offsets,
-                       pred_ids,
-                       mask, metric):
-        masked_lm_loss = self.get_masked_lm_loss(words, feats, gold_offsets, pred_ids, metric)
-        # return masked_lm_loss
-        parser_loss = self.get_loss(arc_scores, rel_scores, arcs, rels, mask, arc_loss, rel_loss)
-        loss = parser_loss + masked_lm_loss * self.config.alpha
-        return loss
-
-    def get_masked_lm_loss(self, words, feats, gold_offsets, pred_ids, metric):
-        if self.config.get('joint_pos', None):
-            gold_ids = tf.gather(feats[-1], gold_offsets, batch_dims=1)
-        else:
-            gold_ids = tf.gather(words, gold_offsets, batch_dims=1)
-        pred_ids = tf.gather(pred_ids, gold_offsets, batch_dims=1)
-        masked_lm_loss = tf.keras.losses.sparse_categorical_crossentropy(gold_ids, pred_ids)
-        mask = gold_offsets != 0
-        if metric:
-            metric(gold_ids, pred_ids, mask)
-        return tf.reduce_mean(tf.boolean_mask(masked_lm_loss, mask))
-
-    def _build_metrics(self):
-        if not self.config['mask_p']:
-            return super()._build_metrics()
-        acc = tf.keras.metrics.SparseCategoricalAccuracy('accuracy')
-        return super()._build_metrics(), acc
-
-    def build_train_dataset(self, trn_data, batch_size, num_examples):
-        trn_data = self.transform.file_to_dataset(trn_data, batch_size=batch_size,
-                                                  shuffle=True,
-                                                  repeat=None,
-                                                  cache=False)  # Generate different masks every time
-        return trn_data
-
-    def build_loss(self, arc_loss, rel_loss, **kwargs):
-        if arc_loss == 'binary_crossentropy':
-            arc_loss = tf.losses.BinaryCrossentropy(from_logits=False)
-        else:
-            arc_loss = tf.keras.losses.SparseCategoricalCrossentropy(
-                from_logits=True) if arc_loss == 'sparse_categorical_crossentropy' else super().build_loss(arc_loss)
-        rel_loss = tf.keras.losses.SparseCategoricalCrossentropy(
-            from_logits=True) if rel_loss == 'sparse_categorical_crossentropy' else super().build_loss(rel_loss)
-        return arc_loss, rel_loss
-
-    def decode(self, arc_scores, rel_scores, mask):
-        if self.transform.graph:
-            return BiaffineSemanticDependencyParserTF.decode(self, arc_scores, rel_scores, mask)
-        return super().decode(arc_scores, rel_scores, mask)
-
-    def get_loss(self, arc_scores, rel_scores, arcs, rels, mask, arc_loss, rel_loss):
-        if self.transform.graph:
-            return BiaffineSemanticDependencyParserTF.get_loss(self, arc_scores, rel_scores, arcs, rels, mask, arc_loss,
-                                                               rel_loss)
-        return super().get_loss(arc_scores, rel_scores, arcs, rels, mask, arc_loss, rel_loss)
```

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/alg.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/alg.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/biaffine_tf/layers.py` & `hanlp-2.1.0b9/hanlp/components/parsers/biaffine_tf/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,68 @@
 # -*- coding:utf-8 -*-
 # Author: hankcs
-# Date: 2019-12-26 23:05
-# Ported from the PyTorch implementation https://github.com/zysite/biaffine-parser
+# Date: 2019-12-26 23:04
 import tensorflow as tf
-from params_flow import LayerNormalization
+from hanlp.layers.transformers.tf_imports import TFPreTrainedModel
+from hanlp.components.parsers.biaffine_tf.layers import IndependentDropout, SharedDropout, Biaffine, MLP
 
-from hanlp.utils.tf_util import tf_bernoulli
 
+class BiaffineModelTF(tf.keras.Model):
 
-class Biaffine(tf.keras.layers.Layer):
-    def __init__(self, n_in, n_out=1, bias_x=True, bias_y=True, trainable=True, name=None, dtype=None, dynamic=False,
-                 **kwargs):
-        super().__init__(trainable, name, dtype, dynamic, **kwargs)
-        self.n_in = n_in
-        self.n_out = n_out
-        self.bias_x = bias_x
-        self.bias_y = bias_y
-        self.weight = None
-
-    def build(self, input_shape):
-        self.weight = self.add_weight(name='kernel',
-                                      shape=(self.n_out,
-                                             self.n_in + self.bias_x,
-                                             self.n_in + self.bias_y),
-                                      initializer='zero')
-
-    def extra_repr(self):
-        s = f"n_in={self.n_in}, n_out={self.n_out}"
-        if self.bias_x:
-            s += f", bias_x={self.bias_x}"
-        if self.bias_y:
-            s += f", bias_y={self.bias_y}"
-
-        return s
-
-    # noinspection PyMethodOverriding
-    def call(self, x, y, **kwargs):
-        if self.bias_x:
-            x = tf.concat((x, tf.ones_like(x[..., :1])), -1)
-        if self.bias_y:
-            y = tf.concat((y, tf.ones_like(y[..., :1])), -1)
-        # [batch_size, n_out, seq_len, seq_len]
-        s = tf.einsum('bxi,oij,byj->boxy', x, self.weight, y)
-        # remove dim 1 if n_out == 1
-        if self.n_out == 1:
-            s = tf.squeeze(s, axis=1)
-
-        return s
-
-
-class MLP(tf.keras.layers.Layer):
-    def __init__(self, n_hidden, dropout=0, trainable=True, name=None, dtype=None, dynamic=False, **kwargs):
-        super().__init__(trainable, name, dtype, dynamic, **kwargs)
-        self.linear = tf.keras.layers.Dense(n_hidden, kernel_initializer='orthogonal')
-        self.activation = tf.keras.layers.LeakyReLU(0.1)
-        self.dropout = SharedDropout(p=dropout)
-
-    def call(self, x, **kwargs):
-        x = self.linear(x)
-        x = self.activation(x)
-        x = self.dropout(x)
-
-        return x
-
-
-class SharedDropout(tf.keras.layers.Layer):
-
-    def __init__(self, p=0.5, batch_first=True, trainable=True, name=None, dtype=None, dynamic=False, **kwargs):
-        """Dropout on timesteps with bernoulli distribution"""
-        super().__init__(trainable, name, dtype, dynamic, **kwargs)
-        self.p = p
-        self.batch_first = batch_first
-
-    def extra_repr(self):
-        s = f"p={self.p}"
-        if self.batch_first:
-            s += f", batch_first={self.batch_first}"
-
-        return s
-
-    def call(self, x, training=None, **kwargs):
-        if training and self.p > 0:
-            if self.batch_first:
-                mask = self.get_mask(x[:, 0], self.p)
-            else:
-                mask = self.get_mask(x[0], self.p)
-            x *= tf.expand_dims(mask, axis=1) if self.batch_first else mask
-
-        return x
-
-    @staticmethod
-    def get_mask(x, p):
-        mask = tf_bernoulli(tf.shape(x), 1 - p, x.dtype)
-        mask = mask / (1 - p)
-
-        return mask
-
-
-class IndependentDropout(tf.keras.layers.Layer):
-
-    def __init__(self, p=0.5, trainable=True, name=None, dtype=None, dynamic=False, **kwargs):
-        """Dropout on the first two dimensions"""
-        super().__init__(trainable, name, dtype, dynamic, **kwargs)
-        self.p = p
-
-    def extra_repr(self):
-        return f"p={self.p}"
-
-    def call(self, inputs, training=None, **kwargs):
-        if training and self.p > 0:
-            masks = [tf_bernoulli(tf.shape(x)[:2], 1 - self.p)
-                     for x in inputs]
-            total = sum(masks)
-            scale = len(inputs) / tf.reduce_max(tf.ones_like(total))
-            masks = [mask * scale for mask in masks]
-            inputs = [item * tf.expand_dims(mask, axis=-1)
-                      for item, mask in zip(inputs, masks)]
-
-        return inputs
-
-
-class StructuralAttentionLayer(tf.keras.layers.Layer):
-    def __init__(self, config, num_heads, x_dim, trainable=True, name=None, dtype=None, dynamic=False, **kwargs):
-        super().__init__(trainable, name, dtype, dynamic, **kwargs)
-
-        sa_dim = config.get('sa_dim', None)
-        if sa_dim:
-            self.shrink = tf.keras.layers.Dense(sa_dim, name='shrink')
-            x_dim = sa_dim
-
+    def __init__(self, config, embed=None, transformer: TFPreTrainedModel = None):
+        """An implementation of T. Dozat and C. D. Manning, “Deep Biaffine Attention for Neural Dependency Parsing.,” ICLR, 2017.
+            Although I have my MXNet implementation, I found zysite's PyTorch implementation is cleaner so I port it to TensorFlow
+
+        Args:
+          config: param embed:
+
+        Returns:
+
+        """
+        super(BiaffineModelTF, self).__init__()
+        assert not (embed and transformer), 'Either pre-trained word embed and transformer is supported, but not both'
+        normal = tf.keras.initializers.RandomNormal(stddev=1.)
+        if not transformer:
+            # the embedding layer
+            self.word_embed = tf.keras.layers.Embedding(input_dim=config.n_words,
+                                                        output_dim=config.n_embed,
+                                                        embeddings_initializer=tf.keras.initializers.zeros() if embed
+                                                        else normal,
+                                                        name='word_embed')
+            self.feat_embed = tf.keras.layers.Embedding(input_dim=config.n_feats,
+                                                        output_dim=config.n_embed,
+                                                        embeddings_initializer=tf.keras.initializers.zeros() if embed
+                                                        else normal,
+                                                        name='feat_embed')
+            self.embed_dropout = IndependentDropout(p=config.embed_dropout, name='embed_dropout')
+
+            # the word-lstm layer
+            self.lstm = tf.keras.models.Sequential(name='lstm')
+            for _ in range(config.n_lstm_layers):
+                self.lstm.add(tf.keras.layers.Bidirectional(tf.keras.layers.LSTM(
+                    units=config.n_lstm_hidden,
+                    dropout=config.lstm_dropout,
+                    recurrent_dropout=config.lstm_dropout,
+                    return_sequences=True,
+                    kernel_initializer='orthogonal',
+                    unit_forget_bias=False,  # turns out to hinder performance
+                )))
+            self.lstm_dropout = SharedDropout(p=config.lstm_dropout, name='lstm_dropout')
+        else:
+            self.transformer = transformer
+            transformer_dropout = config.get('transformer_dropout', None)
+            if transformer_dropout:
+                self.transformer_dropout = SharedDropout(p=config.transformer_dropout, name='transformer_dropout')
+            d_positional = config.get('d_positional', None)
+            if d_positional:
+                max_seq_length = config.get('max_seq_length', 256)
+                self.position_table = self.add_weight(shape=(max_seq_length, d_positional),
+                                                      initializer='random_normal',
+                                                      trainable=True)
+        # the MLP layers
         self.mlp_arc_h = MLP(n_hidden=config.n_mlp_arc,
                              dropout=config.mlp_dropout, name='mlp_arc_h')
         self.mlp_arc_d = MLP(n_hidden=config.n_mlp_arc,
                              dropout=config.mlp_dropout, name='mlp_arc_d')
         self.mlp_rel_h = MLP(n_hidden=config.n_mlp_rel,
                              dropout=config.mlp_dropout, name='mlp_rel_h')
         self.mlp_rel_d = MLP(n_hidden=config.n_mlp_rel,
@@ -142,44 +72,79 @@
         self.arc_attn = Biaffine(n_in=config.n_mlp_arc,
                                  bias_x=True,
                                  bias_y=False, name='arc_attn')
         self.rel_attn = Biaffine(n_in=config.n_mlp_rel,
                                  n_out=config.n_rels,
                                  bias_x=True,
                                  bias_y=True, name='rel_attn')
-        self.heads_WV = self.add_weight(shape=[num_heads, x_dim, x_dim])
-        self.dense = tf.keras.layers.Dense(x_dim)
-        self.layer_norm = LayerNormalization(name="LayerNorm")
-        self.graph = config.get('graph', False)
+        if embed is not None:
+            self.pretrained = embed
+        self.pad_index = tf.constant(config.pad_index, dtype=tf.int64)
+        self.unk_index = tf.constant(config.unk_index, dtype=tf.int64)
 
-    def call(self, inputs, mask=None, **kwargs):
-        x = inputs
+    # noinspection PyMethodOverriding
+    def call(self, inputs, mask_inf=True, **kwargs):
+        # batch_size, seq_len = words.shape
+        # get the mask and lengths of given batch
+        # mask = words.ne(self.pad_index)
+        if hasattr(self, 'lstm'):
+            words, feats = inputs
+            mask = tf.not_equal(words, self.pad_index)
+            # set the indices larger than num_embeddings to unk_index
+            # ext_mask = words.ge(self.word_embed.num_embeddings)
+            ext_mask = tf.greater_equal(words, self.word_embed.input_dim)
+            ext_words = tf.where(ext_mask, self.unk_index, words)
+
+            # get outputs from embedding layers
+            word_embed = self.word_embed(ext_words)
+            if hasattr(self, 'pretrained'):
+                word_embed += self.pretrained(words)
+            feat_embed = self.feat_embed(feats)
+            word_embed, feat_embed = self.embed_dropout([word_embed, feat_embed])
+            # concatenate the word and feat representations
+            embed = tf.concat((word_embed, feat_embed), axis=-1)
+
+            x = self.lstm(embed, mask=mask)
+            x = self.lstm_dropout(x)
+        else:
+            words, (input_ids, input_mask, prefix_offset) = inputs
+            mask = tf.not_equal(words, self.pad_index)
+            x = self.run_transformer(input_ids, input_mask, prefix_offset)
+
+        # apply MLPs to the BiLSTM output states
         arc_h = self.mlp_arc_h(x)
         arc_d = self.mlp_arc_d(x)
         rel_h = self.mlp_rel_h(x)
         rel_d = self.mlp_rel_d(x)
 
         # get arc and rel scores from the bilinear attention
         # [batch_size, seq_len, seq_len]
         s_arc = self.arc_attn(arc_d, arc_h)
-        # if mask is not None:
-        #     negative_infinity = -10000.0
-        #     s_arc += (1.0 - mask) * negative_infinity
-
         # [batch_size, seq_len, seq_len, n_rels]
         s_rel = tf.transpose(self.rel_attn(rel_d, rel_h), [0, 2, 3, 1])
-        if self.graph:
-            p_arc = tf.nn.sigmoid(s_arc - (1.0 - mask) * 10000.0)
+        # set the scores that exceed the length of each sentence to -inf
+        if mask_inf:
+            s_arc = tf.where(tf.expand_dims(mask, 1), s_arc, float('-inf'))
+
+        return s_arc, s_rel
+
+    def run_transformer(self, input_ids, input_mask, prefix_offset):
+        if isinstance(self.transformer, TFPreTrainedModel):
+            sequence_output = self.transformer([input_ids, input_mask])
+            sequence_output = sequence_output[0]
         else:
-            p_arc = tf.nn.softmax(s_arc - (1.0 - mask) * 10000.0, axis=-1)
-        p_rel = tf.nn.softmax(s_rel, axis=-1)
-        A = tf.expand_dims(p_arc, -1) * p_rel
-        A = tf.transpose(A, [0, 3, 1, 2])
-        if hasattr(self, 'shrink'):
-            x = self.shrink(x)
-        Ax = A @ tf.expand_dims(x, 1)
-        AxW = Ax @ self.heads_WV
-        AxW = tf.transpose(AxW, [0, 2, 1, 3])
-        AxW = tf.reshape(AxW, list(tf.shape(AxW)[:2]) + [-1])
-        x = self.dense(AxW) + x
-        x = self.layer_norm(x)
-        return s_arc, s_rel, x
+            sequence_output = self.transformer([input_ids, tf.zeros_like(input_ids)], mask=input_mask)
+        x = tf.gather(sequence_output, prefix_offset, batch_dims=1)
+        if hasattr(self, 'transformer_dropout'):
+            x = self.transformer_dropout(x)
+        if hasattr(self, 'position_table'):
+            batch_size, seq_length = tf.shape(x)[:2]
+            timing_signal = tf.broadcast_to(self.position_table[:seq_length],
+                                            [batch_size, seq_length, self.position_table.shape[-1]])
+            x = tf.concat([x, timing_signal], axis=-1)
+        return x
+
+    def to_functional(self):
+        words = tf.keras.Input(shape=[None], dtype=tf.int64, name='words')
+        feats = tf.keras.Input(shape=[None], dtype=tf.int64, name='feats')
+        s_arc, s_rel = self.call([words, feats], mask_inf=False)
+        return tf.keras.Model(inputs=[words, feats], outputs=[s_arc, s_rel])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/chu_liu_edmonds.py` & `hanlp-2.1.0b9/hanlp/components/parsers/chu_liu_edmonds.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/conll.py` & `hanlp-2.1.0b9/hanlp/components/parsers/conll.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/constituency/crf_constituency_model.py` & `hanlp-2.1.0b9/hanlp/components/parsers/constituency/crf_constituency_model.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/constituency/crf_constituency_parser.py` & `hanlp-2.1.0b9/hanlp/components/parsers/constituency/crf_constituency_parser.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/constituency/treecrf.py` & `hanlp-2.1.0b9/hanlp/components/parsers/constituency/treecrf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/parse_alg.py` & `hanlp-2.1.0b9/hanlp/components/parsers/parse_alg.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/lemma_edit.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/lemma_edit.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/tag_decoder.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/tag_decoder.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/ud_model.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/ud_model.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/ud_parser.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/ud_parser.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/udify_util.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/udify_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/parsers/ud/util.py` & `hanlp-2.1.0b9/hanlp/components/parsers/ud/util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/pipeline.py` & `hanlp-2.1.0b9/hanlp/components/pipeline.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/rnn_language_model_tf.py` & `hanlp-2.1.0b9/hanlp/components/rnn_language_model_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_bio/baffine_tagging.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_bio/baffine_tagging.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_bio/span_bio.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_bio/span_bio.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/highway_variational_lstm.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/highway_variational_lstm.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/inference_utils.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/inference_utils.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/layer.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/layer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/span_rank.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/span_rank.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/span_ranking_srl_model.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/span_ranking_srl_model.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/srl/span_rank/srl_eval_utils.py` & `hanlp-2.1.0b9/hanlp/components/srl/span_rank/srl_eval_utils.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/sts/transformer_sts.py` & `hanlp-2.1.0b9/hanlp/components/sts/transformer_sts.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/cnn_tagger_tf.py` & `hanlp-2.1.0b9/hanlp/components/taggers/cnn_tagger_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/ngram_conv/ngram_conv_tagger.py` & `hanlp-2.1.0b9/hanlp/components/taggers/ngram_conv/ngram_conv_tagger.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/rnn/rnntaggingmodel.py` & `hanlp-2.1.0b9/hanlp/components/taggers/rnn/rnntaggingmodel.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/rnn_tagger.py` & `hanlp-2.1.0b9/hanlp/components/taggers/rnn_tagger.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/rnn_tagger_tf.py` & `hanlp-2.1.0b9/hanlp/components/taggers/rnn_tagger_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/tagger.py` & `hanlp-2.1.0b9/hanlp/components/taggers/tagger.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/tagger_tf.py` & `hanlp-2.1.0b9/hanlp/components/taggers/tagger_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_tagger.py` & `hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_tagger.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_tagger_tf.py` & `hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_tagger_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/transformers/transformer_transform_tf.py` & `hanlp-2.1.0b9/hanlp/components/taggers/transformers/transformer_transform_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/taggers/util.py` & `hanlp-2.1.0b9/hanlp/components/taggers/util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/tokenizers/multi_criteria_cws_transformer.py` & `hanlp-2.1.0b9/hanlp/components/tokenizers/multi_criteria_cws_transformer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/tokenizers/tok.py` & `hanlp-2.1.0b9/hanlp/components/tokenizers/tok.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/tokenizers/tok_tf.py` & `hanlp-2.1.0b9/hanlp/components/tokenizers/tok_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/components/tokenizers/transformer.py` & `hanlp-2.1.0b9/hanlp/components/tokenizers/transformer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/coref/loaders/conll12coref.py` & `hanlp-2.1.0b9/hanlp/datasets/coref/loaders/conll12coref.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/eos/eos.py` & `hanlp-2.1.0b9/hanlp/datasets/eos/eos.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/eos/loaders/nn_eos.py` & `hanlp-2.1.0b9/hanlp/datasets/eos/loaders/nn_eos.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/lm/loaders/lm_dataset.py` & `hanlp-2.1.0b9/hanlp/datasets/lm/loaders/lm_dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/lu/glue.py` & `hanlp-2.1.0b9/hanlp/datasets/lu/glue.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/conll03.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/conll03.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/loaders/json_ner.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/loaders/json_ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/loaders/tsv.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/msra.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/msra.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/resume.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/resume.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/ner/weibo.py` & `hanlp-2.1.0b9/hanlp/datasets/ner/weibo.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/amr.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/amr.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ctb5.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ctb5.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ctb8.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ctb8.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ctb9.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ctb9.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/_ctb_utils.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/_ctb_utils.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/conll_dataset.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/conll_dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/loaders/constituency_dataset.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/loaders/constituency_dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ptb.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ptb.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/semeval15.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/semeval15.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/semeval16.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/semeval16.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ud/__init__.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ud/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud23.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud23.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud27.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud27.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/parsing/ud/ud27m.py` & `hanlp-2.1.0b9/hanlp/datasets/parsing/ud/ud27m.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/qa/hotpotqa.py` & `hanlp-2.1.0b9/hanlp/datasets/qa/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/srl/loaders/conll2012.py` & `hanlp-2.1.0b9/hanlp/datasets/srl/loaders/conll2012.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/srl/loaders/ontonotes_loader.py` & `hanlp-2.1.0b9/hanlp/datasets/srl/loaders/ontonotes_loader.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/_utils.py` & `hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/_utils.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/chinese.py` & `hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/chinese.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/srl/ontonotes5/english.py` & `hanlp-2.1.0b9/hanlp/datasets/srl/ontonotes5/english.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/sts/stsb.py` & `hanlp-2.1.0b9/hanlp/datasets/sts/stsb.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/chunking_dataset.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/chunking_dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/multi_criteria_cws/__init__.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/multi_criteria_cws/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/multi_criteria_cws/mcws_dataset.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/multi_criteria_cws/mcws_dataset.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/loaders/txt.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/loaders/txt.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/__init__.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/as_.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/as_.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/cityu.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/cityu.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/msr.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/msr.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/datasets/tokenization/sighan2005/pku.py` & `hanlp-2.1.0b9/hanlp/datasets/tokenization/sighan2005/pku.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/cnn_encoder.py` & `hanlp-2.1.0b9/hanlp/layers/cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/crf/crf.py` & `hanlp-2.1.0b9/hanlp/layers/crf/crf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/crf/crf_layer_tf.py` & `hanlp-2.1.0b9/hanlp/layers/crf/crf_layer_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/crf/crf_tf.py` & `hanlp-2.1.0b9/hanlp/layers/crf/crf_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/dropout.py` & `hanlp-2.1.0b9/hanlp/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/char_cnn.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/char_cnn.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/char_cnn_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/char_cnn_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/char_rnn.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/char_rnn.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/char_rnn_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/char_rnn_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/concat_embedding.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/concat_embedding.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_string_embedding.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_string_embedding.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_string_embedding_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_string_embedding_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/contextual_word_embedding.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/contextual_word_embedding.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/embedding.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/fast_text.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/fast_text.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/fast_text_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/fast_text_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/util.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/util_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/util_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/word2vec.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/embeddings/word2vec_tf.py` & `hanlp-2.1.0b9/hanlp/layers/embeddings/word2vec_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/feed_forward.py` & `hanlp-2.1.0b9/hanlp/layers/feed_forward.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/feedforward.py` & `hanlp-2.1.0b9/hanlp/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/scalar_mix.py` & `hanlp-2.1.0b9/hanlp/layers/scalar_mix.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/time_distributed.py` & `hanlp-2.1.0b9/hanlp/layers/time_distributed.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/__init__.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/encoder.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/encoder.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/loader_tf.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/loader_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/pt_imports.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/pt_imports.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/relative_transformer.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/relative_transformer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/resource.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/resource.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/utils.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/transformers/utils_tf.py` & `hanlp-2.1.0b9/hanlp/layers/transformers/utils_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/layers/weight_normalization.py` & `hanlp-2.1.0b9/hanlp/layers/weight_normalization.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/losses/sparse_categorical_crossentropy.py` & `hanlp-2.1.0b9/hanlp/losses/sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/accuracy.py` & `hanlp-2.1.0b9/hanlp/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/amr/smatch_eval.py` & `hanlp-2.1.0b9/hanlp/metrics/amr/smatch_eval.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/binary_chunking_f1.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/binary_chunking_f1.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/bmes_tf.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/bmes_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/chunking_f1.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/chunking_f1.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/chunking_f1_tf.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/chunking_f1_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/conlleval.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/conlleval.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/iobes_tf.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/iobes_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/chunking/sequence_labeling.py` & `hanlp-2.1.0b9/hanlp/metrics/chunking/sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/f1.py` & `hanlp-2.1.0b9/hanlp/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/metric.py` & `hanlp-2.1.0b9/hanlp/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/mtl.py` & `hanlp-2.1.0b9/hanlp/metrics/mtl.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/attachmentscore.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/attachmentscore.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/conllx_eval.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/conllx_eval.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_f1.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_f1.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_f1_tf.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_f1_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/labeled_score.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/labeled_score.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/semdep_eval.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/semdep_eval.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/parsing/span.py` & `hanlp-2.1.0b9/hanlp/metrics/parsing/span.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/spearman_correlation.py` & `hanlp-2.1.0b9/hanlp/metrics/spearman_correlation.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/metrics/srl/srlconll.py` & `hanlp-2.1.0b9/hanlp/metrics/srl/srlconll.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/optimizers/adamw/__init__.py` & `hanlp-2.1.0b9/hanlp/optimizers/adamw/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/optimizers/adamw/optimization.py` & `hanlp-2.1.0b9/hanlp/optimizers/adamw/optimization.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/__init__.py` & `hanlp-2.1.0b9/hanlp/pretrained/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/amr.py` & `hanlp-2.1.0b9/hanlp/pretrained/amr.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/constituency.py` & `hanlp-2.1.0b9/hanlp/pretrained/constituency.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/dep.py` & `hanlp-2.1.0b9/hanlp/pretrained/dep.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/fasttext.py` & `hanlp-2.1.0b9/hanlp/pretrained/fasttext.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/glove.py` & `hanlp-2.1.0b9/hanlp/pretrained/glove.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/mtl.py` & `hanlp-2.1.0b9/hanlp/pretrained/mtl.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/ner.py` & `hanlp-2.1.0b9/hanlp/pretrained/ner.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/pos.py` & `hanlp-2.1.0b9/hanlp/pretrained/pos.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/rnnlm.py` & `hanlp-2.1.0b9/hanlp/pretrained/rnnlm.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/sdp.py` & `hanlp-2.1.0b9/hanlp/pretrained/sdp.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/tok.py` & `hanlp-2.1.0b9/hanlp/pretrained/tok.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/pretrained/word2vec.py` & `hanlp-2.1.0b9/hanlp/pretrained/word2vec.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/conll_tf.py` & `hanlp-2.1.0b9/hanlp/transform/conll_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/glue_tf.py` & `hanlp-2.1.0b9/hanlp/transform/glue_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/table_tf.py` & `hanlp-2.1.0b9/hanlp/transform/table_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/tacred_tf.py` & `hanlp-2.1.0b9/hanlp/transform/tacred_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/text_tf.py` & `hanlp-2.1.0b9/hanlp/transform/text_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/transformer_tokenizer.py` & `hanlp-2.1.0b9/hanlp/transform/transformer_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/tsv_tf.py` & `hanlp-2.1.0b9/hanlp/transform/tsv_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/transform/txt_tf.py` & `hanlp-2.1.0b9/hanlp/transform/txt_tf.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/__init__.py` & `hanlp-2.1.0b9/hanlp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/component_util.py` & `hanlp-2.1.0b9/hanlp/utils/component_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/file_read_backwards/buffer_work_space.py` & `hanlp-2.1.0b9/hanlp/utils/file_read_backwards/buffer_work_space.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/file_read_backwards/file_read_backwards.py` & `hanlp-2.1.0b9/hanlp/utils/file_read_backwards/file_read_backwards.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/io_util.py` & `hanlp-2.1.0b9/hanlp/utils/io_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/lang/en/english_tokenizer.py` & `hanlp-2.1.0b9/hanlp/utils/lang/en/english_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/lang/ja/bert_tok.py` & `hanlp-2.1.0b9/hanlp/utils/lang/ja/bert_tok.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/lang/zh/char_table.py` & `hanlp-2.1.0b9/hanlp/utils/lang/zh/char_table.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/lang/zh/localization.py` & `hanlp-2.1.0b9/hanlp/utils/lang/zh/localization.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/log_util.py` & `hanlp-2.1.0b9/hanlp/utils/log_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/rules.py` & `hanlp-2.1.0b9/hanlp/utils/rules.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/span_util.py` & `hanlp-2.1.0b9/hanlp/utils/span_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/string_util.py` & `hanlp-2.1.0b9/hanlp/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/tf_util.py` & `hanlp-2.1.0b9/hanlp/utils/tf_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/time_util.py` & `hanlp-2.1.0b9/hanlp/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp/utils/torch_util.py` & `hanlp-2.1.0b9/hanlp/utils/torch_util.py`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/hanlp.egg-info/PKG-INFO` & `hanlp-2.1.0b9/hanlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hanlp
-Version: 2.1.0b8
+Version: 2.1.0b9
 Summary: HanLP: Han Language Processing
 Home-page: https://github.com/hankcs/HanLP
 Author: hankcs
 Author-email: hankcshe@gmail.com
 License: Apache License 2.0
 Description: <div align="center"><img src="https://file.hankcs.com/img/hanlp-github-banner.png" height="100px"/></div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hanlp Version: 2.1.0b8 Summary: HanLP: Han Language
+Metadata-Version: 2.1 Name: hanlp Version: 2.1.0b9 Summary: HanLP: Han Language
 Processing Home-page: https://github.com/hankcs/HanLP Author: hankcs Author-
 email: hankcshe@gmail.com License: Apache License 2.0 Description:
              [https://file.hankcs.com/img/hanlp-github-banner.png]
                   ***** HanLP: Han Language Processing *****
    [Run_Tests] [PyPI_Version] [Python_Versions] [Downloads] [Open_In_Colab]
                    *** ä¸­æ | æ¥æ¬èª | Docs | Forum ***
 The multilingual NLP library for researchers and companies, built on PyTorch
```

### Comparing `hanlp-2.1.0b8/hanlp.egg-info/SOURCES.txt` & `hanlp-2.1.0b9/hanlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hanlp-2.1.0b8/setup.py` & `hanlp-2.1.0b9/setup.py`

 * *Files identical despite different names*

