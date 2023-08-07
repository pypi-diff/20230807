# Comparing `tmp/hezar-0.21.0.tar.gz` & `tmp/hezar-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.21.0.tar", max compression
+gzip compressed data, was "hezar-0.21.1.tar", max compression
```

## Comparing `hezar-0.21.0.tar` & `hezar-0.21.1.tar`

### file list

```diff
@@ -1,95 +1,97 @@
--rw-r--r--   0        0        0     1065 2023-08-06 20:15:26.873012 hezar-0.21.0/LICENSE
--rw-r--r--   0        0        0     4750 2023-08-06 20:15:26.873012 hezar-0.21.0/README.md
--rw-r--r--   0        0        0      260 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/builders.py
--rw-r--r--   0        0        0    11587 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      320 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1771 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4545 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3653 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3581 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0       26 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4804 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3270 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3301 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1656 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1728 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1686 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11774 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/model.py
--rw-r--r--   0        0        0     1434 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/model_outputs.py
--rw-r--r--   0        0        0      152 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     4076 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4184 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     3941 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0      240 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3710 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2939 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4165 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0     1733 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/text_classification.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      155 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     4494 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     3652 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      324 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19486 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2282 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    18229 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      190 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5615 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/core_utils.py
--rw-r--r--   0        0        0      531 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     3666 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-06 20:15:26.877012 hezar-0.21.0/pyproject.toml
--rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-06 22:01:50.097564 hezar-0.21.1/LICENSE
+-rw-r--r--   0        0        0     4750 2023-08-06 22:01:50.097564 hezar-0.21.1/README.md
+-rw-r--r--   0        0        0      260 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/builders.py
+-rw-r--r--   0        0        0    11587 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1771 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4804 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3270 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3301 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2161 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11774 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/model.py
+-rw-r--r--   0        0        0     1528 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0      152 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     4094 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2802 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0     1642 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/sequence_labeling.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     2948 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0     1088 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/text2text.py
+-rw-r--r--   0        0        0      240 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3377 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3437 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0     1733 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/text_classification.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4494 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3652 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19486 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    18229 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      190 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5615 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0      531 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     3666 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-06 22:01:50.101564 hezar-0.21.1/pyproject.toml
+-rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.1/PKG-INFO
```

### Comparing `hezar-0.21.0/LICENSE` & `hezar-0.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/README.md` & `hezar-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/builders.py` & `hezar-0.21.1/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/configs.py` & `hezar-0.21.1/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/constants.py` & `hezar-0.21.1/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/data_collators.py` & `hezar-0.21.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/datasets/dataset.py` & `hezar-0.21.1/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.21.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.21.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.21.1/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/data/utils/data_utils.py` & `hezar-0.21.1/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/embeddings/embedding.py` & `hezar-0.21.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/embeddings/fasttext.py` & `hezar-0.21.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/embeddings/word2vec.py` & `hezar-0.21.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/metrics/f1.py` & `hezar-0.21.1/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/metrics/metric.py` & `hezar-0.21.1/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/metrics/recall.py` & `hezar-0.21.1/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/metrics/seqeval.py` & `hezar-0.21.1/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """
-A BERT Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
+A DistilBERT Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
 """
 from typing import List, Union
 
-from transformers import BertConfig, BertModel
+from transformers import DistilBertConfig, DistilBertModel
 
 from ....models import Model
 from ....registry import register_model
-from .bert_lm_config import BertLMConfig
+from .distilbert_lm_config import DistilBertLMConfig
 
 
-@register_model("bert_lm", config_class=BertLMConfig)
-class BertLM(Model):
+@register_model("distilbert_lm", config_class=DistilBertLMConfig)
+class DistilBertLM(Model):
     tokenizer_name = "wordpiece_tokenizer"
 
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
-        self.bert = BertModel(BertConfig(**self.config))
+        self.distilbert = DistilBertModel(DistilBertConfig(**self.config))
 
     def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
