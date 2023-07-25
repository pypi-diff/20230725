# Comparing `tmp/botiverse-0.4.5.tar.gz` & `tmp/botiverse-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.4.5.tar", last modified: Tue Jul 25 18:17:18 2023, max compression
+gzip compressed data, was "botiverse-0.4.6.tar", last modified: Tue Jul 25 18:22:03 2023, max compression
```

## Comparing `botiverse-0.4.5.tar` & `botiverse-0.4.6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.120777 botiverse-0.4.5/
--rw-rw-rw-   0        0        0      187 2023-07-25 17:54:38.000000 botiverse-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1534 2023-07-25 18:17:18.118776 botiverse-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-07-25 17:54:38.000000 botiverse-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.845781 botiverse-0.4.5/botiverse/
--rw-rw-rw-   0        0        0       84 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.865781 botiverse-0.4.5/botiverse/bots/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.871778 botiverse-0.4.5/botiverse/bots/BasicBot/
--rw-rw-rw-   0        0        0     7769 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/BasicBot/BasicBot.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/BasicBot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.875775 botiverse-0.4.5/botiverse/bots/ConverseBot/
--rw-rw-rw-   0        0        0     6760 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/ConverseBot/ConverseBot.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/ConverseBot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.885774 botiverse-0.4.5/botiverse/bots/VoiceBot/
--rw-rw-rw-   0        0        0     4309 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/VoiceBot/SpeechClassifier.py
--rw-rw-rw-   0        0        0     3533 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/VoiceBot/VoiceBot.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/VoiceBot/__init__.py
--rw-rw-rw-   0        0        0     1758 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/VoiceBot/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.892776 botiverse-0.4.5/botiverse/bots/WhizBot/
--rw-rw-rw-   0        0        0     2691 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot.py
--rw-rw-rw-   0        0        0     5084 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot_BERT.py
--rw-rw-rw-   0        0        0     5309 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot_GRU.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/WhizBot/__init__.py
--rw-rw-rw-   0        0        0      407 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.904778 botiverse-0.4.5/botiverse/bots/basic_TODS/
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/basic_TODS/__init__.py
--rw-rw-rw-   0        0        0     4076 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/basic_TODS/basic_TODS.py
--rw-rw-rw-   0        0        0     1387 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/basic_TODS/tods_example.py
--rw-rw-rw-   0        0        0     7368 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/basic_TODS/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.909776 botiverse-0.4.5/botiverse/bots/deep_TODS/
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/deep_TODS/__init__.py
--rw-rw-rw-   0        0        0     5990 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/deep_TODS/deep_TODS.py
--rw-rw-rw-   0        0        0     5169 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/bots/deep_TODS/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.915774 botiverse-0.4.5/botiverse/gui/
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/gui.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.922770 botiverse-0.4.5/botiverse/gui/static/
--rw-rw-rw-   0        0        0    13342 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/favicon.png
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.942772 botiverse-0.4.5/botiverse/gui/static/icons/
--rw-rw-rw-   0        0        0   116487 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Basic Bot.png
--rw-rw-rw-   0        0        0   194391 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Converse Bot.png
--rw-rw-rw-   0        0        0   194873 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Task Bot.png
--rw-rw-rw-   0        0        0    99768 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Theorizer.png
--rw-rw-rw-   0        0        0    77851 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Voice Bot.png
--rw-rw-rw-   0        0        0   119550 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/icons/Whiz Bot.png
--rw-rw-rw-   0        0        0    39966 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/logo.png
--rw-rw-rw-   0        0        0     4448 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/static/style.css
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.946788 botiverse-0.4.5/botiverse/gui/templates/
--rw-rw-rw-   0        0        0     3732 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/gui/templates/chat.html
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.950783 botiverse-0.4.5/botiverse/models/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.966784 botiverse-0.4.5/botiverse/models/BERT/
--rw-rw-rw-   0        0        0    11321 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/BERT/BERT.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/BERT/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/BERT/config.py
--rw-rw-rw-   0        0        0     3282 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/BERT/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.975771 botiverse-0.4.5/botiverse/models/FastSpeech1/
--rw-rw-rw-   0        0        0    29110 2023-07-25 18:15:40.000000 botiverse-0.4.5/botiverse/models/FastSpeech1/FastSpeech.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/FastSpeech1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.980775 botiverse-0.4.5/botiverse/models/GRUClassifier/
--rw-rw-rw-   0        0        0     4483 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/GRUClassifier/GRUClassifier.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/GRUClassifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.986773 botiverse-0.4.5/botiverse/models/LSTM/
--rw-rw-rw-   0        0        0    11718 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/LSTM/LSTM.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/LSTM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.989778 botiverse-0.4.5/botiverse/models/LinearClassifier/
--rw-rw-rw-   0        0        0     1214 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/LinearClassifier/LinearClassifier.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/LinearClassifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.996787 botiverse-0.4.5/botiverse/models/NN/
--rw-rw-rw-   0        0        0    13533 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/NN/NN.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/NN/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/NN/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.003775 botiverse-0.4.5/botiverse/models/SVM/
--rw-rw-rw-   0        0        0     9087 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/SVM/SVM.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/SVM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.007775 botiverse-0.4.5/botiverse/models/T5Model/
--rw-rw-rw-   0        0        0    30038 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/T5Model/T5Model.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/T5Model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.054773 botiverse-0.4.5/botiverse/models/TRIPPY/
--rw-rw-rw-   0        0        0     5185 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/TRIPPY.py
--rw-rw-rw-   0        0        0     9192 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/TRIPPY_DST.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/__init__.py
--rw-rw-rw-   0        0        0     3618 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/config.py
--rw-rw-rw-   0        0        0    21274 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/data.py
--rw-rw-rw-   0        0        0     9398 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/evaluate.py
--rw-rw-rw-   0        0        0     4778 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/infer.py
--rw-rw-rw-   0        0        0     6225 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/run.py
--rw-rw-rw-   0        0        0     5068 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/train.py
--rw-rw-rw-   0        0        0    12849 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/utils.py
--rw-rw-rw-   0        0        0   231498 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/TRIPPY/vocab.txt
--rw-rw-rw-   0        0        0      558 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.056774 botiverse-0.4.5/botiverse/preprocessors/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.061783 botiverse-0.4.5/botiverse/preprocessors/BertEmbeddings/
--rw-rw-rw-   0        0        0     3958 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/BertEmbeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.068785 botiverse-0.4.5/botiverse/preprocessors/BoW/
--rw-rw-rw-   0        0        0     1671 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/BoW/BoW.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/BoW/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.073772 botiverse-0.4.5/botiverse/preprocessors/Frequency/
--rw-rw-rw-   0        0        0     9973 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Frequency/Frequency.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Frequency/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.077772 botiverse-0.4.5/botiverse/preprocessors/GloVe/
--rw-rw-rw-   0        0        0     2995 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/GloVe/GloVe.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/GloVe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.830779 botiverse-0.4.5/botiverse/preprocessors/Special/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.084779 botiverse-0.4.5/botiverse/preprocessors/Special/ConverseBot_Preprocessor/
--rw-rw-rw-   0        0        0     5317 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/ConverseBot_Preprocessor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.089776 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/
--rw-rw-rw-   0        0        0     5445 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.092779 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/
--rw-rw-rw-   0        0        0     5515 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.098776 botiverse-0.4.5/botiverse/preprocessors/TF_IDF/
--rw-rw-rw-   0        0        0     2493 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/TF_IDF/TF_IDF.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/TF_IDF/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.105772 botiverse-0.4.5/botiverse/preprocessors/TF_IDF_GLOVE/
--rw-rw-rw-   0        0        0     2763 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/TF_IDF_GLOVE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.109773 botiverse-0.4.5/botiverse/preprocessors/Vocalize/
--rw-rw-rw-   0        0        0     5466 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Vocalize/Vocalize.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Vocalize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:18.115795 botiverse-0.4.5/botiverse/preprocessors/Wav2Vec/
--rw-rw-rw-   0        0        0     6904 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Wav2Vec/Wav2Vec.py
--rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/Wav2Vec/__init__.py
--rw-rw-rw-   0        0        0      584 2023-07-25 17:54:38.000000 botiverse-0.4.5/botiverse/preprocessors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:17:17.861773 botiverse-0.4.5/botiverse.egg-info/
--rw-rw-rw-   0        0        0     1534 2023-07-25 18:17:17.000000 botiverse-0.4.5/botiverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2023-07-25 18:17:17.000000 botiverse-0.4.5/botiverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:17:17.000000 botiverse-0.4.5/botiverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      272 2023-07-25 18:17:17.000000 botiverse-0.4.5/botiverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 18:17:17.000000 botiverse-0.4.5/botiverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 18:17:18.120777 botiverse-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     4559 2023-07-25 18:16:44.000000 botiverse-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.442040 botiverse-0.4.6/
+-rw-rw-rw-   0        0        0      187 2023-07-25 17:54:38.000000 botiverse-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1534 2023-07-25 18:22:03.441043 botiverse-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-07-25 17:54:38.000000 botiverse-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.111604 botiverse-0.4.6/botiverse/
+-rw-rw-rw-   0        0        0       84 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.136030 botiverse-0.4.6/botiverse/bots/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.141032 botiverse-0.4.6/botiverse/bots/BasicBot/
+-rw-rw-rw-   0        0        0     7769 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/BasicBot/BasicBot.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/BasicBot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.144035 botiverse-0.4.6/botiverse/bots/ConverseBot/
+-rw-rw-rw-   0        0        0     6760 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/ConverseBot/ConverseBot.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/ConverseBot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.155033 botiverse-0.4.6/botiverse/bots/VoiceBot/
+-rw-rw-rw-   0        0        0     4309 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/VoiceBot/SpeechClassifier.py
+-rw-rw-rw-   0        0        0     3533 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/VoiceBot/VoiceBot.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/VoiceBot/__init__.py
+-rw-rw-rw-   0        0        0     1758 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/VoiceBot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.161029 botiverse-0.4.6/botiverse/bots/WhizBot/
+-rw-rw-rw-   0        0        0     2691 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot.py
+-rw-rw-rw-   0        0        0     5084 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot_BERT.py
+-rw-rw-rw-   0        0        0     5309 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot_GRU.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/WhizBot/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.169028 botiverse-0.4.6/botiverse/bots/basic_TODS/
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/basic_TODS/__init__.py
+-rw-rw-rw-   0        0        0     4076 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/basic_TODS/basic_TODS.py
+-rw-rw-rw-   0        0        0     1387 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/basic_TODS/tods_example.py
+-rw-rw-rw-   0        0        0     7368 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/basic_TODS/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.174033 botiverse-0.4.6/botiverse/bots/deep_TODS/
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/deep_TODS/__init__.py
+-rw-rw-rw-   0        0        0     5990 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/deep_TODS/deep_TODS.py
+-rw-rw-rw-   0        0        0     5169 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/bots/deep_TODS/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.176029 botiverse-0.4.6/botiverse/gui/
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/gui.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.184043 botiverse-0.4.6/botiverse/gui/static/
+-rw-rw-rw-   0        0        0    13342 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/favicon.png
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.193032 botiverse-0.4.6/botiverse/gui/static/icons/
+-rw-rw-rw-   0        0        0   116487 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Basic Bot.png
+-rw-rw-rw-   0        0        0   194391 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Converse Bot.png
+-rw-rw-rw-   0        0        0   194873 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Task Bot.png
+-rw-rw-rw-   0        0        0    99768 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Theorizer.png
+-rw-rw-rw-   0        0        0    77851 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Voice Bot.png
+-rw-rw-rw-   0        0        0   119550 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/icons/Whiz Bot.png
+-rw-rw-rw-   0        0        0    39966 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/logo.png
+-rw-rw-rw-   0        0        0     4448 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/static/style.css
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.195030 botiverse-0.4.6/botiverse/gui/templates/
+-rw-rw-rw-   0        0        0     3732 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/gui/templates/chat.html
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.197033 botiverse-0.4.6/botiverse/models/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.205027 botiverse-0.4.6/botiverse/models/BERT/
+-rw-rw-rw-   0        0        0    11321 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/BERT/BERT.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/BERT/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/BERT/config.py
+-rw-rw-rw-   0        0        0     3282 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/BERT/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.209038 botiverse-0.4.6/botiverse/models/FastSpeech1/
+-rw-rw-rw-   0        0        0    29123 2023-07-25 18:20:02.000000 botiverse-0.4.6/botiverse/models/FastSpeech1/FastSpeech.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/FastSpeech1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.214038 botiverse-0.4.6/botiverse/models/GRUClassifier/
+-rw-rw-rw-   0        0        0     4483 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/GRUClassifier/GRUClassifier.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/GRUClassifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.219027 botiverse-0.4.6/botiverse/models/LSTM/
+-rw-rw-rw-   0        0        0    11718 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/LSTM/LSTM.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/LSTM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.222032 botiverse-0.4.6/botiverse/models/LinearClassifier/
+-rw-rw-rw-   0        0        0     1214 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/LinearClassifier/LinearClassifier.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/LinearClassifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.227027 botiverse-0.4.6/botiverse/models/NN/
+-rw-rw-rw-   0        0        0    13533 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/NN/NN.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/NN/__init__.py
+-rw-rw-rw-   0        0        0     1358 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/NN/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.233029 botiverse-0.4.6/botiverse/models/SVM/
+-rw-rw-rw-   0        0        0     9087 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/SVM/SVM.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/SVM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.235062 botiverse-0.4.6/botiverse/models/T5Model/
+-rw-rw-rw-   0        0        0    30038 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/T5Model/T5Model.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/T5Model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.388058 botiverse-0.4.6/botiverse/models/TRIPPY/
+-rw-rw-rw-   0        0        0     5185 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/TRIPPY.py
+-rw-rw-rw-   0        0        0     9192 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/TRIPPY_DST.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/__init__.py
+-rw-rw-rw-   0        0        0     3618 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/config.py
+-rw-rw-rw-   0        0        0    21274 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/data.py
+-rw-rw-rw-   0        0        0     9398 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/evaluate.py
+-rw-rw-rw-   0        0        0     4778 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/infer.py
+-rw-rw-rw-   0        0        0     6225 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/run.py
+-rw-rw-rw-   0        0        0     5068 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/train.py
+-rw-rw-rw-   0        0        0    12849 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/utils.py
+-rw-rw-rw-   0        0        0   231498 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/TRIPPY/vocab.txt
+-rw-rw-rw-   0        0        0      558 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.390044 botiverse-0.4.6/botiverse/preprocessors/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.396051 botiverse-0.4.6/botiverse/preprocessors/BertEmbeddings/
+-rw-rw-rw-   0        0        0     3958 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/BertEmbeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.406039 botiverse-0.4.6/botiverse/preprocessors/BoW/
+-rw-rw-rw-   0        0        0     1671 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/BoW/BoW.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/BoW/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.413042 botiverse-0.4.6/botiverse/preprocessors/Frequency/
+-rw-rw-rw-   0        0        0     9973 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Frequency/Frequency.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Frequency/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.418048 botiverse-0.4.6/botiverse/preprocessors/GloVe/
+-rw-rw-rw-   0        0        0     2995 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/GloVe/GloVe.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/GloVe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:02.734015 botiverse-0.4.6/botiverse/preprocessors/Special/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.422041 botiverse-0.4.6/botiverse/preprocessors/Special/ConverseBot_Preprocessor/
+-rw-rw-rw-   0        0        0     5317 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/ConverseBot_Preprocessor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.424039 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/
+-rw-rw-rw-   0        0        0     5445 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.426039 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/
+-rw-rw-rw-   0        0        0     5515 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.429066 botiverse-0.4.6/botiverse/preprocessors/TF_IDF/
+-rw-rw-rw-   0        0        0     2493 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/TF_IDF/TF_IDF.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/TF_IDF/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.435038 botiverse-0.4.6/botiverse/preprocessors/TF_IDF_GLOVE/
+-rw-rw-rw-   0        0        0     2763 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/TF_IDF_GLOVE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.438040 botiverse-0.4.6/botiverse/preprocessors/Vocalize/
+-rw-rw-rw-   0        0        0     5466 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Vocalize/Vocalize.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Vocalize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.440037 botiverse-0.4.6/botiverse/preprocessors/Wav2Vec/
+-rw-rw-rw-   0        0        0     6904 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Wav2Vec/Wav2Vec.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/Wav2Vec/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-07-25 17:54:38.000000 botiverse-0.4.6/botiverse/preprocessors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:03.134042 botiverse-0.4.6/botiverse.egg-info/
+-rw-rw-rw-   0        0        0     1534 2023-07-25 18:22:02.000000 botiverse-0.4.6/botiverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-07-25 18:22:02.000000 botiverse-0.4.6/botiverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:22:02.000000 botiverse-0.4.6/botiverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      272 2023-07-25 18:22:02.000000 botiverse-0.4.6/botiverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 18:22:02.000000 botiverse-0.4.6/botiverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:22:03.442040 botiverse-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     4559 2023-07-25 18:21:17.000000 botiverse-0.4.6/setup.py
```

### Comparing `botiverse-0.4.5/PKG-INFO` & `botiverse-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.4.5
+Version: 0.4.6
 Summary: botiverse is a chatbot library that offers a high-level API to     access a diverse set of chatbot models
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Description: # Botiverse
         A library that imports chatbots from other galaxies
