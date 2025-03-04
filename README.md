# Neural Machine Translation (NMT)

## Overview

This project focuses on building a `Neural Machine Translation (NMT)` system for English-to-Vietnamese translation using deep learning techniques. Two model architectures are implemented:

- GRU-based Sequence-to-Sequence Model (`nt_gru.ipynb`)
- Transformer-based Model (`nt_transformer.ipynb`)

The goal is to translate text from English to Vietnamese using deep learning techniques.

## Dataset

The models are trained and evaluated on the `IWSLT’15 English-Vietnamese` dataset, which consists of:
- **Training set**: 133,317 sentence pairs
- **Validation set**: 1,553 sentence pairs
- **Test set**: 1,269 sentence pair

## Methodologies

**1. GRU Model**: 

- Uses an `Encoder-decoder` architecture with `GRU`.
- Implements `teacher forcing` during training and `greedy decoding` for inference.

**2. Transformer-based Model**:

- Utilizes `multi-head self-attentio`n and `positional encoding` for efficient translation.
- Employs `beam search decoding` to improve translation accuracy.

## Evaluation Metric

Both models are evaluated using the `BLEU (Bilingual Evaluation Understudy)` score, a standard metric for machine translation performance.

## Running the Project

**GRU (`nt_gru.ipynb`)**

1. Load and preprocess the dataset.
2. Train the GRU-based NMT model.
3. Evaluate using BLEU score.

**Transformer (`nt_transformer.ipynb`)**

1. Load and preprocess the dataset.
2. Train the Transformer-based NMT model.
3. Evaluate using BLEU score.

## Result

The `Transformer model` generally outperforms the `GRU model` in translation quality.
