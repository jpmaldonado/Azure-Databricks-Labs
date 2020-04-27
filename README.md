# Project Description

**Azure Databricks** is an Apache Spark-based big data analytics and machine learning framework optimized for the Microsoft Azure Cloud.
Databricks is integrated with Azure to provide one-click setup, streamlined workflows, and an interactive workspace that enables collaboration between data scientists, data engineers, and business analysts.

This repository consists of seven labs that are designed to help you to understand how to use Azure Databricks for different use cases, including:

* Analysis of structured and unstructured data.
* Analysis of streaming data.
* Machine Learning (ML) and Machine Learning Operations (MLOPs)

The seven labs are implemented as seven independent Azure Databricks notebooks as described below.

#### Lab-01_Data Engineering

This tutorial helps you understand how to use Azure Databricks Spark to prepare raw data for analytics.

#### Lab-02_SparkSQL & Performance Optimization

This tutorial help you to understand the capabilities and features of **Spark SQL** and the various performance options provided by Azure Databricks.

#### Lab-03_Machine Learning

This tutorial helps you understand the capabilities and features of **Azure Spark MLlib** for machine learning. It shows how to construct the end-to-end process for building and refining a machine learning model.
	
#### Lab-04_Real-time Stream Analytics
		
This tutorial helps you understand Azure Databricks **Spark Structured Streaming**. It shows the end-to-end process starting with data ingestion into a Azure Databricks cluster in near real-time, through analysis of the the streaming data and integration with machine learning.

#### Lab-05_Databricks Delta
	 
This tutorial is helps you understand the features and capabilities of **Azure Databricks Delta**. Azure Databricks Delta is a next-generation unified analytics engine built on Apache Spark™. It provides ACID transactions, optimized layouts and indexes to enable big data use cases, from batch and streaming ingests, fast interactive queries to machine learning.
		
#### Lab-06_Data orchestration using Azure Data Factory
	
This tutorial helps you understand how **Azure Data Factory** (ADF) can be used with Azure Databricks, to create and automate piplines.

#### Lab-07_MLOps with Azure Databricks

This tutorial helps you understand how to use the MLOps approach to automate machine learning with Azure Databricks. MLOps is a practice for collaboration and communication between data scientists and operations professionals to help manage production ML (or deep learning) lifecycle. MLOps in Azure provided through the integration of two Azure Services:
1) Azure Machine Learning Service (Azure ML Service)
2) Azure DevOps

# Getting Started

Follow these instruction to download the Azure Databricks lab notebooks from this reposiory and import them into Azure Databricks.

## Step 1: Create an Azure Databricks workspace using the Azure portal


1.In the Azure portal, select Create a resource > Data + Analytics > Azure Databricks.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image1.jpg)

2.Under Azure Databricks Service, provide the values to create a Azure Databricks workspace.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image2.jpg)

3.Provide the following values:

a. Workspace name	: A name for your Azure Databricks workspace

b. Subscription	:	From the drop-down, select your Azure subscription.

c. Resource group	:  Specify whether you want to create a new resource group or use an existing one. A resource group is a container that holds related resources for an Azure solution. For more information, see Azure Resource Group overview.

d. Location	:  Specify the location of your Azure Databricks cluster.

e. Pricing Tier	:  Choose between Standard or Premium.

You can choose the *Select Pin to Dashboard* option to pin the resource to the Azure Dashboard

**Then click Create**

4.The workspace creation takes a few minutes. During workspace creation, the portal displays *"Submitting deployment for Azure Databricks"* tile on the right side. You may need to scroll right on your dashboard to see the tile. There is also a progress bar displayed near the top of the screen. You can watch either area for progress.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image3.png)


5.In the Azure portal, go to the Azure Databricks workspace that you created, and then click **Launch Workspace**.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image4.jpg) 

6.You are now inside your Databricks workspace.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image5.jpg)


## Step 2: Download the labs from the Bitbucket repository.

1.Go to Download tab and click on Download Repository.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image6.jpg)

2.The downloaded file is in the zip format.

3.If you extract the ZIP file, you will see the different lab notebooks. All the notebooks are of type .dbc, which stands for Databricks Archive.

## Step 3: Import the Notebooks into the Azure Databricks Workspace.

1.Click the Workspace button![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/workspace.png) or the Home button ![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/Home.png) in the sidebar. Select Import as shown in the screenshot. Alternatively, next to any folder, click the right side of the text and select Import.

![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image7.jpg)

3.Browse to the location of your lab DBC file, and click import.

![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image8.jpg)


## Step 4: Creating a Databricks Cluster

In Databricks you can create two different types of clusters:

1.**Standard** : Standard clusters are the default and can be used with Python, R, Scala, and SQL. 

2.**High Concurrency** : High-concurrency clusters are tuned to provide the efficient resource utilization, isolation, security, and the best performance for sharing by multiple concurrently active users.

We'll be using a Standard cluster for our Labs.

1.Click the clusters icon ![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/clusters.png) in the sidebar.

2.Click the Create Cluster button at the top of the page.


![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image9.jpg)


3.Click the Create button. The cluster list page shows the status of the new cluster.

a. On the Create Cluster page, specify the cluster name QS.

b. select 5.2 (Scala 2.11, Spark 2.4.0) in the Databricks Runtime Version drop-down.
		
		
![GitHub Logo](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image10.jpg)	
		
c.Click Create Cluster 

## Step 6: Attach the Notebook to your cluster.

1. Go to the Databricks WorkSpace

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image11.jpg)

2. Go to your specific notebook in the workspace.

![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image12.jpg)

3. Click on `detached` written on the top-left corner, and you'll see a list of active clusters.

4. Attach your notebook to a running cluster. A green icon shall appear on top, meaning our notebook is now attached to our cluster and is ready to be executed.
![deploy](https://github.com/snapanalytx/AzureDBLabs/blob/master/images/image13.jpg)

### Your Databricks Environment is now setup and you can proceed with the labs.
