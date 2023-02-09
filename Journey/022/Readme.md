# Other Compute (Part 2)


## Introduction


- Amazon API Gateway
- AWS Bath
- Batch vs Lambda
- Amazon Lightsail
- Other Compute - SUmmary
- Lambda - SUmmary


## Cloud Research


### #1. Amazon API Gateway


- Example: building a serverless API

![image](https://user-images.githubusercontent.com/121140952/217696475-7038aa4d-279e-4ca7-afe9-2a6f0b1027a5.png)

- Fully managed service for developers to easily create, publish, maintain, monitor, and secure APIs
- Serverless and scalable
- Supports RESTful APIs and WebSocket APIs
- Support for security, user authentication, API throttling, API keys, monitoring... 


### #2. AWS Bath


- Fully managed batch processing at any scale
- Efficiently run 100,000s of computing batch jobs on AWS
- A “batch” job is a job with a start and an end (opposed to continuous)
- Batch will dynamically launch EC2 instances or Spot Instances
- AWS Batch provisions the right amount of compute / memory
- You submit or schedule batch jobs and AWS Batch does the rest!
- Batch jobs are defined as Docker images and run on ECS
- Helpful for cost optimizations and focusing less on the infrastructure


### #3. Batch vs Lambda


- Lambda:
    - Time limit
    - Limited runtimes
    - Limited temporary disk space
    - Serverless


- Batch:
    - No time limit- Any runtime as long as it’s packaged as a Docker image
    - Rely on EBS / instance store for disk space
    - Relies on EC2 (can be managed by AWS)


### #4. Amazon Lightsail


- Virtual servers, storage, databases, and networking
- Low & predictable pricing
- Simpler alternative to using EC2, RDS, ELB, EBS, Route 53…
- Great for people with little cloud experience!
- Can setup notifications and monitoring of your Lightsail resources
- Use cases:
    - Simple web applications (has templates for LAMP, Nginx, MEAN, Node.js…)
    - Websites (templates for WordPress, Magento, Plesk, Joomla)
    - Dev / Test environment
- Has high availability but no auto-scaling, limited AWS integrations


### #5. Other Compute - SUmmary


- Docker: container technology to run applications
- ECS: run Docker containers on EC2 instances
- Fargate:
    - Run Docker containers without provisioning the infrastructure
    - Serverless offering (no EC2 instances)
- ECR: Private Docker Images Repository
- Batch: run batch jobs on AWS across managed EC2 instances
- Lightsail: predictable & low pricing for simple application & DB stacks


### #6. Lambda - SUmmary


- Lambda is Serverless, Function as a Service, seamless scaling, reactive
- Lambda Billing:
    - By the time run x by the RAM provisioned
    - By the number of invocations
- Language Support: many programming languages except (arbitrary) Docker
- Invocation time: up to 15 minutes
- Use cases:
    - Create Thumbnails for images uploaded onto S3
    - Run a Serverless cron job
    - API Gateway: expose Lambda functions as HTTP API


## Next Steps

- Deploying and Managing Infrastructure at Scale

## Date
- February 10, 2023
