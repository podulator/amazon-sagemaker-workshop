# Amazon SageMaker Workshops

Amazon SageMaker is a fully managed service that enables developers and data scientists to quickly and easily build, train, and deploy machine learning models at any scale. This repository contains a collection of workshops and other hands on content that will guide you through using the many features of Amazon SageMaker.  

![Overview](./images/overview.png)

You'll start by creating an Amazon SageMaker notebook instance with the requisite permissions. Depending on the workshop, you will then interact with Amazon SageMaker via sample Jupyter notebooks, the AWS CLI, the Amazon SageMaker console, or all three. 

**BEFORE attempting any of the workshops, please review the Prerequisites below and complete any actions that are required.**

## Prerequisites

### AWS Account

**Permissions**: In order to complete this workshop you'll need an AWS Account, and an AWS IAM user in that account with at least full permissions to the following AWS services: 

- AWS IAM
- Amazon S3
- Amazon SageMaker
- Amazon EC2:  including P3, C5, and M5 instance types; to check your limits, see [Viewing Your Current Limits](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html)

**Use Your Own Account**: The code and instructions in this workshop assume only one participant is using a given AWS account at a time. If you try sharing an account with another person, you'll run into naming conflicts for certain resources. You can work around these by appending a unique suffix to the resources that fail to create due to conflicts, but the instructions do not provide details on the changes required to make this work. Use a personal account or create a new AWS account for this workshop rather than using an organization’s account to ensure you have full access to the necessary services and to ensure you do not leave behind any resources from the workshop.

**Costs**: Some, but NOT all, of the resources you will launch as part of this workshop are eligible for the AWS free tier if your account is less than 12 months old. See the [AWS Free Tier page](https://aws.amazon.com/free/) for more details. An example of a resource that is **not** covered by the free tier is the Amazon SageMaker notebook instance type used in some workshops. To avoid charges for endpoints and other resources you might not need after you've finished a workshop, please refer to the [**Cleanup Guide**](./CleanupGuide). 


### AWS Region

Amazon SageMaker is not available in all AWS Regions at this time.  Accordingly, we recommend running this workshop in one of the following supported AWS Regions:  N. Virginia, Oregon, Ohio, Frankfurt or Ireland.

Once you've chosen a region, you should create all of the resources for this workshop there, including a new Amazon S3 bucket and a new SageMaker notebook instance. 
Make sure you select your region from the dropdown in the upper right corner of the AWS Console before getting started.

![Region selection screenshot](./images/region-selection.png)


### Browser

We recommend you use the latest version of Chrome or Firefox to complete this workshop.

## Jupyter Notebooks

If you are new to using Jupyter notebooks, please read the next section, otherwise you may now skip ahead to the workshop links.

<details>
<summary><strong>An introduction to Jupyter notebooks</strong></summary><p>

Jupyter is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more. With respect to code, it can be thought of as a web-based IDE that executes code on the server it is running on instead of locally. 

There are two main types of "cells" in a notebook:  code cells, and "markdown" cells with explanatory text. You will be running the code cells.  These are distinguished by having "In" next to them in the left margin next to the cell, and a greyish background.  Markdown cells lack "In" and have a white background. In the screenshot below, the upper cell is a markdown cell, while the lower cell is a code cell:

![Cells](./images/cells.png)

To run a code cell, simply click in it, then either click the **Run Cell** button in the notebook's toolbar, or use Control+Enter from your computer's keyboard. It may take a few seconds to a few minutes for a code cell to run. You can determine whether a cell is running by examining the `In[]:` indicator in the left margin next to each cell:  a cell will show `In [*]:` when running, and `In [a number]:` when complete.

Please run each code cell in order, and **only once**, to avoid repeated operations.  For example, running the same training job cell twice might create two training jobs, possibly exceeding your service limits.
</p></details>


## Workshops

- **Preliminaries**

    - **Create a notebook instance**
        - SageMaker provides hosted Jupyter notebooks that require no setup, so you can begin processing your training data sets immediately. With a few clicks in the SageMaker console, you can create a fully managed notebook instance, pre-loaded with useful libraries for machine learning. You need only add your data.

        - To create a SageMaker notebook instance for this workshop, follow the instructions at [**Creating a Notebook Instance**](./NotebookCreation), then return here to continue with the next step.

    - **Download this repository to your computer**
        - Return to the home page of this GitHub repository or open it in another tab;
        - Click the green **Clone or download** button from the upper right of the main page of the repository, then **Download ZIP**.
        - Use the downloaded notebooks in the notebooks directory rather than other versions you might find inside your notebook instance or elsewhere; the downloaded versions are modified for use in workshops.  

- **Workshop 1 : Introduction to Amazon SageMaker**
    - [**Introduction to Amazon SageMaker**](Workshop1) - This workshop demonstrates some of the key features of Amazon SageMaker.  
    It does so via a set of examples for common prediction use cases, customer churn and product success, using the provided XgBoost algorithm. It will give an intro into working with and preparing data sets, as well as doing ad hoc visualisations in a Jupyter Notebook.

- **Workshop 2 : Image recognition with Amazon SageMaker**
    - [**Image recognition with Amazon SageMaker**](Workshop2) - This workshop uses image recognitiom / computer vision as a way to dive into transfer learning, pre-made off the shelf algorithms, using Elastic Inference to reduce costs, and hyper paramater optimisation auto tuning to get better results.

- **Workshop 3 : Tensor Flow on Amazon SageMaker**
    - [**Tensor Flow on Amazon SageMaker**](Workshop3) -  This workshop focusses on the TensorFlow framework on Amazon SageMaker. We'll be looking at Natural Language Processing via Sentiment Analysis, as well as looking at bringing your own model to Amazon SageMaker, using the service in a modular way, batch transform jobs


## License & Contributing

The contents of this workshop are licensed under the [Apache 2.0 License](./LICENSE). 
If you are interested in contributing to this project, please see the [Contributing Guidelines](./contributing/CONTRIBUTING.md).  In connection with contributing, also review the [Code of Conduct](./contributing/CODE_OF_CONDUCT.md).


