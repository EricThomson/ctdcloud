# Code the Dream Cloud Workspace
A workspace to develop hands-on, accessible cloud computing teaching materials for [Code the Dream](https://codethedream.org/). This informal space is to experiment with lesson plans, identify the most important skills, and create learning paths for Python 200. Student facing-material will be hosted separately at Code the Dream. 

Cloud computing is a massive domain that easily fill an entire year of instruction. In Python 200, we have four weeks, so we try to focus mainly on topics relevant to Python and data engineering pipelines. 

Unlike machine learning and AI workflows, cloud computing is not always about writing code. Much of it involves connecting to infrastructure, understanding available services, and working with GUIs. Therefore, we’ll use MkDocs and Markdown-based guides instead of Jupyter notebooks.

> One challenge of teaching cloud concepts is that the terminology and UI are constantly changing. Be cautious about recording long videos, and be prepared to re-take screenshots -- they're likely to go out of date within a few months. This is just the way of the cloud. :laughing: :cloud:

## Main Workflow
After giving a general introduction to cloud computing, we will provide a hands-on introduction to cloud computing using Azure as the vehicle. The following is a tentative path that will culminate in a full ETL pipeline. 

Our tentative four-week plan that we are building is as follows (for details see the docs):

### Week 1: Hello Cloud
- Focus:  Intro to cloud concepts and working with Azure.

[I'm not sure if we want to include databricks here, but I think this is a good place to include a overview of Databricks/Snowflake vs Azure/AWS even if we are not using databricks/snowflake at all]::

- Hands-on: Students will log into the Azure portal and run Python code via the command line interface. 
- Outcomes: 
  - Understand basic cloud concepts (compute, storage, networking, etc).
  - Navigate the Azure portal.
  - Use the Azure CLI to deploy python modules.

  [Personally, I think we might also want to let students know how to manage files in Azure Blob as part of the training here as many of the tasks in the following weeks might work with files in cloud storage]::

- Materials:
  - Azure official training site: https://learn.microsoft.com/en-us/training/azure/


### Week 2: AI in the Cloud
- Focus: Learn how to spin up cloud compute resources and deploy an AI application.
- Hands-on: Build an interactive AI chatbot using Dash and the Azure OpenAI API, and deploy it to a virtual machine (VM) in Azure.
- Outcomes: 
  - Understand the purpose and usage of cloud-based compute (e.g., virtual machines)
  - Provision and configure an Azure VM.
  - Deploy and serve a Python app (Dash + Azure OpenAI) from a public cloud endpoint.
  - Integrate cloud-based AI (Azure OpenAI) into a real-time web application
- Materials:
  - OpenAI in Azure Foundry Demo: https://azure.microsoft.com/en-us/products/ai-services/openai-service

### Week 3: ML in the Cloud
- Focus: Introduction to cloud-based storage (Blob Storage) in the context of ML workflows.
- Hands-on: Build machine vision application that classifies images using:
  -  A low-code solution with Azure ML Designer.
  -  A code-first approach with the Azure ML SDK.  
- Outcomes: 
  - Understand the structure and role of cloud storage.
  - Upload image data to the cloud and manage input/output formats.
  - Build and deploy an ML model using Azure ML Designer.
  - Run inference using Python and the Azure ML SDK
  - Compare usability, transparency, and cost between low-code and high-code ML pipelines

### Week 4: ETL Pipeline
- Focus: Build ETL pipelines in the cloud using both code-first and low-code tools.  
- Hands-on: Build a complete ETL (Extract, Transform, Load) pipeline in the cloud, comparing two approaches:
  - A low-code solution with Azure Data Factory. 
  - A code-first approach with Prefect.

  [Maybe another example working with PySpark with larger dataset? I think this will really give the students a good example of why we need cloud. But finding proper dataset and managing the cost could be challenging]::

- Outcomes. Work on a team to:
  - Understand the structure and purpose of ETL pipelines in production systems
  - Compare tradeoffs between flexible code-first and scalable low-code approaches
  - Extract data from a public REST API using the requests library
  - Transform and clean the data using pandas
  - Load the data into an Azure PostgreSQL database

  [I'm not sure if it is feasible for the students, but I think many of these cleaning and loading are more commonly done with SQL (with SparkSQL, Duckdb, or something like AWS Athena), so personally I would like to have a bit more emphasis on ETL with SQL than with Pandas. Anecdotally, if something is doable with Pandas, then it is usally doable and easier on local machine rather than on the cloud, and I think this will give the students a bit more chance to practice SQL]::

  - Analyze the results and generate simple insights

  [I think this another place where we might be able to introduce and compare no/low code approach vs code-first visualization, and we might also give some general sense of building dashboards]::