```

### Comparing `botiverse-0.4.5/botiverse/bots/BasicBot/BasicBot.py` & `botiverse-0.4.6/botiverse/bots/BasicBot/BasicBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/ConverseBot/ConverseBot.py` & `botiverse-0.4.6/botiverse/bots/ConverseBot/ConverseBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/VoiceBot/SpeechClassifier.py` & `botiverse-0.4.6/botiverse/bots/VoiceBot/SpeechClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/VoiceBot/VoiceBot.py` & `botiverse-0.4.6/botiverse/bots/VoiceBot/VoiceBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/VoiceBot/utils.py` & `botiverse-0.4.6/botiverse/bots/VoiceBot/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot.py` & `botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot_BERT.py` & `botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot_BERT.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/WhizBot/WhizBot_GRU.py` & `botiverse-0.4.6/botiverse/bots/WhizBot/WhizBot_GRU.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/basic_TODS/basic_TODS.py` & `botiverse-0.4.6/botiverse/bots/basic_TODS/basic_TODS.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/basic_TODS/tods_example.py` & `botiverse-0.4.6/botiverse/bots/basic_TODS/tods_example.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/basic_TODS/utils.py` & `botiverse-0.4.6/botiverse/bots/basic_TODS/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/deep_TODS/deep_TODS.py` & `botiverse-0.4.6/botiverse/bots/deep_TODS/deep_TODS.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/bots/deep_TODS/utils.py` & `botiverse-0.4.6/botiverse/bots/deep_TODS/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/gui.py` & `botiverse-0.4.6/botiverse/gui/gui.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/favicon.png` & `botiverse-0.4.6/botiverse/gui/static/favicon.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Basic Bot.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Basic Bot.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Converse Bot.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Converse Bot.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Task Bot.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Task Bot.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Theorizer.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Theorizer.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Voice Bot.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Voice Bot.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/icons/Whiz Bot.png` & `botiverse-0.4.6/botiverse/gui/static/icons/Whiz Bot.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/logo.png` & `botiverse-0.4.6/botiverse/gui/static/logo.png`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/static/style.css` & `botiverse-0.4.6/botiverse/gui/static/style.css`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/gui/templates/chat.html` & `botiverse-0.4.6/botiverse/gui/templates/chat.html`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/BERT/BERT.py` & `botiverse-0.4.6/botiverse/models/BERT/BERT.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/BERT/config.py` & `botiverse-0.4.6/botiverse/models/BERT/config.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/BERT/utils.py` & `botiverse-0.4.6/botiverse/models/BERT/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/FastSpeech1/FastSpeech.py` & `botiverse-0.4.6/botiverse/models/FastSpeech1/FastSpeech.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # # <font color="cyan">FastSpeech 1.0 </font> Implementation
 # 
 # In this notebook, we shall demonstrate implementing FastSpeech 1.0 from scratch for inference purposes. 
 
-# In[1]:
+# In[14]:
 
 
 '''
 FastSpeech 1.0 interface and implementation from scratch in PyTorch for inference.
 '''
 import torch
 import torch.nn as nn
@@ -152,15 +152,15 @@
 #   such that
 # 
 #   $\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right) \cdot V$
 # 
 #   
 #   </div>
 
-# In[2]:
+# In[15]:
 
 
 class MultiHeadAttention(nn.Module):
     '''
     Multi-Head Attention module with a residual connection and layer normalization. Used as self-attention in the FFT block of the encoder and decoder.
     '''
     def __init__(self, num_head, emb_dim, h_dim, dropout=0.1):
@@ -231,15 +231,15 @@
         return output
 
 
 # #### <font color="white"> Conv1D Network </font>
 
 # $Embeddings ⇒ Conv1D ⇒ ReuLU ⇒ Conv1D ⇒  Dropout ⇒ AddNorm$
 
-# In[3]:
+# In[16]:
 
 
 class Conv1DNet(nn.Module):
     '''
     1D convolutional network with residual connection and layer normalization. Used in the FFT block of the encoder and decoder.
     '''
     
@@ -276,15 +276,15 @@
         return output
 
 
 # #### <font color="white"> FFT Block </font>
 # 
 # Here we just put the two pieces together
 
-# In[4]:
+# In[17]:
 
 
 class FFTBlock(torch.nn.Module):
     '''
     FFT block used in the encoder and decoder. It consists of a Multi-Head Attention module and a 1D convolutional network.
     '''
     def __init__(self,  emb_dim, num_head, h_dim,  inner_dim, dropout=0.1):
@@ -331,15 +331,15 @@
 # 
 # 
 # $$PE_{(pos, 2i+1)} = \cos(\frac{{pos}}{{10000^{2i/d_{\text{inp}}}}})$$
 # 
 
 # The purpose of this is to add some notion of order to the input sequence without distorting it by adding a positional depending signal
 
-# In[5]:
+# In[18]:
 
 
 class SinusoidEncodingTable:
     '''
     Sinusoid encoding table used in the encoder and decoder. It is used to add positional information to the input embeddings.
     '''
     def __init__(self, max_seq_len, inp_dim, padding_idx=None):
@@ -379,15 +379,15 @@
         return torch.Tensor(sinusoid_table)
 
 
 # #### <font color="white"> Dencoder </font>
 # 
 # This is both the encoder and decoder in one module
 
-# In[6]:
+# In[19]:
 
 
 class Dencoder(nn.Module):
     '''
     A single module that implements the encoder and decoder of the FastSpeech 1.0 model. 
     '''
     def __init__(self, mode, vocab_dim, max_seq_len, emb_dim, num_layer, num_head, h_dim, d_inner, mel_num, dropout):
@@ -443,15 +443,15 @@
 # ![](https://i.imgur.com/xUvPwh6.png)
 
 # #### <font color="white"> Duration Predictor </font>
 # 
 
 # $PhonemeEmb ⇒ Conv1D ⇒ ReuLU ⇒ LayerNorm ⇒  Dropout ⇒ Conv1D ⇒ ReuLU ⇒ LayerNorm ⇒  Dropout ⇒ Relu ⇒ Linear$
 
-# In[7]:
+# In[20]:
 
 
 class DurationPredictor(nn.Module):
     '''
     Duration predictor module. It predicts the duration of each phoneme in the input sequence of encoder phoneme embeddings.
     '''
     def __init__(self, inp_dim, inner_dim, kernel_size, padding_size, dropout=0.1):
@@ -500,15 +500,15 @@
 
 
 # #### <font color="white">Length Regulation Logic </font>
 # 
 
 # Given $H=[h_1, h_2, ..., h_n]$ as phone embeddings from the encoder predict the duration of each phoneme $d=[d_1, d_2, ..., d_n]$ and repeat accordingly.
 
-# In[8]:
+# In[21]:
 
 
 class LengthRegulator(nn.Module):
     '''
     Length regulator module. It repeats the encoder outputs according to the predicted duration of each phoneme in the input sequence of encoder phoneme embeddings.
     '''
     def __init__(self, inp_dim, inner_dim, kernel_size, padding_size, dropout=0.1):
@@ -555,15 +555,15 @@
 
 # ### <font color="cyan">4. Model </font>
 
 # ![](https://i.imgur.com/azh7cwn.png)
 
 # #### Hyperparameters
 
-# In[9]:
+# In[22]:
 
 
 # Encoder
 VOCAB_SIZE = 300
 ENC_EMB_DIM = 256
 ENC_NUM_LAYER = 4
 ENC_NUM_HEAD = 2
@@ -584,15 +584,15 @@
 DEC_1D_FILTER_SIZE = 1024
 MEL_NUM = 80
 
 
 # #### <font color="white">FastSpeech</font>
 # 
 
-# In[10]:
+# In[23]:
 
 
 class FastSpeech(nn.Module):
     '''
     FastSpeech 1.0 model. It consists of an encoder, a duration predictor, a length regulator and a decoder.
     '''
     def __init__(self):
@@ -633,29 +633,29 @@
 
 # ![](https://i.imgur.com/Xl9HEgm.png)
 
 #  </font>
 
 # ## <font color="yellow"> Inference </font>
 
-# In[11]:
+# In[24]:
 
 
 import warnings; warnings.filterwarnings("ignore")
 from scipy.io.wavfile import write
 try:
     from playsound import playsound
+    import waveglow
 except:
     pass
 import os
-import waveglow
 import gdown
 
 
-# In[12]:
+# In[25]:
 
 
 class TTS():
     def __init__(self, force_download_wg=False, force_download_fs=False):
         '''
         Initialize the FastSpeech 1.0 model and the WaveGlow model. 
         force_download_wg: whether to force download the WaveGlow weights in case they already seems to exist 
@@ -709,14 +709,14 @@
         if play:
             write('sample.wav', 22050, audio.astype('int16'))
             playsound("sample.wav")
             os.remove("sample.wav")
         return audio
 
 
-# In[13]:
+# In[26]:
 
 
 # if running from notebook
 if __name__ == '__main__':
     get_ipython().system('jupyter nbconvert --to script FastSpeech.ipynb')
```

