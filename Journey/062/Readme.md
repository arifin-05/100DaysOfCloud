# Pillars Well Architected Framework Part 2


## Introduction


- Performance Efficiency
- Cost Optimization
- Sustainability


## Cloud Research


### #4. Performance Efficiency

- Includes the ability to use computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve

- Design Principles :
    - Democratize advanced technologies - Advance technologies become services and hence you can focus more on product development
    - Go global in minutes - Easy deployment in multiple regions
    - Use serverless architectures - Avoid burden of managing servers
    - Experiment more often - Easy to carry out comparative testing
    - Mechanical sympathy - Be aware of all AWS services

AWS services used fo performance efficiency :

- Selection : Auto Scaling, AWS Lambda, Amazon EBS, Amazon (S3), Amazon RDS
- Review : AWS CloudFormation, AWS News Blog
- Monitoring : Amazon CloudWatch, AWS Lambda
- Tradeoffs : Amazon RDS, Amazon ElastiCache, AWS Snowball, Amazon CloudFront

### #5. Cost Optimization 


Includes the ability to run systems to deliver business value at the lowest price point

- Design Principles :
- Adopt a consumption mode - Pay only for what you use
- Measure overall efficiency - Use CloudWatch
- Stop spending money on data center operations - AWS does the infrastructure part and enables customer to focus on organization projects
- Analyze and attribute expenditure - Accurate identification of system usage and costs, helps measure return on investment (ROI) - Make sure to use tags
- Use managed and application level services to reduce cost of ownership - As managed services operate at cloud scale, they can offer a lower cost per transaction or service

AWS services used for Cost Optimization :

- Expenditure Awareness : AWS Budgets, AWS Cost and Usage Report, AWS Cost Explorer, Reserved Instance Reporting
- Cost-Effective Resources : Spot instance, Reserved instance, Amazon S3 Glacier
- Matching supply and demand : AWS Auto Scaling, AWS Lambda
- Optimizing Over Time : AWS Trusted Advisor, AWS Cost and Usage Report,AWS News Blog


### 6. Sustainability


- The sustainability pillar focuses on minimizing the environmental impacts of running cloud workloads.
- Design Principles
    - Understand your impact – establish performance indicators, evaluate improvements - Establish sustainability goals – Set long-term goals for each workload, model return on investment (ROI)
    - Maximize utilization – Right size each workload to maximize the energy efficiency of the underlying hardware and minimize idle resources.
    - Anticipate and adopt new, more efficient hardware and software offerings – and design for flexibility to adopt new technologies over time.
    - Use managed services – Shared services reduce the amount of infrastructure; Managed services help automate sustainability best practices as moving infrequent accessed data to cold storage and adjusting compute capacity.
    - Reduce the downstream impact of your cloud workloads – Reduce the amount of energy or resources required to use your services and reduce the need for your customers to upgrade their devices

AWS services used for Sustainability :

- EC2 Auto Scaling, Serverless Offering (Lambda, Fargate)
- Cost Explorer, AWS Graviton 2, EC2 T instances, @Spot Instances
- EFS-IA, Amazon S3 Glacier, EBS Cold HDD volumes
- S3 Lifecycle Configurations, S3 Intelligent Tiering
- Amazon Data Lifecycle Manager
- Read Local, Write Global: RDS Read Replicas, Aurora Global DB, DynamoDB Global Table, CloudFront

