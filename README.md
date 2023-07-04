# Creating, Importing, Querying, and Exporting Data with Amazon DynamoDB

## Introduction
- Provide an overview of Amazon DynamoDB and its key features.

## What is DynamoDB
Amazon DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). It is designed to deliver fast and predictable performance at any scale. DynamoDB offers a flexible schema-less data model, allowing you to store and retrieve data using simple key-value or document-based operations.

## Prerequisites
- List the prerequisites required to follow the steps in the documentation, such as an AWS account and access to the AWS Management Console.

## Step 1: Creating a DynamoDB Table
- Creating a DynamoDB table:
![Screenshot (4)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/e5609f8e-6f17-48e7-9416-255d95d2aec8)
- In Table, click 'Create table'.
![Screenshot (6)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/6b57f4b2-699d-4502-b6c9-9323d8c1f612)
- In Table detail, input table name, partition key, and sort key.
![Screenshot (8)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/2e69e0f5-9359-4566-8a25-df1b4acb46b7)
- Then click 'Create Table'.
![Screenshot (9)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/5a329722-3e1c-45f2-b041-1156743d40ee)
- The table will appear in the DynamoDB tables list. Wait a short while for the status table to change to active if it is initially still developing.
![Screenshot (10)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/caef8a40-350f-4f3d-99d9-b0fc2090cf65)
- Go to Explore items: your-table-name, select 'Create item'.
![Screenshot (11)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/211f5133-654f-4999-a131-8fecb1b6a169)
- Enter the value for the table attribute, and then select "Create item" to add data to the table.
![Screenshot (12)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/d70af7a0-f13e-4d86-a125-436702e49500)
- It will be displayed like this.
![Screenshot (13)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/54df7aa0-5292-4467-b6e4-d1bfdea4d62d)

## Step 2: Importing Data from a CSV File
- Select DynamoDB from the menu, click Import from S3, and then select "Import from S3" to import datasets from an S3 bucket.
![Screenshot (14)](https://github.com/RaphonGaluh/DynamoDB/assets/122784852/1bb966dd-e4b0-40cc-a0f8-0ed4f2bd74aa)
- 

## Step 3: Performing Queries or Scans with Filters
- Explain the concepts of querying and scanning in DynamoDB.
- Guide the reader through the process of performing queries or scans with filters:
  - Discuss the Scan operation and its limitations.
  - Introduce the Query operation and its benefits.
  - Provide examples of filtering data using the primary key attributes.
  - Demonstrate the use of global secondary indexes (GSIs) for more advanced querying.

## Step 4: Exporting Results from DynamoDB
- Explain the options available for exporting data from DynamoDB.
- Guide the reader through the chosen method to export results:
  - Describe DynamoDB Data Pipeline and its capabilities.
  - Discuss DynamoDB Streams and its integration with AWS Lambda for processing and exporting data.
  - Demonstrate the configuration and setup required for the chosen method.

## Conclusion
- Recap the key steps covered in the documentation.
- Highlight the importance of understanding DynamoDB's data model and best practices.
- Encourage further exploration of DynamoDB's features and capabilities.

## References
- Include a list of references or links to relevant AWS documentation and other resources used in the documentation.
