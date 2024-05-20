# End-to-End-Serverless-Data-Analytics-Project
End - End  Serverless data analytics, where you can store and analyze vast amounts of data without having to manage any underlying infrastructure. It leverages AWS services like Glue, Data Catalog, Athena, and QuickSight to streamline the process of data discovery, querying, and visualization.

Here's an explanation of the components involved:


1. AWS IAM (Identity and Access Management): IAM User represents an authenticated user or application that initiates the data analytics process.
2. Amazon S3 (Simple Storage Service): S3 is an object storage service where the raw data or files are stored.
3. AWS Glue: Glue is a fully managed extract, transform, and load (ETL) service. It crawls the data stored in S3, infers the schema, and creates metadata tables in the AWS Data Catalog.
4. AWS Data Catalog: The Data Catalog is a centralized repository that stores metadata about the data sources, data formats, and data schemas. It maintains a unified view of data across different data stores, making it easier to discover and access data for analytics.
5. AWS Athena: Athena is an interactive query service that allows you to analyze data directly from S3 using standard SQL queries. It uses the metadata stored in the Data Catalog to understand the structure of the data and perform queries.
6. AWS QuickSight: QuickSight is a cloud-native business intelligence (BI) service that allows you to create visualizations, dashboards, and reports based on the data queried from Athena or other data sources.

The workflow can be summarized as follows:


1. The IAM User (or an application) uploads raw data or files to Amazon S3.
2. AWS Glue crawls the data stored in S3 and infers the schema, creating metadata tables in the AWS Data Catalog.
3. The AWS Data Catalog stores and maintains the metadata about the data sources, formats, and schemas.
4. AWS Athena uses the metadata from the Data Catalog to query and analyze the data stored in S3 using SQL.
5. The queried data from Athena can be visualized and analyzed further using AWS QuickSight, which creates dashboards and reports based on the data.

