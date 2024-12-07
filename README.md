# Mixed-emotion-analysis

This is the core code for article [Mixed emotion extraction analysis and visualisation of social media text](https://www.sciencedirect.com/science/article/pii/S0169023X23000800)

## Introduction

The code consists of 2 main components in the article: 

- The correlation of the selected emotion labels from the SemEval-2018 Twitter sentiment dataset
- The multi-label emotion classification model which is based on BiLSTM model

## Dataset

Adapted from [SemEval-2018 Task 1: Affect in Tweets](https://aclanthology.org/S18-1001/)

- Data/2018train.csv: training set from SemEval-2018 Task 1.
- Data/2018train-8.csv: training set aligned with the eight labels of Plutchik’s wheel of emotions.
- Data/newtrain.csv: training set + [NRC emotion lexicon](https://nrc-publications.canada.ca/eng/view/object/?id=0b6a5b58-a656-49d3-ab3e-252050a7a88c)
- Data/newtrain-8.csv: training set + [NRC emotion lexicon](https://nrc-publications.canada.ca/eng/view/object/?id=0b6a5b58-a656-49d3-ab3e-252050a7a88c) aligned with the eight labels of Plutchik’s wheel of emotions.
- Data/2018dev2.csv: dev set from SemEval-2018 Task 1, evaluate the model’s performance.

  ## Emotion model training
Due to the large file size, the embedding file needs to be downloaded from: [glove.840B.300d.txt](https://www.kaggle.com/datasets/takuok/glove840b300dtxt)
