# Cloud Intergation


## Introduction


- Introduction
- Amazon SQS – Standard Queue
- Amazon Kinesis


## Cloud Research


### #1.Introduction


- When we start deploying multiple applications, they will inevitably need to communicate with one another
- There are two patterns of application communication


![image](https://user-images.githubusercontent.com/121140952/219994047-47aa5f58-5102-42f8-9c09-a900256b531e.png)

- Synchronous between applications can be problematic if there are sudden spikes of traffic
- What if you need to suddenly encode 1000 videos but usually it’s 10?
- In that case, it’s better to decouple your applications:
- using SQS: queue model
- using SNS: pub/sub model
- using Kinesis: real-time data streaming model
- These services can scale independently from our application


### #2.  Amazon SQS – Standard Queue


- Oldest AWS offering (over 10 years old)
- Fully managed service (~serverless), use to decouple applications
- Scales from 1 message per second to 10,000s per second
- Default retention of messages: 4 days, maximum of 14 days
- No limit to how many messages can be in the queue
- Messages are deleted after they’re read by consumers
- Low latency (<10 ms on publish and receive)
- Consumers share the work to read messages & scale horizontally


### #3. Amazon Kinesis


- For the exam: Kinesis = real-time big data streaming
- Managed service to collect, process, and analyze real-time streaming data at any scale

- Too detailed for the Cloud Practitioner exam but good to know:
    - Kinesis Data Streams: low latency streaming to ingest data at scale from hundreds of thousands of sources
    - Kinesis Data Firehose: load streams into S3, Redshift, ElasticSearch, etc…
    - Kinesis Data Analytics: perform real-time analytics on streams using SQL
    - Kinesis Video Streams: monitor real-time video streams for analytics or ML


## Next Steps


- Amazon SNS, Amazon MQ, Integration-Summary


## Date


- February 20, 2023

