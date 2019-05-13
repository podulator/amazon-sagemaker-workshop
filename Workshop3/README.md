# Tensor Flow on Amazon SageMaker

## Modules

This workshop is divided into 2 modules, and you can do them in any order.

You should have already downloaded the repository code locally, and set up an Amazon Sagemaker instance. If you haven't, please see the [**Workshop prerequisites**](../)

- Natural Language Processing Use Case:  Sentiment Analysis

- Bring Your Own Model Use Case:  Containers

## Natural Language Processing Use Case:  Sentiment Analysis

In contrast to the previous modules, which used some of Amazon SageMaker's built-in algorithms, in this module we'll use a deep learning framework within Amazon SageMaker with our own script defining our model, namely TensorFlow.

Please go to the following link for this module:  [**Sentiment Analysis**](../modules/Sentiment_Analysis.md).  

Be sure to use the **downloaded** version of the applicable Jupyter notebook from this workshop repository.  

When you're finished, return here to move on to the next module.  

## Bring Your Own Model Use Case:  Containers

In this module we use Docker to create our own algorithm container, and use it within Amazon SageMaker. This can be essential if you need complex dependencies, or if you want to use a framework that Amazon SageMaker doesn't support directly.

Please go to the following link for this module:  [**Containers**](../modules/Containers.md). 

Be sure to use the **downloaded** version of the applicable Jupyter notebook from this workshop repository.  

When you're finished, return here and go on to the Cleanup Guide.  

## Cleanup

To avoid charges for endpoints and other resources you might not need after the workshop, please refer to the [**Cleanup Guide**](../CleanupGuide).

[**Return to the instructions**](../)