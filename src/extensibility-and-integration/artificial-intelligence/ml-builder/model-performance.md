---
summary: How to assess performance of your machine learning model, and how to improve it.
tags:
---

# Model performance

What follows is more information about how you can assess you model's performance, and how to improve it.

## Assessing model performance

Once ML Builder successfully trains a model, check the performance of the model. To understand the performance results, you should be familiar with the concepts of:

* **Baseline model** is a very simple model that's quick to generate and ML Builder uses it as **a reference to calculate the performance of the model**.
* **Accuracy** measures the percentage of the correct predictions over the total of predictions. The accuracy score you see in the interface is about the model generated by the ML Builder.


When assessing the model performance, you want that your model **performs better than the baseline model**.

### Methods

For classification problems, ML Builder uses the zero rule algorithm to create the baseline. For regression problems, it calculates the baseline by using the target mean in the train dataset. At the moment, ML Builder uses the accuracy score to analyse the classification model performance; for regression models ML Builder applies Mean Absolute Error (MAE).

## Improving model performance { #improve-model-performance }

AI Builder takes advantage of the automated machine learning process to generate your model. Therefore, most of the work happens behind the scenes. However, there are some things you can do to improve your model performance:

1. Train the model with more good data. More data improves the model performance and lets the automated machine learning process to select the best training methods.

1. Add more attributes to your data. More attributes, or "features" in machine learning language,  increases model performance. Consider using aggregates to join multiple tables before using AI Builder. Be careful when adding new attributes when your data set is small.

1. Try making a better choice of the input attributes. Removing attributes helps reduce noisy and uninformative data from the model, even though models can automatically handle noisy and uninformative attributes if you have enough data. Be careful not to introduce data leak or concept drift (see [Data considerations](data-considerations.md#data-considerations) for more information).

1. Train with more experiments. Having more experiments improves the model, but also increases the time and costs required to generate a model.
