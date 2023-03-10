# TSVM
For Functional Non-coding Variants Prediction using genomic sequence
# Introduction
We propose TSVM to predict context-specific functional NCVs, Which uses a convolutional neural network to extract features and support vector machine to predict functional non-coding variants. First, the convolutional layer was pretrained using large-scale generic functional non-coding variants as sequence feature extractors.  Second, a combination of random forest and support vector machine was used to predict context-specific functional non-coding variants.  
# Requirements
    Python 3.8
    Keras == 2.4.0
    numpy >= 1.15.4
    scipy >= 1.2.1
    scikit-learn >= 0.20.3
# Data
Download the data from https://pan.baidu.com/s/1ZdkaYJWXXdTc8uDiw1JA1Q?pwd=6l6l 
It has Generic dataset and MPRA dataset for pretraining and testing.
# Usage
    python pretrain.py
    The pretrain.py file contains pretain_model. The model was pretrained by a general functional NCVs 
    with the same number of negative variants as positive variants.
    python TSVM.py
    The pretrain.py file contains feature extraction and prediction of context-specific functional NCVs.
# Supported GPUs
    Now it supports GPUs. The code support GPUs and CPUs, it automatically check whether you server install GPU or not, 
    it will proritize using the GPUs if there exist GPUs.
# Contact
Minglie Li: minglie.li@foxmail.com
# Updates
5/3/2023
