# Account Management, Billing & Support (Part 2)


## Pricing Models in AWS

- AWS has 4 pricing models:
- Pay as you go: pay for what you use, remain agile, responsive, meet scale demands
- Save when you reserve: minimize risks, predictably manage budgets, comply with long-terms requirements
    - Reservations are available for EC2 Reserved Instances, DynamoDB Reserved Capacity, ElastiCache Reserved Nodes, RDS Reserved Instance, Redshift Reserved Nodes
- Pay less by using more: volume-based discounts
- Pay less as AWS grows


## Introduction


- Compute Pricing - EC2
- Compute Pricing - EC2
- Compute Pricing - Lambda & ECS 
- Storage Pricing - S3 
- Storage Pricing - EBS
- Database Pricing - RDS
- Database Pricing - RDS


## Cloud Research


### #1. Compute Pricing - EC2


- Only charged for what you use
- Number of instances
- Instance configuration:
    - Physical capacity
    - Region
    - OS and software
    - Instance type
    - Instance size
- ELB running time and amount of data processed
- Detailed monitoring


### #2. Compute Pricing - EC2


- On-demand instances:
    - Minimum of 60s
    - Pay per second (Linux/Windows) or per hour (other)
- Reserved instances:
    - Up to 75% discount compared to On-demand on hourly rate
    - 1- or 3-years commitment
    - All upfront, partial upfront, no upfront
- Spot instances:
    - Up to 90% discount compared to On-demand on hourly rate
    - Bid for unused capacity
- Dedicated Host:
    - On-demand
    - Reservation for 1 year or 3 years commitment
- Savings plans as an alternative to save on sustained usage
 
 
### #3. Compute Pricing - Lambda & ECS 


- Lambda:

    - Pay per call
    - Pay per duration

- ECS:
    - EC2 Launch Type Model: No additional fees, you pay for AWS resources stored and created in your application

- Fargate:
    - Fargate Launch Type Model: Pay for vCPU and memory resources allocated to your applications in your containers


### #4. Storage Pricing - S3


- Storage class: S3 Standard, S3 Infrequent Access, S3 One-Zone IA, S3 Intelligent Tiering, S3 Glacier and S3 Glacier Deep Archive
- Number and size of objects: Price can be tiered (based on volume)
- Number and type of requests
- Data transfer OUT of the S3 region
- S3 Transfer Acceleration
- Lifecycle transitions

- Similar service: EFS (pay per use, has infrequent access & lifecycle rules)


### #5. Storage Pricing - EBS


- Volume type (based on performance)
- Storage volume in GB per month provisionned
- IOPS:
    - General Purpose SSD: Included
    - Provisioned IOPS SSD: Provisionned amount in IOPS
    - Magnetic: Number of requests
- Snapshots:
    - Added data cost per GB per month
- Data transfer:
    - Outbound data transfer are tiered for volume discounts
    - Inbound is free


### #6. Database Pricing - RDS


- Per hour billing
- Database characteristics:
    - Engine
    - Size
    - Memory class
- Purchase type:
    - On-demand
    - Reserved instances (1 or 3 years) with required up-front
- Backup Storage: There is no additional charge for backup storage up to 100% of your total database storage for a region. 


### #7. Database Pricing - RDS


- Additional storage (per GB per month)
- Number of input and output requests per month
- Deployment type (storage and I/O are variable):
    - Single AZ
    - Multiple AZs
- Data transfer:
    - Outbound data transfer are tiered for volume discounts
    - Inbound is free


## Next Steps


- Account Management, Billing & Support (Part 3)

