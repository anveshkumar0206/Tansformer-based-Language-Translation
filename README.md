# Tansformer-based-Language-Translation

Project Overview
This project implements a Transformer-based Neural Machine Translation system, translating from English-German in step1.ipynb file and German to English in step2.ipynb file. It is based on PyTorch and TorchText, following the standard architecture of language modeling with Transformers.

Installation
The project requires Python and dependencies such as PyTorch, TorchText, Spacy, and Matplotlib. Ensure you have the necessary libraries installed before running the notebooks.

Dataset
The model is trained on a German-English parallel corpus using TorchText datasets. The dataset consists of sentence pairs where each English sentence has a corresponding German translation.

Preprocessing
Tokenization is performed using SpaCy models (en_core_web_sm and de_core_news_sm).
Sentences are converted into numerical sequences using vocabulary indexing.
Special tokens like <sos> (start of sentence) and <eos> (end of sentence) are added to each sentence.

Model Training
The model is a Transformer-based sequence-to-sequence (Seq2Seq) model trained using cross-entropy loss. Training is performed for multiple epochs with gradient clipping and learning rate scheduling to improve performance.

Evaluation
The model is evaluated by: Measuring the BLEU score to assess translation quality and comparing model predictions with ground truth translations.

Inference
The trained model is used to: Translate English to German and Translate German to English.
Perform round-trip translation, where an English sentence is translated to German and then back to English.
