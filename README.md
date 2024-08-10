# AWS Machine Learning Exam

![AWS-Certified-Machine-Learning-Specialty_badge](images/aws_badge.png)
Welcome to this unofficial exam preparation guide for the AWS Certified - Machine Learning Specialty Exam.

The guide contains all links to all materials you would need to prepare for the exam from scratch, a cheetsheet for the AWS services likely to appear in the exam, and my notes on 4 topics covered by the exam. 

Although this was made for MLS-C01 (Machine Learning Specialty) Exam, it should also cover both Associate ML Exams - (Machine Learning Associate) and (Machine Learning Engineer Associate). The extra material useful just for ML Engineer exam appears is marked.

> [!NOTE]
> The notes are supposed to help you revise before the exam, not study the topics from scratch. If you are a beginner to ML, I recommend on doing a full ML course first. This project is aimed more at Data Scientists/ML Engineers already working in the field, but missing the full scope of AWS services available for ML Lifecycle.

- [AWS Machine Learning Exam](#aws-machine-learning-exam)
  - [Preparatory Courses](#preparatory-courses)
    - [AWS Official (SkillBuilder)](#aws-official-skillbuilder)
    - [Non-Official](#non-official)
  - [How to Start?](#how-to-start)
  - [Exam Contents (High Level)](#exam-contents-high-level)
  - [Cheatsheet: AWS Services for ML](#cheatsheet-aws-services-for-ml)
  - [Topics](#topics)
    - [Data Engineering on AWS](#data-engineering-on-aws)
    - [Data Analytics on AWS](#data-analytics-on-aws)
    - [ML on AWS](#ml-on-aws)
    - [MLOps on AWS](#mlops-on-aws)
  - [Machine Learning Engineer Associate Exam](#machine-learning-engineer-associate-exam)
  - [AWS Services for the Exam](#aws-services-for-the-exam)
        - [Amazon Kinesis](#amazon-kinesis)
        - [Amazon Data Firehose](#amazon-data-firehose)
        - [Amazon EMR](#amazon-emr)
        - [AWS Glue](#aws-glue)
        - [Amazon Managed Service for Apache Flink](#amazon-managed-service-for-apache-flink)
        - [AWS Data Pipeline](#aws-data-pipeline)
        - [AWS Batch](#aws-batch)
        - [Amazon S3](#amazon-s3)
        - [Amazon EFS](#amazon-efs)
        - [Amazon EBS](#amazon-ebs)
        - [Amazon Athena](#amazon-athena)
        - [Amazon Quicksight](#amazon-quicksight)
        - [AWS DynamoDB](#aws-dynamodb)
        - [AWS SageMaker](#aws-sagemaker)
        - [AWS Forecast](#aws-forecast)
        - [AWS Bedrock](#aws-bedrock)
        - [AWS Kendra](#aws-kendra)
        - [AWS DeepRacer](#aws-deepracer)
        - [AWS Textract](#aws-textract)
        - [AWS Personalize](#aws-personalize)
        - [AWS Lookout](#aws-lookout)
        - [AWS Monitron](#aws-monitron)
        - [AWS Comprehend](#aws-comprehend)
        - [AWS Translate](#aws-translate)
        - [AWS Comprehend](#aws-comprehend-1)
        - [AWS Polly](#aws-polly)
        - [AWS Lex](#aws-lex)
        - [AWS Rekognition](#aws-rekognition)
        - [AWS Lambda](#aws-lambda)
        - [AWS DMS](#aws-dms)
        - [AWS StepFunctions](#aws-stepfunctions)
        - [AWS DataSync](#aws-datasync)
        - [AWS IoT Greengrass](#aws-iot-greengrass)
        - [AWS KMS](#aws-kms)
        - [AWS IAM](#aws-iam)
        - [AWS Macie](#aws-macie)
        - [AWS CloudWatch](#aws-cloudwatch)
        - [AWS CloudTrail](#aws-cloudtrail)
        - [AWS VPC](#aws-vpc)
        - [AWS EC2](#aws-ec2)
  - [Type of Questions](#type-of-questions)
  - [Answering Strategies](#answering-strategies)

## Preparatory Courses
### AWS Official (SkillBuilder)
[Machine Learning: Exam Preparation](https://aws.amazon.com/training/learning-paths/machine-learning/exam-preparation/) - an official roadmap of AWS courses to be ready for the exam. Many of the courses are not free (come with AWS SkillBuilder subsription at $29 per month), although some shorter content is available for free. In both cases you would need an AWS acount. 

[Exam Guide](https://d1.awsstatic.com/training-and-certification/docs-ml/AWS-Certified-Machine-Learning-Specialty_Exam-Guide.pdf) - list of topics and service typically appearing in the exam. It also list AWS services you do not need for the exam, to avoid wasting time on over-preparing.

[Practice Exam - 20 Questions]()

### Non-Official
Personally I preferrd this course by Frank Kane:
[AWS Certified Machine Learning Specialty 2024 - Hands On!](https://www.udemy.com/course/aws-machine-learning/?couponCode=ST10MT8624)

I found it more structured than AWS official preparation material and Udemy UI to be easier to navigate than AWS Skillbuilder. I would suggest to take the Udemy course (if you feel you need any at all),

## How to Start?
I would suggest preparing in the following way:
1. ${\color{fuchsia}\textsf{Identify Your gaps}}$ Take the practice exam to find **where your gaps are** and which topics you need to cover. If you scored 70+ points on your first try, perhaps it doesn't make sense to spend 20h on teh video course and you should focus on specific ML topic/AWS services only. 
2. (Optional) ${\color{fuchsia}\textsf{Take a video course}}$ Depending on the gaps you identified in (1), either go through a full course (if your score was low), or partial, focusing on areas of interest.
3. ${\color{fuchsia}\textsf{Revise with notes}}$ You can either use your personal notes or go through mine on this repo.
4. ${\color{fuchsia}\textsf{Practice exam}}$ Go through a mock test again.
5. (Optional, but recommended) ${\color{fuchsia}\textsf{Take an official Exam Readiness Test}}$ on AWS SkillBulder. It imitates the full test experience, to make you feel comfortable with the UI and the timing.


## Exam Contents (High Level)
See official [Exam Guide](https://d1.awsstatic.com/training-and-certification/docs-ml/AWS-Certified-Machine-Learning-Specialty_Exam-Guide.pdf) for mode details

There are 65 questions in total, either (1) multiple choice or (2) multiple selection. Out of 65 questions, 15 are unscored (they are beta questions that might be scored in the future). The unscored questions are not marked, so you should treat all questiions equally serious. You should never skip a question and at least try to guess, as wrong answer results in the same zero points as does the no answer.

Exam lasts 170 min, and you can get 30 min extra if you are a non-native speaker, but you must request this in advance.

The questions are related to 4 main topics and a question may require knowledge about any combination of those. The topics are:

• Data Engineering *(20% of scored content)*
  - Storage ([Amazon S3](https://aws.amazon.com/s3/), [Amazon EFS](https://aws.amazon.com/de/efs/), [Amazon EBS](https://aws.amazon.com/ebs/))
  - Orchestration ([Amazon Kinesis](https://aws.amazon.com/kinesis/), [Amazon Data Firehose](https://aws.amazon.com/firehose/), [Amazon EMR](https://aws.amazon.com/emr/), [AWS Glue](https://aws.amazon.com/glue/), [Amazon Managed Service for Apache Flink](https://aws.amazon.com/managed-service-apache-flink/))
  - ETL ([AWS Glue](https://aws.amazon.com/glue/), [AWS Data Pipeline](https://docs.aws.amazon.com/data-pipeline/), [Amazon EMR](https://aws.amazon.com/emr/), [AWS Batch](https://aws.amazon.com/batch))
  - Big Data with MapReduce (for example, [Apache Hadoop](https://aws.amazon.com/emr/features/hadoop/), [Apache Spark](https://aws.amazon.com/emr/features/spark/), [Apache Hive](https://aws.amazon.com/emr/features/hive/))

• Data Analytics (EDA) *(24% of scored content)*

• Modelling (ML) (36% of scored content) 

• MLOps *(20% of scored content)*


## Cheatsheet: AWS Services for ML
[image]()

## Topics

### Data Engineering on AWS
Data storage, injestion and transformation.

**Key services**:
- Storage: Lake Formation, S3, EFS, EBS, FSx
- Injestion: Kinesis (Firehorse, Data Streams, Video Streams), Glue, DMS, StepFunctions
- Transformation: EMR (managed Spark), Athena, Quicksight, Redshift Spectrum

**Key terms**: data lake, data mesh, data warehouse, data injestion, batch processing, streaming

This part accounts for 20% of the scored content.
Read more [here](1_Data_Engineering.md)

### Data Analytics on AWS
This part accounts for 24% of the scored content.
Read more [here](2_Data_Analytics.md)

### ML on AWS
This part accounts for 36% of the scored content.
Read more [here](3_Machine_Learning.md)

### MLOps on AWS
This part accounts for 20% of the scored content.
Read more [here](4_MLOps.md)

## Machine Learning Engineer Associate Exam
This section contains materials specifically for the Machine Learning Engineer Associate Exam, the parts that were not covered by MLS-C01 notes.


## AWS Services for the Exam

##### [Amazon Kinesis](https://aws.amazon.com/kinesis/)
Amazon Kinesis Data Streams is a serverless streaming data service that simplifies the capture, processing, and storage of data streams at any scale. With Amazon Kinesis Video Streams, you can more easily and securely stream video from connected devices to AWS for analytics, ML, playback, and other processing.
##### [Amazon Data Firehose](https://aws.amazon.com/firehose/)
Amazon Data Firehose is the easiest way to capture, transform, and deliver data streams into Amazon S3, Amazon Redshift, Amazon OpenSearch Service, Splunk, Snowflake, and other 3rd party analytics services
##### [Amazon EMR](https://aws.amazon.com/emr/)
Amazon EMR (Amazon Elastic MapReduce) is a managed cluster platform that simplifies running big data frameworks, such as Apache Hadoop and Apache Spark , on AWS to process and analyze vast amounts of data.
##### [AWS Glue](https://aws.amazon.com/glue/)
AWS Glue provides a serverless solution that simplifies the entire process of discovering, preparing, and combining data for application development, machine learning, and analytics.
Glue ETL, DataQuality, DataBrew and Data Catalog
##### [Amazon Managed Service for Apache Flink](https://aws.amazon.com/managed-service-apache-flink/)
With Amazon Managed Service for Apache Flink, you can transform and analyze streaming data in real time using Apache Flink and integrate applications with other AWS services. There are no servers and clusters to manage, and there is no compute and storage infrastructure to set up.
##### [AWS Data Pipeline](https://docs.aws.amazon.com/data-pipeline/)
AWS Data Pipeline is a web service that you can use to automate the movement and transformation of data. With AWS Data Pipeline, you can define data-driven workflows, so that tasks can be dependent on the successful completion of previous tasks. You define the parameters of your data transformations and AWS Data Pipeline enforces the logic that you've set up.
##### [AWS Batch](https://aws.amazon.com/batch)
##### [Amazon S3](https://aws.amazon.com/s3/)
##### [Amazon EFS](https://aws.amazon.com/de/efs/)
##### [Amazon EBS](https://aws.amazon.com/ebs/)
##### [Amazon Athena](https://aws.amazon.com/athena/)
##### [Amazon Quicksight](https://aws.amazon.com/quicksight/)
##### [AWS DynamoDB](https://aws.amazon.com/dynamodb/)
##### [AWS SageMaker](https://aws.amazon.com/sagemaker/)
##### [AWS Forecast](https://aws.amazon.com/forecast/)
##### [AWS Bedrock](https://aws.amazon.com/bedrock/)
##### [AWS Kendra](https://aws.amazon.com/kendra/)
Amazon Kendra is an intelligent search service that uses natural language processing and advanced machine learning algorithms to return specific answers to search questions from your data.
##### [AWS DeepRacer](hhttps://aws.amazon.com/deepracer/)
Build models in Amazon SageMaker and train, test, and iterate quickly and easily on the track in the AWS DeepRacer 3D racing simulator.
##### [AWS Textract](hhttps://aws.amazon.com/textract/)
Amazon Textract is a machine learning (ML) service that automatically extracts text, handwriting, layout elements, and data from scanned documents.
##### [AWS Personalize](https://aws.amazon.com/personalize/)
##### [AWS Lookout](https://aws.amazon.com/lookout/)
##### [AWS Monitron](https://aws.amazon.com/monitron/)
##### [AWS Comprehend](https://aws.amazon.com/comprehend/)
##### [AWS Translate](https://aws.amazon.com/translate/)
##### [AWS Comprehend](https://aws.amazon.com/comprehend/)
##### [AWS Polly](https://aws.amazon.com/polly/)
##### [AWS Lex](https://aws.amazon.com/lex/)
##### [AWS Rekognition](https://aws.amazon.com/rekognition/)
##### [AWS Lambda](https://aws.amazon.com/lambda/)
##### [AWS DMS](https://aws.amazon.com/dms/)
##### [AWS StepFunctions](https://aws.amazon.com/step-functions/)
##### [AWS DataSync](https://aws.amazon.com/datasync/)
##### [AWS IoT Greengrass]()
##### [AWS KMS](https://aws.amazon.com/kms/)
##### [AWS IAM](https://aws.amazon.com/iam/)
##### [AWS Macie](https://aws.amazon.com/macie/)
##### [AWS CloudWatch](https://aws.amazon.com/cloudwatch/)
##### [AWS CloudTrail](https://aws.amazon.com/cloudtrail/)
##### [AWS VPC](https://aws.amazon.com/vpc/)
Amazon Virtual Private Cloud (VPC) is a service that lets you launch AWS resources in a logically isolated virtual network that you define.
##### [AWS EC2](https://aws.amazon.com/ec2/)


## Type of Questions
Questions focus on a scenario where a Data Scientists/Machine Leanring Engineer is facing a certain problem. Some examples: 

1. What is the easiest/least operationally heavy way to ...
2. What ML model would you use to ...
3. Given the problem in this industry/context, what AWS service should you use? (industry- or context-specific services)


## Answering Strategies

> [!TIP]
> Questions are supposed to included only relevant information, no trick information is added to make you confused or distracted

> [!TIP]
> Try to answer the question before even looking at the answer choices, then see if any of those answer choices match your original answer.

> [!TIP]
> Identify the key phrases and qualifiers in the question. It can be keywords like "most operationally efficient".

> [!TIP]
> Get to the correct answer by elimination.

> [!TIP]
> When you are unsure, flag the question and continue. You can come back to the marked questions later.
