---
layout: post
title: OCR Post-Processing Algorithm Implementation and Evaluation
author: Joey Zhang
post_list: "date"
toc: true
home_btn: true
btn_text: true
footer: true
maximize: true
encrypted_text: true
toc_level: 4
category: Algorithm
date: 2018-11-29
excerpt: "This is excerpt."
---

## Summary

* Implemented an Optical Character Recognition (OCR) post-processing algorithm to enhance Tesseract OCR output by performing both error detection and error correction
* Accomplished Error detection by extracting error features from the output and building an SVM model to predict the location of errors; Corrected the errors by scoring each candidate word using Bayesian combination rule; Conducted performance measure on both word wise and character wise

## About OCR
* OCR is a technology that enables you to convert different types of documents (e.g., scanned documents, PDF files or images captured by a digital camera) into editable and searchable data. An OCR system consists of a pre-processing module, a word recognition module and a post-processing module, which are pipelined together to retrieve a relevant scanned document.

![img-smpl]({{site.url}}{{site.baseurl}}{{site.assets_path}}/img/intro.png)
![img-smpl]({{site.url}}{{site.baseurl}}{{site.assets_path}}/img/ocr_flowchart.png)

## Performance
![img-smpl]({{site.url}}{{site.baseurl}}{{site.assets_path}}/img/PerformancePic.png)

