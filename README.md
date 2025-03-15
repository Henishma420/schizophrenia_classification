# schizophrenia_classification
Overview
This dataset was created for a machine learning project aimed at distinguishing schizophrenia-related content from general discussions in control groups using deep learning models like BiLSTM and BERT.

Dataset Description
The dataset consists of Reddit posts collected from schizophrenia-related and control subreddits. After preprocessing, the final dataset comprises:

8,007 posts from r/schizophrenia
9,000 posts each from each of the four control subreddits:
🏋 r/fitness
😂 r/jokes
💑 r/relationships
👨‍👩‍👧‍👦 r/parenting
Total: 44,007 posts
Split:
Training set: 35,205 posts (80%)
Validation set: 8,802 posts (20%)
Data Format
Each post is represented with:
input_ids – Tokenized post input for the BERT model.
attention_mask – Mask indicating which tokens are real vs. padding.
labels – Assigned labels (0 to 4), where:
0: r/schizophrenia
1: r/fitness
2: r/jokes
3: r/relationships
4: r/parenting
Usage
The dataset can be used for sentiment analysis, mental health research, and NLP classification tasks. The trained models (.pt files) are included for inference.

Model & Training
Preprocessing: Tokenization using BERT tokenizer.
Models Used: BiLSTM, BERT and hybrid model(BERT+BiLSTM) for classification.
Framework: PyTorch.
