---
layout: post
title: Image Super-Resolution
author: Joey Zhang
post_list: "date"
toc: true
home_btn: true
btn_text: true
footer: true
maximize: true
encrypted_text: true
toc_level: 4
category: Machine Learning
date: 2018-11-07
excerpt: "This is excerpt."
---

## Summary
* Contributed to three classification engines to enhance the resolution of images; Trained with 1500 pairs of images and tested with 1000 low-resolution images
* Implemented GBM, Xgboost, and Neural Network model, and tuned the model parameters by cross-validation; Performed image prediction, and carried out both model evaluation and selection by comparing PSNR

## About Super-Resolution


## Project Details
* In this project, we created a classification engine for enhance the resolution of images. We have achieved three things in this project:

	1. Implemented the current practice as the baseline model.
	2. Implemented an improvement to the current practice. In this part, we chose two different models as improvements: Xgboost and Neural Network.
	3. Evaluated the performance gain of our proposed improvement against the baseline.

* Specifically, in feature selection part, we implemented Laplace transformation to training pictures, in order to find the most representaive points in each picture and sampled them as our training data points. Then after building models using training data, through cross validation for each model (mentioned above), we got the best parameters for each model according to the cross validation error, then implemented each model with their best parameters on testing pictures. Finally, according to the PSNR value of each model, we decided which model is the best model in super resolution problem.
