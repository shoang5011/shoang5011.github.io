---
title: "Deep Learning Project: Facial Emotion Recognition"
date: 2019-08-20
tags: [machine learning, data science, deep learning]
header:
  image: "/images/FacialRecognition/cover.jpg"

  excerpt: "Machine Learning, Data Science"

---

# Emotion Detection Using Deep Learning


## Data
The data is from a Kaggle [*data set*](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview). Dimension of each picture is 48x48. There are 28,709 samples in train data, 3,589 samples in test data and 3,589 samples in validation data.
<img src="{{ site.url }}{{ site.baseurl }}/images/FacialRecognition/overview.png" alt="">

Also, distribution of each label in train and validation data is shown below.
<img src="{{ site.url }}{{ site.baseurl }}/images/FacialRecognition/distribution.png" alt="">


## Modeling
Naturally, when it comes to image classification, Convolutional Neural Networks (CNN) are the most popular and powerful in this category. For this project, I start with 3 layers followed by maxpooling layer. More layers will be added to capture more features.
<img src="{{ site.url }}{{ site.baseurl }}/images/FacialRecognition/modeling.png" alt="">
From the above, the model seems to overfit at around 10 epochs, at which accuracy starts to oscillate around certain value. The same happens to loss function.

## Model Validation
Using test data, I can evaluate my trained CNN.
<img src="{{ site.url }}{{ site.baseurl }}/images/FacialRecognition/validation.png" alt="">

The model has an accuracy of 55.61% on validation data, which is comparable to that when used against test data.
<img src="{{ site.url }}{{ site.baseurl }}/images/FacialRecognition/validation2.png" alt="">

Probability of each label predicted by the model is included, together with true label. From the above, the model has hard times predicting some labels, especially between happy and surprise.

## Summary
Even though the model has difficulties in differentiating between some label pairs (neutral-sad, fear-sad, happy-surprise), it is quite understandable even human couldn't do that sometimes (I actually tried to classify some pictures using my own subjective view, and failed quite often).

### Code
Visit my [*GitHub repo*](https://github.com/shoang5011/FacialRecognition-Kaggle) to see the code.
