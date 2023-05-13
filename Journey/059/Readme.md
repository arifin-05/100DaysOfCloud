# Other AWS Services Part 3


## Introduction


- AWS Application Discovery Service
- AWS Application Migration Service (MGN)
- AWS Fault Injection Simulator (FIS)
- AWS Step Functions
- AWS Ground Station
- Amazon Pinpoint


## Cloud Research


### #1. AWS Application Discovery Service


- Plan migration projects by gathering information about on-premises data centers
- Server utilization data and dependency mapping are important for migrations

- Agentless Discovery (AWS Agentless Discovery Connector)
    - VM inventory, configuration, and performance history such as CPU, memory, and disk usage
- Agent-based Discovery (AWS Application Discovery Agent)
    - System configuration, system performance, running processes, and details of the network connections between systems
- Resulting data can be viewed within AWS Migration Hub


### #2. AWS Application Migration Service (MGN)


- The “AWS evolution” of CloudEndure Migration, replacing AWS Server Migration Service (SMS)

- Lift-and-shift (rehost) solution which simplify migrating applications to AWS
- Converts your physical, virtual, and cloud-based servers to run natively on AWS
- Supports wide range of platforms, Operating Systems, and databases
- Minimal downtime, reduced costs


### #3. AWS Fault Injection Simulator (FIS)


- A fully managed service for running fault injection experiments on AWS workloads
- Based on Chaos Engineering – stressing an application by creating disruptive events (e.g., sudden increase in CPU or memory), observing how the system responds, and implementing improvements
- Helps you uncover hidden bugs and performance bottlenecks
- Supports the following AWS services: EC2, ECS, EKS, RDS…
- Use pre-built templates that generate the desired disruptions


### #4. AWS Step Functions


- Build serverless visual workflow to orchestrate your Lambda functions
- Features: sequence, parallel, conditions, timeouts, error handling, …
- Can integrate with EC2, ECS, On
-premises servers, API Gateway, SQS queues, etc …
- Possibility of implementing human approval feature
- Use cases: order fulfillment, data processing, web applications, any workflow


### #5. AWS Ground Station


- Fully managed service that lets you control satellite communications, process data, and scale your satellite operations
- Provides a global network of satellite ground stations near AWS regions
- Allows you to download satellite data to your AWS VPC within seconds
- Send satellite data to S3 or EC2 instance
- Use cases: weather forecasting, surface imaging, communications, video broadcasts


### #6. Amazon Pinpoint


- Scalable 2-way (outbound/inbound) marketing communications service
- Supports email, SMS, push, voice, and in-app messaging
- Ability to segment and personalize messages with the right content to customers
- Possibility to receive replies
- Scales to billions of messages per day
- Use cases: run campaigns by sending marketing, bulk, transactional SMS messages
- Versus Amazon SNS or Amazon SES
    - In SNS & SES you managed each message's audience, content, and delivery schedule
    - In Amazon Pinpoint, you create message templates, delivery schedules, highly-targeted segments, and full campaigns


## Next Steps


- AWS Architecting & Ecosystem

