---
title: Credit Card Fraud Detection Using Machine Learning
summary: 'In this project, I tackled the challenge of credit card fraud detection, an issue that affects financial institutions and consumers worldwide. The objective was to develop a robust machine learning system capable of identifying fraudulent transactions effectively. To to that, I employed three distinct models: logistic regression, random forest, and shallow neural networks. Each model was chosen for its unique strengths in handling binary classification problems and its potential to perform well on imbalanced datasets.'

tags:
  - Supervised Learning
  - Logestic Regression
  - Random Forest
  - Neural Network

show_date: false

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
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





## Data Preprocessing
One of the major challenge in fraud detection is the highly imbalanced nature of the datasets, where fraudulent transactions are much rarer than legitimate ones. This imbalance can bias the model towards predicting the majority class, leading to high accuracy but poor recall for fraudulent transactions. To counteract this, I implemented an undersampling strategy, reducing the size of the majority class (legitimate transactions) to balance the dataset. This approach helps in enhancing the sensitivity of the models to fraudulent activities by giving equal importance to both classes during training.

## Logistic Regression Model
The first model I employed was logistic regression, a linear model that is particularly useful for binary classification tasks due to its simplicity and efficiency in producing probability-based outputs. Logistic regression was trained using a combination of features extracted from the transaction data, including amount, time, and previously known fraud indicators. The model was optimized using techniques such as feature scaling and regularization to prevent overfitting and to improve its generalization capabilities on unseen data.

## Random Forest Model
Next, I utilized a random forest model, which operates by constructing a multitude of decision trees during training and outputting the class that is the mode of the classes of the individual trees. This ensemble method is well-suited for handling complex datasets with a mixture of numerical and categorical data. The random forest model was particularly advantageous due to its ability to handle overfitting better than many other algorithms and its intrinsic feature selection capabilities, providing insights into which features most significantly impact the prediction of fraudulent transactions.

## Shallow Neural Network
The third model explored was a shallow neural network, comprising a few layers to keep the computation manageable while still capturing nonlinear relationships in the data. The network included input, hidden, and output layers with activation functions tailored to enhance model performance on the classification task. Training involved backpropagation and optimization techniques such as stochastic gradient descent to iteratively adjust the weights of the network, aiming to minimize prediction errors.

## Model Performance Evaluation
To evaluate the effectiveness of each model, I focused on the confusion matrix and the F1 score as the primary metrics. The confusion matrix provided a detailed breakdown of the models' performance, distinguishing between true positives, false positives, true negatives, and false negatives. The F1 score was particularly crucial as it balances the precision and recall of the model, providing a more holistic view of model performance especially in the context of an imbalanced dataset. This metric was instrumental in identifying the best-performing model under real-world conditions, where the cost of misclassifying fraudulent transactions can be substantial.