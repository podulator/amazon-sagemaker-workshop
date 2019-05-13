# Introduction to Amazon SageMaker

In this workshop, we'll work though several examples that demonstrate Amazon SageMaker's core components including notebook instances, hosted training, and hosted model endpoints.  Examples are divided into modules.  The examples that involve training machine learning models show how Amazon SageMaker can be applied in three fundamental categories of machine learning:  working with structured data, computer vision, and natural language processing.  

We'll also make use of some of Amazon SageMaker's built-in algorithms, specifically an AWS-optimized version of XGBoost and a deep learning-based image classification algorithm.  Built-in algorithms enable you to avoid spending time against algorithm/neural net design, provide conveniences such as reduced need for model tuning, and are meant to handle the scalability and reliability issues that arise when working with large datasets.  As a contrast, in one module we'll use a script defining our own deep learning model rather than a built-in algorithm.  Whether using your own models or built-in algorithms, all of Amazon SageMaker's features may be used in a similar way.  

To summarize, here are some of the key components and features of Amazon SageMaker demonstrated in this workshop:

- Using **Notebook Instances** for Exploratory Data Analysis and prototyping.
- **Local Mode Training** to confirm your code is working before moving on to full scale model training.
- **Hosted Training** for large scale model training.
- **Built-in algorithms** designed for web scale and kickstarting data science projects.
- **Script Mode**, which enables you to use your own model definitions and scripts similar to those outside SageMaker, with prebuilt machine learning containers.
- **Hosted Endpoints** for near real-time predictions.
- [**Batch Transform**](https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works-batch.html) for asynchronous, large scale batch inference.

## Modules

This workshop is divided into multiple modules, and you can do them in any order.

You should have already downloaded the repository code locally, and set up an Amazon Sagemaker instance. If you haven't, please see the [**Workshop prerequisites**](../)


- Structured Data Use Case:  Videogame Sales 

- Computer Vision Use Case:  Image Classification  

- Natural Language Processing Use Case:  Sentiment Analysis

## Structured Data Use Case:  Videogame Sales

In this module, we'll use Amazon SageMaker's built-in version of XGBoost to make predictions based on structured data related to the videogame industry.  Please go to the following link for this module:  [**Videogame Sales**](../modules/Video_Game_Sales.md).  Be sure to use the **downloaded** version of the applicable Jupyter notebook from this workshop repository.  

When you're finished, return here to move on to the next module.  


## Computer Vision Use Case:  Image Classification

This module uses Amazon SageMaker's built-in Image Classification algorithm.  Please go to the following link for this module:  [**Image Classification with Transfer Learning**](../modules/Image_Classification_Transfer_Learning.md).  Be sure to use the **downloaded** version of the applicable Jupyter notebook from this workshop repository.  

When you're finished, return here to move on to the next module.  


## Natural Language Processing Use Case:  Sentiment Analysis  

In contrast to the previous modules, which used some of Amazon SageMaker's built-in algorithms, in this module we'll use a deep learning framework within Amazon SageMaker with our own script defining our model.  Please go to the following link for this module:  [**Sentiment Analysis**](../modules/Sentiment_Analysis.md).  Be sure to use the **downloaded** version of the applicable Jupyter notebook from this workshop repository.  

When you're finished, return here and go on to the Cleanup Guide.  


## Cleanup

To avoid charges for endpoints and other resources you might not need after the workshop, please refer to the [**Cleanup Guide**](../CleanupGuide).

[**Return to the instructions**](../)