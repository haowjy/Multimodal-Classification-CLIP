# Exploration of Multimodal Text and Image Classification
---

by Jimmy Yao and Yuxuan Zhang


This is an independent group project for the course [CSC 298: Deep Learning](https://www.cs.rochester.edu/~cxu22/t/298F21/). This repo contains the code for our project.

## Project Description

In this project, we explore multimodal text and image classification. We explore different models used in multimodal learning, including convolutional neural networks (CNNs), long short-term memory (LSTM) networks, and pre-trained embeddings such as CLIP (Contrastive Language-Image Pre-training). We train and evaluate these models on the [Fakeddit](https://github.com/entitize/Fakeddit) dataset, which contains images and text descriptions labeled with up to 6 different labels of various types of fake/misleading information.

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