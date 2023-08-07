# Comparing `tmp/hezar-0.21.1.tar.gz` & `tmp/hezar-0.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.21.1.tar", max compression
+gzip compressed data, was "hezar-0.21.2.tar", max compression
```

## Comparing `hezar-0.21.1.tar` & `hezar-0.21.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1065 2023-08-06 22:01:50.097564 hezar-0.21.1/LICENSE
--rw-r--r--   0        0        0     4750 2023-08-06 22:01:50.097564 hezar-0.21.1/README.md
--rw-r--r--   0        0        0      260 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/builders.py
--rw-r--r--   0        0        0    11587 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      320 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1771 2023-08-06 22:01:50.097564 hezar-0.21.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4545 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3653 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3581 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0       26 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4804 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3270 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3301 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     2743 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     2161 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     2743 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11774 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/model.py
--rw-r--r--   0        0        0     1528 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/model_outputs.py
--rw-r--r--   0        0        0      152 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     4094 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     2802 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0     1642 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/sequence_labeling/sequence_labeling.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     2948 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0     1088 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text2text/text2text.py
--rw-r--r--   0        0        0      240 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3377 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2853 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3437 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0     1733 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_classification/text_classification.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      155 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     4494 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     3652 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      324 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19486 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2282 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    18229 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      190 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5615 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/core_utils.py
--rw-r--r--   0        0        0      531 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     3666 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-06 22:01:50.101564 hezar-0.21.1/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-06 22:01:50.101564 hezar-0.21.1/pyproject.toml
--rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 05:55:55.828773 hezar-0.21.2/LICENSE
+-rw-r--r--   0        0        0     4750 2023-08-07 05:55:55.828773 hezar-0.21.2/README.md
+-rw-r--r--   0        0        0      260 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/builders.py
+-rw-r--r--   0        0        0    11587 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1771 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     5129 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     4810 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     4864 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2161 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     2743 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-07 05:55:55.828773 hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11774 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/model.py
+-rw-r--r--   0        0        0     1528 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0      152 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     4094 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     2802 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0     1642 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/sequence_labeling/sequence_labeling.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     2948 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0     1088 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text2text/text2text.py
+-rw-r--r--   0        0        0      240 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3377 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3437 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0     1733 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_classification/text_classification.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4494 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3652 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19486 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    18229 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      190 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5615 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0      531 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     3666 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-07 05:55:55.832773 hezar-0.21.2/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-07 05:55:55.832773 hezar-0.21.2/pyproject.toml
+-rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.2/PKG-INFO
```

### Comparing `hezar-0.21.1/LICENSE` & `hezar-0.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/README.md` & `hezar-0.21.2/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/builders.py` & `hezar-0.21.2/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/configs.py` & `hezar-0.21.2/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/constants.py` & `hezar-0.21.2/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/data_collators.py` & `hezar-0.21.2/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/datasets/dataset.py` & `hezar-0.21.2/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.21.2/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.21.2/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.21.2/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/data/utils/data_utils.py` & `hezar-0.21.2/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/embeddings/embedding.py` & `hezar-0.21.2/hezar/embeddings/embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,26 @@
     def word2index(self, word):
         return self.vocab.get(word, -1)
 
     def index2word(self, index):
         keyed_vocab = {v: k for v, k in self.vocab.items()}
         return keyed_vocab[index]
 