### Comparing `botiverse-0.4.5/botiverse/models/GRUClassifier/GRUClassifier.py` & `botiverse-0.4.6/botiverse/models/GRUClassifier/GRUClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/LSTM/LSTM.py` & `botiverse-0.4.6/botiverse/models/LSTM/LSTM.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/LinearClassifier/LinearClassifier.py` & `botiverse-0.4.6/botiverse/models/LinearClassifier/LinearClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/NN/NN.py` & `botiverse-0.4.6/botiverse/models/NN/NN.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/NN/utils.py` & `botiverse-0.4.6/botiverse/models/NN/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/SVM/SVM.py` & `botiverse-0.4.6/botiverse/models/SVM/SVM.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/T5Model/T5Model.py` & `botiverse-0.4.6/botiverse/models/T5Model/T5Model.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/TRIPPY.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/TRIPPY.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/TRIPPY_DST.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/TRIPPY_DST.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/config.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/config.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/data.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/data.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/evaluate.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/evaluate.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/infer.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/infer.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/run.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/run.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/train.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/train.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/utils.py` & `botiverse-0.4.6/botiverse/models/TRIPPY/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/TRIPPY/vocab.txt` & `botiverse-0.4.6/botiverse/models/TRIPPY/vocab.txt`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/models/__init__.py` & `botiverse-0.4.6/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py` & `botiverse-0.4.6/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/BoW/BoW.py` & `botiverse-0.4.6/botiverse/preprocessors/BoW/BoW.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Frequency/Frequency.py` & `botiverse-0.4.6/botiverse/preprocessors/Frequency/Frequency.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/GloVe/GloVe.py` & `botiverse-0.4.6/botiverse/preprocessors/GloVe/GloVe.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py` & `botiverse-0.4.6/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py` & `botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py` & `botiverse-0.4.6/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/TF_IDF/TF_IDF.py` & `botiverse-0.4.6/botiverse/preprocessors/TF_IDF/TF_IDF.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py` & `botiverse-0.4.6/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Vocalize/Vocalize.py` & `botiverse-0.4.6/botiverse/preprocessors/Vocalize/Vocalize.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/Wav2Vec/Wav2Vec.py` & `botiverse-0.4.6/botiverse/preprocessors/Wav2Vec/Wav2Vec.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse/preprocessors/__init__.py` & `botiverse-0.4.6/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/botiverse.egg-info/PKG-INFO` & `botiverse-0.4.6/botiverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.4.5
+Version: 0.4.6
 Summary: botiverse is a chatbot library that offers a high-level API to     access a diverse set of chatbot models
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Description: # Botiverse
         A library that imports chatbots from other galaxies
```

### Comparing `botiverse-0.4.5/botiverse.egg-info/SOURCES.txt` & `botiverse-0.4.6/botiverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botiverse-0.4.5/setup.py` & `botiverse-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return requirements
 
 
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.4.5",
+    version="0.4.6",
     description='''botiverse is a chatbot library that offers a high-level API to
     access a diverse set of chatbot models''',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://botiverse.readthedocs.io/",
     author="Essam W., Mohamed Saad, Yousef Atef, Karim Taha",
     author_email="essamwisam@outlook.com",
```

