# Exploration of Multimodal Text and Image Classification

by Jimmy Yao and Yezeyuan Zheng


This is an independent group project for the course [CSC 298: Deep Learning](https://www.cs.rochester.edu/~cxu22/t/298F22/). This repo contains the code for our project.

## Project Description

In this project, we explore multimodal text and image classification. We explore different models used in multimodal learning, including convolutional neural networks (CNNs), long short-term memory (LSTM) networks, and pre-trained embeddings such as [CLIP](https://github.com/openai/CLIP) (Contrastive Language-Image Pre-training). We train and evaluate these models on the [Fakeddit](https://github.com/entitize/Fakeddit) dataset, which contains images and text descriptions labeled with up to 6 different labels of various types of fake/misleading information.

We combine CNN and LSTM and also evaluate using the LSTM and CNN alone for the first 3 models. Then, we use combine CLIP text embeddings with CLIP image embeddings (ViT-B/32) and concatenate both embeddings to be passed into a 3-layer Multilayer Perceptron (MLP) network. We also evaluate using CLIP text embeddings or CLIP image embeddings alone. These are the second batch of 3 models. Finally, instead of passing the embeddings into a MLP, we perform linear probing by passing them into a simple multiclass logistic regression to produce our final 3 models.

## Final Results

| Model                   | Train Accuracy | Test Accuracy |
|-------------------------|----------------|---------------|
| CNN-LSTM                | 61.75\%        | 59.14\%       |
| LSTM                    | 62.20\%        | 59.11\%       |
| CNN                     | 40.31\%        | 39.51\%       |
| CLIP MLP Cat            | 82.174\%       | 72.906\%      |
| CLIP MLP Text Transformer | 66.633\%       | 63.299\%      |
| CLIP MLP ViT            | 66.440\%       | 64.212\%      |
| CLIP Linear Probe (LP) Cat | 91.710\%       | 86.029\%      |
| CLIP LP Text Transformer  | 77.892\%       | 74.459\%      |
| CLIP LP ViT               | 82.775\%       | 79.787\%      |
