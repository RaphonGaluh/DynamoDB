# Creating, Importing, Querying, and Exporting Data with Amazon DynamoDB
Raphon Galuh C | 21110034 | S1-SD02A

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
- Before anything else, I suggest uploading your CSV into s3 first. so you just need to browse it.
  <img width="665" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/0850a54e-a76b-4754-8c95-6ab2710b913e">
- Choose the format based on the file you uploaded, and adjust as necessary.
  <img width="636" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/b37f7928-3286-4b81-afd2-5f155753deb3">
- After that, fill in the table details, by inputting your table name and its primary key. *I change the file name to 'Catering_KostReika'.
  <img width="641" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/9be08478-4755-418a-94fe-f6e4dacaa30c">
- In the table setting, I choose the default setting.

   <img width="630" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/5cb64097-f212-4ec3-8fc8-b92985d65794">
- Then on the review and import page, when you see that all the data is in accordance with what you wish for, click 'import'.
  <img width="605" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/00015168-93bd-46df-aa79-fb373f53e3a3">
- It will take the file for a while to import, as can be seen in the status.
  <img width="685" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/9e38f3b6-9b48-443a-a09f-7c6b940296dc">
- We will wait until we have a green 'Completed' status beside the imported data.
  <img width="704" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/dd538bf1-094d-41c0-a1c1-3605af0c0a5e">
- When the file finished importing, we can see it by going back to the DynamoDB menu > Tables > Click our table > explore table item.
  <img width="666" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/ec49680c-0635-4769-88ef-60992d65412c">
- This is the table that we just imported.

   <img width="436" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/b1112308-da04-4076-ba18-c707c8ed90e4">
  
## Step 3: Performing Queries or Scans with Filters
# Scan Data
- Click on Explore Item and scan. You can explore this function yourself.

  <img width="451" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/2735a0b8-1e41-4fe4-ac1a-ab973e4d22fa">
- Scan result.

  <img width="434" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/ab87c777-fba8-4aaa-8696-da2770667f12">
# Query Data
- Click the query options on the same page as the last one. And explore the function ourselves.
  <img width="445" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/d6de09a3-650b-4bc9-9cbb-e3221b90f280">
- Query Result

  <img width="435" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/43f8d30f-ad76-42d1-9538-57b36decc03d">


## Step 4: Exporting Results from DynamoDB
- The last step is to export the data. First, we need to go to DynamoDB > Export to S3.
  <img width="684" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/f5ca1c0c-c114-4e31-a512-4ff9db083622">
- Input your source table, and the destination bucket that you want to export it into >  Export.
  <img width="674" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/2b1ad37f-7e40-401d-ac7f-e88c506a1b7d">
- It will take the file a while to be exported, as can be seen in the status.
  <img width="663" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/e0045df4-e9b0-4269-b4d0-7aae070c821f">
- We will wait until we have a green 'Completed' status beside the exported data.
  <img width="640" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/984b711c-d67c-475c-b065-5cfd14eff0b2">
- Then we will go to S3 > our bucket that we export our data in > and we will see our exported data as 'AWSDynamoDB/'.
  <img width="666" alt="image" src="https://github.com/RaphonGaluh/DynamoDB/assets/122784852/3210c8d9-eaf6-4d89-ad55-34247ac2864e">



## Conclusion
In conclusion, DynamoDB functions provide powerful capabilities to manipulate and transform data within Amazon DynamoDB. These functions enable you to create custom expressions and logic for various DynamoDB operations, such as filtering, updating, and transforming data.

In this documentation, we explored the process of creating, importing, querying, and exporting data with Amazon DynamoDB. We covered the steps to create a DynamoDB table, import data from CSV files, perform queries and scans with filters, and export results using DynamoDB Data Pipeline and DynamoDB Streams. By following this documentation, you gained the knowledge to utilize DynamoDB effectively for building scalable and high-performance applications.

## References
- Amazon DynamoDB Documentation
- AWS DynamoDB Developer Guide
- AWS DynamoDB Best Practices
- AWS DynamoDB API Reference

## Thank You, I hope you can find this helpful <3
