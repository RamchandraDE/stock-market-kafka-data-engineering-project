# stock-market-kafka-data-engineering-project


## Introduction 
In this project, you will carry out an end-to-end data engineering project on real-time stock market data using Kafka.

We will use a variety of technologies, including Python, Amazon Web Services (AWS), Apache Kafka, Glue, Athena, and SQL.

## Architecture 
<img src="Architecture.jpg">

## Technology Used
- Programming Language - Python
- Amazon Web Service (AWS)
1. S3 (Simple Storage Service)
2. Athena
3. Glue Crawler
4. Glue Catalog
5. EC2
- Apache Kafka

# Data Collection: 
- started by collecting stock market data in CSV file format using Python. This data represents real-time stock market events and activities.
# Data Streaming with Kafka:
-Next,set up Apache Kafka on your EC2 machine. Kafka acts as a message broker, allowing you to publish (produce) stock market events to topics. You wrote a producer code that reads the CSV data and publishes these events to Kafka topics.
# Data Consumption with Kafka Consumer: 
-Then, wrote a consumer code to consume (read) these stock market events from Kafka. The consumer processes these events and performs actions such as storing them or further analysis.
# Data Storage on Amazon S3: 
- Decided to store the consumed stock market data on Amazon S3, a scalable storage service provided by Amazon Web -Services (AWS). This allows for efficient and durable storage of large volumes of data.
# Data Cataloging with AWS Glue: 
-To make querying and analysis easier, used AWS Glue, a fully managed extract, transform, and load (ETL) service. ran a Glue crawler, which automatically analyzes the data stored in Amazon S3, infers the schema, and builds a metadata catalog (Glue Data Catalog).
#Data Querying with Athena: 
-With the Glue Data Catalog in place, can now query the stock market data directly using Amazon Athena, an interactive query service that makes it easy to analyze data in Amazon S3 using SQL. Athena seamlessly integrates with the Glue Data Catalog, allowing you to query data without the need for complex ETL processes.


## Dataset Used
You can use any dataset, we are mainly interested in operation side of Data Engineering.

