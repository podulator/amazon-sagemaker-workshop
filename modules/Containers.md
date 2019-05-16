## Containers

In this module, we'll create our own deep learning container for Amazon SageMaker. Ones already exist for TensorFlow, MXNet, PyTorch, and Chainer, but sometimes you need extra dependencies (in this case we add OpenCV Computer Vision libraries), or a different framework altogether, and this will show you how to use Amazon SageMakwer in a modular way. We will create a single image that is used for both training and hosting the model.

1. Be sure you have downloaded this GitHub repository as specified in **Preliminaries** before you start.  Next, in your notebook instance, click the **New** button on the right and select **Folder**.

2. Click the checkbox next to your new folder, click the **Rename** button above in the menu bar, and give the folder a name such as 'containers'.

3. Click the folder to enter it.

4. To upload the notebook, click the **Upload** button on the right. Then in the file selection popup, select the file 'tf-byom.ipynb' from the notebooks subdirectory in the folder on your computer where you downloaded this GitHub repository. Click the blue **Upload** button that appears to the right of the notebook's file name.

5. You are now ready to begin the notebook:  click the notebook's file name to open it, then follow the directions in the notebook.


<p><strong>NOTE:  training the model for this example typically takes about 5 minutes.</strong></p>

[**Return to the workshop**](../Workshop3)