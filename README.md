# Anti-Vietnamese government text detection

## Overview
The Anti-Vietnamese government (rebellious) post classifier is built using deep learning techniques, specifically recurrent neural network (RNN) architectures such as GRU (Gated Recurrent Unit) and LSTM (Long Short-Term Memory). It takes as input text content, and predicts the rebellious level of the post. The classifier can identify whether posts are rebellious or not.
<br></br>
This repository contains code for a rebellious post classifier, a machine learning model designed to classify posts into different categories based on their toxicity levels. The classifier can be used to automatically detect and filter out rebellious posts, helping to create safer online communities.

## Dependencies
The Anti-Vietnamese government (rebellious) post classifier requires the following dependencies:
- Python 3.x
- NumPy
- Pandas
- Torch
- NLTK (Natural Language Toolkit)
- gensim

## Experiments

### Model Evaluation Results Summary

| Model (File)   | Accuracy | F1-Score   |
| -------------- | -------- | ---------- |
| `BERT`         | **0.92** | **0.6444** |
| `mBART`        | 0.89     | 0.52       |
| `Vistral`      | 0.90     | 0.60       |
| `Transformers` | 0.88     | 0.56       |
| `GRU`          | 0.85     | 0.45       |

### Insight
Even though Vistral is a Vietnamese-native LLM, BERT remains the strongest model for classification because encoder-based architectures are optimized for discriminative decision boundaries, not generation. Vistral understands Vietnamese well, but its larger generative design requires more data and tuning to adapt effectively to classification, whereas BERT learns compact class-separating features more efficiently on a dataset of this scale. In short, language specialization alone is not enough; task-oriented architecture still plays a dominant role in performance.

## Members
Members:
- Nguyễn Đức Anh
- Nguyễn Kim Hoàng Anh
- Nguyễn Tiến Hùng
- Chu Hữu Đăng Trường
