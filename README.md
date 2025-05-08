# Multimodal Sentiment Analysis: Text and Image Fusion

## Overview

This project focuses on building a **Multimodal Sentiment Analysis** system that uses both **text** and **image** data. The main goal is to improve sentiment classification by combining the strengths of both text and visual information. The model uses **attention fusion** techniques to merge features from both modalities in a meaningful way.

## Key Components

1. **Text Classifier**: A model that processes textual input using **word embeddings** and an **LSTM** layer. This part of the model extracts key features from the text data.
  
2. **Image Classifier**: A model that processes images to pull out important features, often using pre-trained CNN models like **ResNet** or **VGG**.

3. **Multimodal Classifier**: The fusion model that brings together both **text** and **image** features. It applies an **attention-based fusion** technique to combine both modalities effectively, and then classifies the input into sentiment categories.

## Workflow

1. **Text Preprocessing**: The text data is processed with a pre-trained embedding matrix, followed by an LSTM layer to capture the sequential context of the text.
2. **Image Preprocessing**: The image data is passed through a CNN model to extract relevant features.
3. **Multimodal Fusion**: Features from both text and images are fused using an attention mechanism, where the model learns to focus on the most important parts of both data types.
4. **Classification**: The combined features are fed into a final classification layer to predict the sentiment label.
