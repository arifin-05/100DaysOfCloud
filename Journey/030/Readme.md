# Cloud Integration

## Introduction


- Amazon SNS
- Amazon MQ
- Integration - Summary 


## Cloud Research


### #1. Amazon SNS


- The “event publishers” only sends message to one SNS topic
- As many “event subscribers” as we want to listen to the SNS topic notifications
- Each subscriber to the topic will get all the messages
- Up to 12,500,000 subscriptions per topic, 100,000 topics limit


### #2. Amazon MQ


- SQS, SNS are “cloud-native” services: proprietary protocols from AWS
- Traditional applications running from on-premises may use open protocols such as: MQTT, AMQP, STOMP, Openwire, WSS
- When migrating to the cloud, instead of re-engineering the application to use SQS and SNS, we can use Amazon MQ
- Amazon MQ is a managed message broker service for


![image](https://user-images.githubusercontent.com/121140952/220231278-8b5d16f7-bcf2-4b21-b877-49aee93731aa.png)


- Amazon MQ doesn’t “scale” as much as SQS / SNS
- Amazon MQ runs on servers, can run in Multi-AZ with failover
- Amazon MQ has both queue feature (~SQS) and topic features (~SNS)


### #3. Cloud Integration - Summary


- SQS:
    - Queue service in AWS
    - Multiple Producers, messages are kept up to 14 days
    - Multiple Consumers share the read and delete messages when done
    - Used to decouple applications in AWS
- SNS:
    - Notification service in AWS
    - Subscribers: Email, Lambda, SQS, HTTP, Mobile…
    - Multiple Subscribers, send all messages to all of them
    - No message retention
- Kinesis: real-time data streaming, persistence and analysis
- Amazon MQ: managed message broker for ActiveMQ and RabbitMQ in the cloud (MQTT, AMQP.. protocols)


## Next Steps


- Cloud Monitoring


## Date


- February 21, 2023

