# Week 4: ETL Pipeline
In the final week, we bring many different skills together: cloud compute, storage, networking, and databases. Students will build a complete ETL (Extract, Transform, Load) pipeline using two different approaches — low-code and code-first.

### Focus
- Understand how ETL pipelines work in cloud-based production systems
- Build and run pipelines using both graphical and code-based tools
- Compare the flexibility, transparency, and scalability of each approach

### Hands-On Activities
- Extract data from a public REST API using the `requests` library
- Transform and clean data 
- Load the processed data into db
- Compare two approaches to orchestrating the workflow:
  - Low-code: Azure Data Factory
  - Code-first: Python with Prefect
- Show how to pull and analyze stored data

### Learning Outcomes
By the end of this week, students will be able to:

- Explain the purpose and structure of an ETL pipeline
- Extract external data from an API using Python
- Load data into a relational cloud-native database 
- Analyze the final dataset to generate  insights
- Compare tradeoffs between:
  - Azure Data Factory (low-code, scalable, abstracted)
  - Prefect (flexible, Python-native, transparent)

### Resources

- [What is ETL? (Microsoft)](https://learn.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl)
- [Azure Data Factory Overview](https://learn.microsoft.com/en-us/azure/data-factory/introduction)
- [Prefect Docs](https://docs.prefect.io/)


### Instructor Notes
Teamwork is central this week — students will collaborate on designing and deploying a real pipeline.

Consider:
- Assigning different groups to different tools (ADF vs Prefect)
- Reviewing how to monitor and troubleshoot pipelines in both environments
- Prompting class discussion on the long-term maintainability of low-code vs code-first solutions


