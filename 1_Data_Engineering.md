# Domain 1.1: Create data repositories for machine learning


### Terminology
* **Data Lake** - 
* **Data Mesh** - 
* **Data Warehouse** - 
* **Elastic** - varies depending on needs
* **File storage** vs **[Block Storage](https://aws.amazon.com/what-is/block-storage/)**

#### Services mentioned

* [AWS Lake Formation](https://aws.amazon.com/lake-formation/) - security & governance
* [AWS S3](https://aws.amazon.com/s3/)
* [Amazon EFS](https://aws.amazon.com/efs/)
* [Amazon EBS](https://aws.amazon.com/ebs/)
* [Amazon FSx](https://aws.amazon.com/fsx/)


## AWS S3 Storage Classes
Ranked from most to least access frequency
* Standard (frequent, milliseconds)
* Intelligent Tiering (changing access patterns)
* Standard IA (infrequent access, milliseconds)
* One Zone IA
* Glacier (archived data, slower)

## Storages for Model Training
Ranked by speed of training load time
* AWS S3
* Amazon Elastic File System. Use if you store data there, as you can start taining jobs faster without copying the content first.
* Amazon Elastic Block Storage. Faster file transfer from storage to compute than EFS
* Amazon FSx for Lustre - files system in the could. Speeds up reading repeatedly accessed data from S3

### Amazon EBS Volumes
??

### Amazon S3 lifecycle configuration


# Domain 1.2: Identify and implement a data ingestion solution

## Services mentioned
* [AWS Kinesis](https://aws.amazon.com/kinesis/)
  * Video Streams
  * Data Streams
  * Data Firehorse
  * Data Analytics
* [AWS Glue](https://aws.amazon.com/glue/)
* [AWS Database Migration Service (DMS)](https://aws.amazon.com/dms/)
* [AWS StepFunctions](https://aws.amazon.com/stepfunctions/) - an orchestrator that can be potentially used for ETL pipelines.
* [Amazon Managed Streaming for Kafka](https://aws.amazon.com/msk/) - AWS managed Kafka

Terminology:
* **Data injestion** - Data ingestion is the process of importing larvge, assorted data files from multiple sources into a single, cloud-based storage medium—a data warehouse, data mart or database—where it can be accessed and analyzed. [Read more](https://www.teradata.com/insights/cloud-data-analytics/data-ingestion-in-analytics)

## Data Injection
There are two main types, batch and stream. **Batch processing** is used when there is no need for real-time injestion, and a periodically collected data is good enough. Batch injestion is running on a schedule (daily, monthly, ...) and is easier and cheaper to implement. on AWS it can be achieved with AWS Glue, an ETL-service. In addition, AWS DMS (database migration service that is possibel to use for this goal) or StepFunctions (a more general orchestrator alowing more complex workflows) can also be used.

With **stream processing**, on teh other hand, there is no scheduled reads of data. It is read as soon as it arrives. This is less cost-effectives, as it requires constantly monitoring changes in the data, but vital for real-time predictions. The main service for dealing with stream data in AWS is Kinesis. It provides several solutions, depending on the data type and the needs. Kinesis Video Streams processes video and audio data. [Data Streams](https://aws.amazon.com/kinesis/data-streams/) uses Producer and Client libraries to preprocess streaming data as it arrives and to emit the data. [Firehorse](https://aws.amazon.com/firehose/) allows to streams data to data lakes or warehouses. [Data Analytics](https://docs.aws.amazon.com/kinesisanalytics/latest/dev/what-is.html) provides the easiest way to process and transform the data that is streaming through Kinesis Data Streams or Kinesis Data Firehose using SQL.

# Domain 1.3: Identify and implement a data transformation solution