-        outputs = self.bert(
+        head_mask = inputs.get("head_mask", None)
+        inputs_embeds = inputs.get("inputs_embeds", None)
+        output_attentions = inputs.get("output_attentions", None)
+        output_hidden_states = inputs.get("output_hidden_states", None)
+
+        outputs = self.distilbert(
             input_ids=input_ids,
             attention_mask=attention_mask,
-            **kwargs,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=True,
         )
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
```

### Comparing `hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.21.1/hezar/models/sequence_labeling/sequence_labeling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 """
-A DistilBERT Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
+A Base class for sequence labeling models
 """
-from typing import List, Union
+from typing import Dict, Union, List
 
-from transformers import DistilBertConfig, DistilBertModel
+from ...models import Model
 
-from ....models import Model
-from ....registry import register_model
-from .distilbert_lm_config import DistilBertLMConfig
-
-
-@register_model("distilbert_lm", config_class=DistilBertLMConfig)
-class DistilBertLM(Model):
-    tokenizer_name = "wordpiece_tokenizer"
-
-    def __init__(self, config, **kwargs):
-        super().__init__(config=config, **kwargs)
-        self.distilbert = DistilBertModel(DistilBertConfig(**self.config))
-
-    def forward(self, inputs, **kwargs):
-        input_ids = inputs.get("token_ids")
-        attention_mask = inputs.get("attention_mask", None)
-        outputs = self.distilbert(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            **kwargs,
-        )
-        return outputs
 
+class SequenceLabelingModel(Model):
+    """
+    Base class for all sequence labeling models (Also a Model subclass)
+    """
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor[self.tokenizer_name]
-        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
+        inputs = tokenizer(
+            inputs,
+            return_word_ids=True,
+            return_tokens=True,
+            padding=True,
+            truncation=True,
+            return_tensors="pt",
+            device=self.device,
+        )
         return inputs
 
     def post_process(self, inputs, **kwargs):
-        hidden_states = inputs.get("hidden_states", None)
-        attentions = inputs.get("attentions", None)
-        outputs = {
-            "last_hidden_state": inputs.get("last_hidden_state"),
-            "hidden_states": hidden_states,
-            "attentions": attentions,
-        }
+        # TODO sequence labeling outputs should consider rejoining split words into single words with proper tag
+        logits = inputs["logits"]
+        tokens = inputs["tokens"]
+        word_ids = inputs["word_ids"]  # noqa
+        predictions = logits.argmax(2).cpu()
+        predictions = [[self.config.id2label[p.item()] for p in prediction] for prediction in predictions]
+        outputs = []
+        for tokens_list, prediction in zip(tokens, predictions):
+            results = []
+            for token, tag in zip(tokens_list, prediction):
+                if token not in self.config.prediction_skip_tokens:
+                    results.append({"token": token, "tag": tag})
+            outputs.append(results)
         return outputs
```

### Comparing `hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/model.py` & `hezar-0.21.1/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/model_outputs.py` & `hezar-0.21.1/hezar/models/model_outputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import torch
 
 
 @dataclass
 class ModelOutputs:
     """
     Base class for all model outputs (named based on tasks)
+
+    The helper functions in the class enable it to be treated as a mapping or a dict object.
     """
 
     def dict(self):
         return asdict(self)
 
     def __getitem__(self, item):
         try:
```

### Comparing `hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 A BERT model for sequence labeling built using HuggingFace Transformers
 """
 from typing import Dict, List, Union
 
 from torch import nn
 from transformers import BertConfig, BertModel
 
-from ....models import Model
 from ....registry import register_model
+from ..sequence_labeling import SequenceLabelingModel
 from .bert_sequence_labeling_config import BertSequenceLabelingConfig
 
-
 @register_model("bert_sequence_labeling", BertSequenceLabelingConfig)
-class BertSequenceLabeling(Model):
+class BertSequenceLabeling(SequenceLabelingModel):
     """
     BERT model for sequence labeling
     """
     tokenizer_name = "wordpiece_tokenizer"
 
     def __init__(self, config: BertSequenceLabelingConfig, **kwargs):
         super().__init__(config, **kwargs)
@@ -50,15 +49,14 @@
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            **kwargs,
         )
         sequence_output = lm_outputs[0]
 
         sequence_output = self.dropout(sequence_output)
         logits = self.classifier(sequence_output)
 
         outputs = {
```

### Comparing `hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.21.1/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,40 +38,39 @@
             self.config.num_labels = len(self.config.id2label)
         bert_config = BertConfig(**self.config)
         return bert_config
 
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
-        token_types_ids = inputs.get("token_type_ids", None) or kwargs.get("token_type_ids", None)
-        position_ids = inputs.get("position_ids", None) or kwargs.get("position_ids", None)
+        token_types_ids = inputs.get("token_type_ids", None)
+        position_ids = inputs.get("position_ids", None)
         head_mask = inputs.get("head_mask", None)
         inputs_embeds = inputs.get("inputs_embeds", None)
-        encoder_hidden_states = inputs.get("encoder_hidden_states", None) or kwargs.get("encoder_hidden_states", None)
-        encoder_attention_mask = inputs.get("encoder_attention_mask", None) or kwargs.get("encoder_attention_mask", None)
-        past_key_values = inputs.get("past_key_values", None) or kwargs.get("past_key_values", None)
-        use_cache = inputs.get("use_cache", None) or kwargs.get("use_cache", None)
+        encoder_hidden_states = inputs.get("encoder_hidden_states", None)
+        encoder_attention_mask = inputs.get("encoder_attention_mask", None)
+        past_key_values = inputs.get("past_key_values", None)
+        use_cache = inputs.get("use_cache", None)
         output_attentions = inputs.get("output_attentions", None)
         output_hidden_states = inputs.get("output_hidden_states", None)
-        return_dict = inputs.get("return_dict", None) or kwargs.get("return_dict", None)
 
         lm_outputs = self.bert(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_types_ids,
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             past_key_values=past_key_values,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+            return_dict=True,
         )
         pooled_output = lm_outputs[1]
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
```

### Comparing `hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,24 +39,23 @@
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
         head_mask = inputs.get("head_mask", None)
         inputs_embeds = inputs.get("inputs_embeds", None)
         output_attentions = inputs.get("output_attentions", None)
         output_hidden_states = inputs.get("output_hidden_states", None)
-        return_dict = inputs.get("return_dict", None) or kwargs.get("return_dict", None)
 
         lm_outputs = self.distilbert(
-            input_ids,
+            input_ids=input_ids,
             attention_mask=attention_mask,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+            return_dict=True,
         )
         hidden_state = lm_outputs[0]
         pooled_output = hidden_state[:, 0]
         pooled_output = self.pre_classifier(pooled_output)
         pooled_output = nn.ReLU()(pooled_output)
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
```

### Comparing `hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/models/text_classification/text_classification.py` & `hezar-0.21.1/hezar/models/text_classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/preprocessor.py` & `hezar-0.21.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/text_normalizer.py` & `hezar-0.21.1/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.21.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.21.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.21.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/registry.py` & `hezar-0.21.1/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.21.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.21.1/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/trainers/trainer.py` & `hezar-0.21.1/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/trainers/trainer_utils.py` & `hezar-0.21.1/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/utils/common_utils.py` & `hezar-0.21.1/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/utils/core_utils.py` & `hezar-0.21.1/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/utils/file_utils.py` & `hezar-0.21.1/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/utils/hub_utils.py` & `hezar-0.21.1/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/hezar/utils/registry_utils.py` & `hezar-0.21.1/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.0/pyproject.toml` & `hezar-0.21.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.21.0"
+version = "0.21.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.21.0/PKG-INFO` & `hezar-0.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.21.0
+Version: 0.21.1
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