+    def similarity(self, word1: str, word2: str):
+        raise NotImplementedError
+
+    def doesnt_match(self, words: List[str]):
+        raise NotImplementedError
+
+    def most_similar(self, word: str, top_n: int = 5):
+        raise NotImplementedError
+
+    def get_normed_vectors(self):
+        raise NotImplementedError
+
     @classmethod
     def load(
         cls,
         hub_or_local_path,
         config_filename=None,
         subfolder=None,
         **kwargs,
```

### Comparing `hezar-0.21.1/hezar/embeddings/word2vec.py` & `hezar-0.21.2/hezar/embeddings/word2vec.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,21 +42,34 @@
             if not os.path.isdir(pretrained_path):
                 embedding_path = hf_hub_download(
                     pretrained_path,
                     filename=self.filename,
                     subfolder=self.subfolder,
                     cache_dir=HEZAR_CACHE_DIR,
                 )
-
+                vectors_path = hf_hub_download(
+                    pretrained_path,
+                    filename=self.vectors_filename,
+                    subfolder=self.subfolder,
+                    cache_dir=HEZAR_CACHE_DIR,
+                )
             else:
                 embedding_path = os.path.join(
                     pretrained_path,
                     self.subfolder,
                     self.filename,
                 )
+                vectors_path = os.path.join(
+                    pretrained_path,
+                    self.subfolder,
+                    self.vectors_filename,
+                )
+            if not os.path.isfile(vectors_path):
+                raise ValueError(f"Could not load or find vectors file at `{vectors_path}`! "
+                                 f"Please make sure it's been downloaded properly!")
             embedding_model = word2vec.Word2Vec.load(embedding_path)
         else:
             embedding_model = word2vec.Word2Vec(
                 vector_size=self.config.vector_size,
                 window=self.config.window,
                 sg=1 if self.config.train_algorithm == "skipgram" else 0,
                 workers=self.config.workers,
@@ -94,14 +107,35 @@
 
         save_dir = os.path.join(path, subfolder)
         os.makedirs(save_dir, exist_ok=True)
         self.config.save(path, config_filename, subfolder=subfolder)
 
         self.model.save(os.path.join(save_dir, filename))
 
+    def similarity(self, word1: str, word2: str):
+        if not isinstance(word1, str) or not isinstance(word2, str):
+            raise ValueError(f"`Embedding.similarity()` takes two string objects!\n"
+                             f"`word1`: {type(word1)}, `word2`: {type(word2)}")
+        similarity = self.word_vectors.similarity(word1, word2)
+        return similarity
+
+    def doesnt_match(self, words: List[str]):
+        doesnt_match = self.word_vectors.doesnt_match(words)
+        return doesnt_match
+
+    def most_similar(self, word: str, top_n: int = 5):
+        if not isinstance(word, str):
+            raise ValueError(f"`word` must be `str`, got `{type(word)}`!")
+        most_similar = self.word_vectors.most_similar(word, topn=top_n)
+        return most_similar
+
+    def get_normed_vectors(self):
+        normed_vectors = self.word_vectors.get_normed_vectors()
+        return normed_vectors
+
     @property
     def word_vectors(self):
         return self.model.wv
 
     @property
     def vectors(self):
         return self.model.wv.vectors
```

### Comparing `hezar-0.21.1/hezar/metrics/f1.py` & `hezar-0.21.2/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/metrics/metric.py` & `hezar-0.21.2/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/metrics/recall.py` & `hezar-0.21.2/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/metrics/seqeval.py` & `hezar-0.21.2/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.21.2/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.21.2/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.21.2/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/model.py` & `hezar-0.21.2/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/model_outputs.py` & `hezar-0.21.2/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.21.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.21.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/sequence_labeling/sequence_labeling.py` & `hezar-0.21.2/hezar/models/sequence_labeling/sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text2text/t5/t5_text2text.py` & `hezar-0.21.2/hezar/models/text2text/t5/t5_text2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.21.2/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text2text/text2text.py` & `hezar-0.21.2/hezar/models/text2text/text2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.21.2/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.21.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.21.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/models/text_classification/text_classification.py` & `hezar-0.21.2/hezar/models/text_classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/preprocessor.py` & `hezar-0.21.2/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/text_normalizer.py` & `hezar-0.21.2/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.21.2/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.21.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.21.2/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.21.2/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/registry.py` & `hezar-0.21.2/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.21.2/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.21.2/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/trainers/trainer.py` & `hezar-0.21.2/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/trainers/trainer_utils.py` & `hezar-0.21.2/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/utils/common_utils.py` & `hezar-0.21.2/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/utils/core_utils.py` & `hezar-0.21.2/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/utils/file_utils.py` & `hezar-0.21.2/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/utils/hub_utils.py` & `hezar-0.21.2/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/hezar/utils/registry_utils.py` & `hezar-0.21.2/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.21.1/pyproject.toml` & `hezar-0.21.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.21.1"
+version = "0.21.2"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.21.1/PKG-INFO` & `hezar-0.21.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.21.1
+Version: 0.21.2
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

