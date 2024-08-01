---
title: Machine Learning Techniques in Galaxy Classification
summary: '
This project aims to classify galaxies based on their morphologies using advanced machine learning techniques.
'

tags:
  - Unsupervised Learning
  - Cluster Algorithm

show_date: false

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Andromeda Galaxy (M31). photo: Zhuan Li
  focal_point: Smart

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

## Introduction
Galaxies, the vast and sprawling structures that dominate our universe, come in an array of intriguing shapes and sizes. Understanding these shapes not only deepens our knowledge of the cosmos but also provides insights into the evolution of galaxies. In this portfolio project, I leveraged advanced machine learning methods to classify galaxies based on their shapes, utilizing several powerful techniques to enhance both accuracy and efficiency.

## Utilizing Deep Learning with ResNet18
To tackle the complex task of galaxy classification, I began by employing a pre-trained convolutional neural network (CNN), specifically ResNet18. CNNs are particularly adept at processing visual information and learning hierarchical patterns, making them ideal for image classification tasks like this one. ResNet18, known for its deep residual learning framework, helps in avoiding the problem of vanishing gradients—a common issue in training deep networks.
In this project, I modified ResNet18 by removing its final layer. This alteration transforms the network into a feature extractor, where the input—images of galaxies—yields vectors containing salient features of each image rather than a class label. These feature vectors are critical for the subsequent clustering step.

## Clustering with K-means and Spectral Methods
With feature vectors in hand, I applied two clustering methods: K-means and Spectral clustering. K-means, a centroid-based clustering, partitions the vectors into clusters, with each belonging to the nearest mean. Meanwhile, Spectral clustering uses similarity between examples as a basis for clustering, which is particularly useful for grouping data that is not linearly separable.

## Semi-Supervised Learning Enhancement
To enhance the performance of the clustering, I introduced a semi-supervised learning component. By manually labeling a small subset of the galaxy images, I was able to retrain the ResNet18 network. This step helps the model learn more specific features relevant to galaxy shapes, thus improving the clustering accuracy in subsequent iterations.

