-- Week 4 Assignment --

 --> Title

Azure Cloud Fundamentals and Data Pipeline Implementation using Azure Data Factory

--> Objective

To understand Azure cloud services and implement a complete data pipeline using Azure Blob Storage and Azure Data Factory.

--> Services Used

* Azure Resource Group
* Azure Storage Account
* Azure Blob Storage
* Azure Data Factory
* Azure IAM (Role Based Access Control)

--> Implementation Steps

--> Task 1: Resource Group Creation

Created a Resource Group named RG-DataEngineering in Azure Portal.

--> Task 2: Storage Setup

Created a Storage Account and Blob Container named source-data. Uploaded the file Sample-Superstore.csv.

--> Task 3: Azure Data Factory Setup

Created Azure Data Factory and configured:

* Linked Service to Azure Blob Storage
* Source Dataset (DelimitedText1)
* Destination Dataset (DelimitedText2)

--> Task 4: Pipeline Development

Developed a pipeline named PL_SuperstorePipeline consisting of:

1. Get Metadata Activity
2. Copy Data Activity

Pipeline Flow:
Get Metadata → Copy Data

--> Task 5: Pipeline Execution

Executed the pipeline using Debug mode. Pipeline completed successfully with status "Succeeded".

--> Task 6: IAM Roles

Assigned the following roles:

* Reader
* Contributor
* Storage Blob Data Contributor

ADF Managed Identity was granted access to Blob Storage.

--> Results

* Metadata validation completed successfully.
* Source CSV file was read successfully.
* Data copied from source container to destination location.
* Pipeline executed successfully without errors.

--> Insights

1. Azure Blob Storage provides scalable cloud storage for files.
2. Linked Services are used to connect ADF with external resources.
3. Datasets represent source and destination data structures.
4. Get Metadata activity validates file properties before processing.
5. Copy Data activity enables efficient movement of data between storage locations.
6. IAM roles ensure secure access management for Azure resources.

--> Conclusion

A complete Azure Data Factory pipeline was successfully implemented using Blob Storage as the source. Metadata validation and data copy operations were performed successfully, demonstrating the fundamentals of Azure cloud-based data integration.
