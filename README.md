# Machine Learning, Deployment Case Studies with AWS SageMaker

This repository contains code and associated files for deploying ML models using AWS SageMaker, several tutorial notebooks exists spanning various case studies, code exercises, and project files that will be to illustrate parts of the ML workflow and give enough practice deploying a variety of ML algorithms on Sagemaker.

### Tutorials

* [Population Segmentation](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Population_Segmentation): Learn how to build and deploy unsupervised models in SageMaker. In this example, you'll cluster US Census data; reducing the dimensionality of data using PCA and the clustering the resulting, top components with k-means.
* [Payment Fraud Detection](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Payment_Fraud_Detection): Learn how to build and deploy a supervised, LinearLearner model in SageMaker. You'll tune a model and handle a case of class imbalance to train a model to detect cases of credit card fraud.
* [Deploy a Custom PyTorch Model (Moon Data)](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Moon_Data): Train and deploy a custom PyTorch neural network that classifies "moon" data; binary data distributed in moon-like shapes.
* [Time Series Forecasting](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Time_Series_Forecasting): Learn to analyze time series data and format it for training a [DeepAR](https://docs.aws.amazon.com/sagemaker/latest/dg/deepar.html) algorithm; a forecasting algorithm that utilizes a recurrent neural network. Train a model to predict household energy consumption patterns and evaluate the results.

### Project

[Plagiarism Detector](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Project_Plagiarism_Detection): Build an end-to-end plagiarism classification model. Apply all skills gained from previous learnings to clean data, extract meaningful features, and deploy a plagiarism classifier in SageMaker.

![Examples of dimensionality reduction and time series prediction](./Time_Series_Forecasting/notebook_ims/example_applications.png)

---

## Setup Instructions

These notebooks are intended to be executed on Amazon's SageMaker platform. Follow the instruction below to provision a notebook instance, from which all notebooks can be run.

### Log in to the AWS console and create a notebook instance

Log in to the [AWS console](https://console.aws.amazon.com) and go to the SageMaker dashboard. Click on 'Create notebook instance'.
* The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. 
* For the role, creating a new role works fine. Using the default options is also okay. 
* It's important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or object, with “sagemaker" in the name, is available to the notebook.
* Use the option to **git clone** the project repository into the notebook instance by pasting `https://github.com/iahsanujunda/ml_sagemaker_studies.git`

### Open and run the notebook of your choice

Now that the repository has been cloned into the notebook instance you may navigate to any of the notebooks that you wish to complete or execute and work with them. Additional instructions are contained in their respective notebooks.
