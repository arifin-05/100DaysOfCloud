# Pillars Well Architected Framework Part 1


## Introduction


- Operational Excellence
- Security
- Reliability


## Cloud Research


#1. Operational Excellence Includes the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures

- Design Principles :
    - Perform operations as code - Infrastructure as code
    - Annotate documentation - Automate the creation of annotated documentation after every build
    - Make frequent, small, reversible changes - So that in case of any failure, you can reverse it
    - Refine operations procedures frequently - And ensure that team members are familiar with it
    - Anticipate failure
    - Learn from all operational failures Operational excellence AWS Service :
- Prepare : AWS CloudFormation, AWS Config
- Operate : AWS CloudFormation, AWS Config, AWS CloudTrail, CloudWatch, AWS X-Ray
- Evolve : AWS CloudFormation, AWS CodeBuild, AWS CodeCommit, AWS CodeDeploy, AWS CodePipeline

#2. Security Includes the ability to protect information, systems, and assets while deliverin business values through risk assessments and mitigation strategies

- Design Principles :
- Implement a strong identity foundation - Centralize privilege management and reduce (or even eliminate) reliability on long-term credentials - Principle of least privilege - IAM
- Enable traceability - Integrate logs and metrics with systems to automatically respond and take action
- Apply security at all layers - Like edge network, VPC, subnet, load balancer, every instance, operating system, and application
- Automate security best practices
- Protect data in transit and at rest - Encryption, tokenization, and access control
- Keep people away from data - Reduce or eliminate the need for direct or manual access processing of data
- Prepare for security events - Run incident response simulations and use tools with automation to increase your speed for detection, investigation, and recovery

AWS services used for security :

- Identity and Access Management : IAM, AWS-STS, MFA token, AWS Organizations
- Detective Controls : AWS Config, AWS CloudTrail, Amazon CloudWatch
- Infrastructure Protection : Amazon CloudFront, Amazon VPC, AWS Shield, AWS WAF, Amazon Inspector
- Data Protection : KMS, S3, Elastic Load Balancing (ELB), Amazon EBS, Amazon RDS
- Incident Response : IAM, AWS CloudFormation, Amazon CloudWatch Events

#3. Reliability Ability of a system to recover from infrastructure or service disruptions,dynamically acquire computing resources to meet demand, and mitigate disruptions such as misconfigurations or transient network issues

Design Principles : 
- Test recovery procedures - Use automation to simulate different failures or to recreate scenarios that led to failures before 
- Automatically recover from failure - Anticipate and remediate failures before they occur 
- Scale horizontally to increase aggregate system availability - Distribute requests across multiple, smaller resources to ensure that they don't share a common point of failure
- Stop guessing capacity - Maintain the optimal level to satisfy demand without over or under provisioning - Use Auto Scaling
- Manage change in automation - Use automation to make changes to infrastructure

AWS services used for reliability :

- Foundations : IAM, VPC, Service limit, AWS Trusted Advisor
- Change management : Auto scaling, CloudWatch, CloudTrail, AWS Config
- Failure management : Backups, CloudFormation, S3, S3 Glacier, Route 53

