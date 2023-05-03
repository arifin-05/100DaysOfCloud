# Account Management, Billing & Support (Part 3)


## Introduction


- Savings Plan
- AWS Compute Optimizer
- Billing and Costing Tools
- Cost Allocation Tags
- Tagging and Resource Groups
- Cost Explorer
- Trusted Advisor 


## Cloud Research


### #1. Savings Plan


- Commit a certain $ amount per hour for 1 or 3 years
- Easiest way to setup long-term commitments on AWS
- EC2 Savings Plan
    - Up to 72% discount compared to On-Demand
    - Commit to usage of individual instance families in a region (e.g. C5 or M5)
    - Regardless of AZ, size (m5.xl to m5.4xl), OS (Linux/Windows) or tenancy
    - All upfront, partial upfront, no upfront
- Compute Savings Plan
    - Up to 66% discount compared to On-Demand
    - Regardless of Family, Region, size, OS, tenancy, compute options
    - Compute Options: EC2, Fargate, Lambda
- Machine Learning Savings Plan: SageMaker…
- Setup from the AWS Cost Explorer console
- Estimate pricing at https://aws.amazon.com/savingsplans/pricing/


### #2. AWS Compute Optimizer


- Reduce costs and improve performance by recommending optimal AWS resources for your workloads
- Helps you choose optimal configurations and right
- size your workloads (over/under provisioned)
- Uses Machine Learning to analyze your resources’ configurations and their utilization CloudWatch metrics
- Supported resources
    - EC2 instances
    - EC2 Auto Scaling Groups
    - EBS volumes
    - Lambda functions
- Lower your costs by up to 25%
- Recommendations can be exported to S3


### #3. Billing and Costing Tools


- Estimating costs in the cloud:
- Pricing Calculator
- Tracking costs in the cloud:
    - Billing Dashboard
    - Cost Allocation Tags
    - Cost and Usage Reports
    - Cost Explorer
- Monitoring against costs plans:
    - Billing Alarms
    - Budgets


### #4. Cost Allocation Tags


- Use cost allocation tags to track your AWS costs on a detailed level
- AWS generated tags
    - Automatically applied to the resource you create
    - Starts with Prefix aws: (e.g. aws: createdBy)
- User-defined tags
    - Defined by the user
    - Starts with Prefix user: 


### #5. Tagging and Resource Groups


- Tags are used for organizing resources:
    - EC2: instances, images, load balancers, security groups…
    - RDS, VPC resources, Route 53, IAM users, etc…
    - Resources created by CloudFormation are all tagged the same way

- Free naming, common tags are: Name, Environment, Team …

- Tags can be used to create Resource Groups
    - Create, maintain, and view a collection of resources that share common tags
    - Manage these tags using the Tag Editor


### #6. Cost Explorer


- Visualize, understand, and manage your AWS costs and usage over time
- Create custom reports that analyze cost and usage data.
- Analyze your data at a high level: total costs and usage across all accounts
- Or Monthly, hourly, resource level granularity
- Choose an optimal Savings Plan (to lower prices on your bill)
- Forecast usage up to 12 months based on previous usage


### #7. Trusted Advisor 


- No need to install anything – high level AWS account assessment

- Analyze your AWS accounts and provides recommendation on 5 categories
- Cost optimization 
- Performance
- Security
- Fault tolerance
- Service limits


## Next Steps


- Account Management, Billing & Support (Part 4)

