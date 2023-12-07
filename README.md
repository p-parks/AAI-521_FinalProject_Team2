# AAI-521 Final Project Team 2

Team Members:
- Paul Parks
- Bin Lu
- Eyoha Girma
- Jeremy Cryer

## Overview

Create AI model to detect ASL gestures.

## Dataset

The dataset chosen is the Google - Isolated Sign Language Recognition: 
- https://www.kaggle.com/competitions/asl-signs/overview

The dataset contains .parquet files which were generated from mediapipe. Each file contains the mediapipe landmark information for an ASL sign. There are a total of 250 unique signs and the dataset is 52 gigabytes. 

## EDA

Our group conducted individual EDA and generated ideas on what types of models would be application for detecting sign language from a media pipe video file. 

All EDA can be found in `./EDA/`

## Model

Several iterations on models were performed throughout the course. The two different models and approaches can be found in their respective folders. 

### LSTM 

The LSTM model is located in `./LSTM/`. We attemped to improve performance by removing low performing signs and generated 3 different models which can be found in the directory.

### Transformer

The Transformer model has significantly better performance and can be found in `./Transformer/`

## Inference

We are providing two notebooks that can be used for Inference. 

`./Inference_Colab.ipynb` can be ran in Google Colab and will access you webcam to run the models. Note: We have found very bad performance while attempting to detecting the sign language from within Google Colab. This is why we have created the second inference notebook.

`./Inference_Local.ipynb` can be ran on you local machine and will use opencv to access the webcam. 