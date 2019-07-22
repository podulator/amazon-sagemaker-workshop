## Advanced Image Classification With Automatic Tuning 


For this module, we'll work with an image classification example notebook. In particular, we'll use Amazon SageMaker's built-in image classification algorithm, which is a supervised learning algorithm that takes an image as input and classifies it into one of multiple output categories. 

It uses a convolutional neural network (ResNet)for the training, but this time we use auto tuning to improve the prediction accuracy. Finally, we deploy the model using a smaller instance with Elastic Inference attached to it, to optiise for cost.

Follow these steps:

1. Go to your Jupyter notebooks homepage 

2. Click into the folder called `amazon-sagemaker-workshop`

3. Click into the folder called `notebooks`

4. Click on the notebook called `advanced-image-classification.ipynb`, then follow the directions in the notebook.

<p><strong>NOTE:  training the model for this example typically takes about 30 minutes.</strong> However, keep in mind that this is due to a soft limit on the number of machine instances that an AWS account starts with, for your own protection. If you desired, you could raise this limit and launch 10 instances at the same time, and the total billable time would be the same.</p>

[**Return to the workshop**](../Workshop2/README.md)