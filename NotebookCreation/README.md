
# Creating a Notebook Instance

## Configure the Notebook Instance

1. Make sure you are on the AWS Management Console home page.  
In the **Find Services** search box, type **SageMaker**.  The search result list will populate with Amazon SageMaker, which you should now click.  This will bring you to the Amazon SageMaker console homepage.

![Services in Console](./images/console-services.png)

2. In the upper-right corner of the AWS Management Console, confirm you are in the desired AWS region.

3. To create a new notebook instance, click the **Notebook instances** link on the left side, and click the **Create notebook instance** button in the upper right corner of the browser window.

![Notebook Instances](./images/notebook-instances.png)

4. Type smworkshop-[First Name]-[Last Name] into the **Notebook instance name** text box, and select ml.m5.xlarge for the **Notebook instance type**.

![Notebook Settings](./images/notebook-settings.png)

5. Expand the Advanced configuration section, and select the **SageMakerLCCDemo** Lifecycle configuration created earlier.

![Add Lifecycle Configuration](./images/Create-1.png)

6. In the **Permissions and encryption** section
    - select **Enter a custom IAM Role ARN**
    - Paste in the Role ARN that was created earlier, in the Setting up your account section

![Add Role ARN](./images/Create-2.png)

7. Expand out the optional **Git repositories** section. Select the previously created SageMakerCollaboration CodeCommit repository for the Default repository

![Add Repository](./images/Create-3.png)

8. Click **Create notebook instance**. You will be taken to the list of instances, showing your newly created one in the **Pending** state.

![Pending](./images/Create-4.png)

9. Wait for your Instance to be fully created. The status will say **InService**.

![InService](./images/Create-5.png)

10. Click on your Notebook Instances' name, and you will be taken to its settings page

![Settings](./images/Create-6.png)

11. Click on the **View Logs** Link

12. The launch logs will open in a new tab. Have a look at the logs for the LifeCycle hooks

![Logs](./images/Create-7.png)

13. Close the Logs tab in your browser

14. Click the Open Jupyter Lab button, and let the interface open in a new tab. You will see that it opens to your CodeCommit default repository

![JupyterLabs](./images/Create-8.png)

15. Click on the README.md file in the directory browser. Edit the file, add your name or similar, and save the file (ctrl + s) 

![Edit File](./images/Create-9.png)

16. Click the Git icon in the left hand pane. You will see that the README.md file is marked as changed.

![Changed](./images/Create-10.png)

17. Right click the README.md file, and click **Satge**

![Stage](./images/Create-11.png)

18. The file is now ready to be comitted. Enter a commit message and save it.

![Commit](./images/Create-12.png)

19. Finally, push the file using the Push icon. (Cloud and up arrow)

![Push](./images/Create-13.png)

20. Clost the JupyterLab tab, so you are back at the Amazon SageMaker interface.

![Launch Notebook](./images/Create-14.png)

21. Click the **Open Jupyter** button to launch the labs. Click to the root folder so you can see both repositories.

![Home Folder](./images/Create-15.png)

22. Click into the amazon-sagemaker-workshop directory, and you are ready to start the labs


[**Return to the instructions**](../README.md)
