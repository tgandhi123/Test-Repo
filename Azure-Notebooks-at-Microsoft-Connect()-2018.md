The Azure Notebooks team is excited to share with you our latest update that we announced at Connect() 2018 during Scott Hanselman’s keynote. Here’s what’s new:  
  
# Refreshed Azure Notebooks User Interface 
We have a refreshed user interface at https://notebooks.azure.com; based on your feedback, we’ve improved a number of things in our refreshed user interface: 
  
1. Libraries are now more appropriately named projects. They function just like the libraries you are used to, but we’ve made it easier to create and maintain your content.
  
[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/my_projects.png]]

2. The site now supports notifications that we will use to keep you informed of new features and additions to Azure Notebooks.  

[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/home_page.png]]

3. The site homepage is now more alive with featured and popular content from the Jupyter community.  

[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/home_page_featured_projects.png]]

# Connect Notebooks to your own Azure Compute  
If you are signed into Azure Notebooks with an account associated with an Azure Subscription ([which you can get for FREE with $200 credit](https://azure.microsoft.com/en-us/free/)), then you will enjoy easier and deeper integration with your Azure resources. Besides the free compute that Azure Notebooks provides, users with Azure subscriptions can create Linux Data Science Virtual Machines (DSVMs) and use them to run their notebooks. This is particularly useful if you have computationally expensive workloads, such as training deep learning models using GPUs. 
 
Get started now [provisioning a Linux DSVM](https://azure.microsoft.com/en-us/services/virtual-machines/data-science-virtual-machines/), which comes ready to use with Azure Notebooks. Once you have a DSVM provisioned into your Azure Subscription, ensure that your Azure Notebooks log in account has access to it in the azure portal.  

If you have an account provided by your work or school, Azure Notebooks will discover the DSVMs that you have access to and list them into a menu under the run button. Choose the DSVM that you would like to connect to and enter the user name and password of the Linux account on the DSVM.  

[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/cricket_chirps.png]]


If you have a Microsoft Account (e.g. @outlook.com or @hotmail.com), you can connect to a DSVM directly using its IP address. Choose the Direct Compute option from the Run menu.  

[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/cricket_chirps_2.png]]

### GPU
If you are a Microsoft employee, you will also be able to connect to GPU and provide feedback to the Azure Notebooks team. We are testing GPU support internally and we are excited about enabling this for all our users in the future. If you are not a Microsoft employee, please use the Azure Notebooks support link to let us know about the scenarios and kinds of notebooks that you would want to run on GPUs.  
  
# Just-In-Time Azure Authentication  
 
You can now authorize a project and its notebooks to access Azure resources on your behalf. For example, when accessing your Azure resources using the Azure Python SDK from your notebook, you will now be automatically prompted to allow Azure Notebooks to authenticate the notebook with Azure on your behalf. This avoids having to take additional steps to pre-authenticate.

By clicking on the Grant access button in this dialog, you are making your Azure subscriptions and credentials available to any code running in this Project. Once you have granted access, notebooks can create and access Azure resources on your behalf. For example, you can import data from Azure Storage or export results to Azure Machine Learning Workspaces.

You should, of course, grant access only to Projects that contain code that you trust. 

[[https://github.com/Microsoft/AzureNotebooks/blob/master/wiki_images/jit.png]]

# Azure Notebooks integration with Azure Machine Learning workspaces  
We have integrated the [Azure Machine Learning Service](https://aka.ms/amlfree) with Azure Notebooks by making the Azure Machine Learning SDK available to all code running in the Python 3.6 kernel. This, combined with Azure Subscription support, makes it easy for data scientists to train and optimize machine learning models using the rich set of compute resources available on Azure, and deploy them to Azure for inferencing.   

[Start with the Azure ML Getting Started Project](https://notebooks.azure.com/azureml/projects/azureml-getting-started) to learn more about using Azure Notebooks with the Azure Machine Learning Service. 
 
# Azure Notebooks in the Classroom 
We know that many of you are using Azure Notebooks in classrooms. Based on your feedback we've made it easier for you to be successful with Azure Notebooks, whether you are an instructor or a student.

For instructors, you can use Azure to set up dedicated Data Science Virtual Machines and customize the kernel image to your needs. Use the steps above to connect and use the DSVM from Azure Notebooks. To enable your students to access your DSVMs you will grant them access to the DSVM in Azure Portal and share the username and password for the user account on the DSVM. For students with Microsoft accounts (e.g. @outlook.com) along with the username and password also share the IP address of the machine with them. 

For Students with work and school accounts (e.g. @myschool.edu), you will be able to discover these DSVMs automatically in Azure Notebooks and connect to them, entering the username and password when prompted. 

For Students with MSAs (e.g. @outlook.com) you can use the Direct Connect feature in Azure Notebooks to access the DSVM.  

# Free Compute Package Updates  
Besides the custom compute resources that you can provision in Azure and use with Azure Notebooks, you can still use our free compute for your notebooks, running on our standard image. Based on your feedback we have added new packages to our standard image and we have updated hundreds of other packages to recent versions. For the full list including our latest updates please take a look at the [Azure Notebooks Fall 2018 Package Update](https://github.com/Microsoft/AzureNotebooks/wiki/Azure-Notebooks-Fall-2018-Package-Update).

# Azure Notebooks and Kusto Query Language 
Azure Notebooks now supports KQL, which enables notebooks to query big data stores such as [Azure Log Analytics](https://docs.microsoft.com/en-us/azure/azure-monitor/log-query/get-started-portal) and [Application Insights Analytics](https://docs.microsoft.com/en-us/azure/application-insights/app-insights-analytics). You can get started using the [KQL sample notebooks in GitHub](https://github.com/Microsoft/jupyter-Kqlmagic/tree/master/notebooks).

# Your Feedback Matters! 
* [File an issue](https://github.com/Microsoft/AzureNotebooks/issues/new) for bugs, feature requests, etc. If you need immediate assistance, ping nbhelp@microsoft.com. 
* Azure Notebooks is on [twitter](https://twitter.com/azurenotebooks). Have a cool notebook you want to share? Upload & tweet it with #AzureNotebooks!   

# Links  
* Site: https://notebooks.azure.com   
* Samples https://notebooks.azure.com/microsoft  
* Docs:  https://docs.microsoft.com/azure/notebooks 