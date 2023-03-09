# Security & Compliance Part 2


## Introduction


- CloudHSM 
- Types of CMK
- AWS Certificate Manager (ACM)
- AWS Secrets Manager
- AWS Artifact
- Amazon GuardDuty


## Cloud Research


### #1. CloudHSM


- KMS => AWS manages the software for encryption
- CloudHSM => AWS provisions encryption hardware
- Dedicated Hardware (HSM = Hardware Security Module)
- You manage your own encryption keys entirely (not AWS)
- HSM device is tamper resistant, FIPS 140 -2 Level 3 compliance


### #2. Types of CMK (Customer Master Keys)


- Customer Managed CMK:
    - Create, manage and used by the customer, can enable or disable
    - Possibility of rotation policy (new key generated every year, old key preserved)
    - Possibility to bring-your-own-key
- AWS managed CMK:
    - Created, managed and used on the customer’s behalf by AWS
    - Used by AWS services (aws/s3, aws/ebs, aws/redshift)
- AWS owned CMK:
    - Collection of CMKs that an AWS service owns and manages to use in multiple accounts
    - AWS can use those to protect resources in your account (but you can’t view the keys)
- CloudHSM Keys (custom keystore):
    - Keys generated from your own CloudHSM hardware device
    - Cryptographic operations are performed within the CloudHSM cluster


### #3. AWS Certificate Manager (ACM)


- Let’s you easily provision, manage, and deploy SSL/TLS Certificates
- Used to provide in-flight encryption for websites (HTTPS)
- Supports both public and private TLS certificates
- Free of charge for public TLS certificates
- Automatic TLS certificate renewal
- Integrations with (load TLS certificates on)
- Elastic Load Balancers
- CloudFront Distributions
- APIs on API Gateway


### #4. AWS Secrets Manager


- Newer service, meant for storing secrets
- Capability to force rotation of secrets every X days
- Automate generation of secrets on rotation (uses Lambda)
- Integration with Amazon RDS (MySQL, PostgreSQL, Aurora)
- Secrets are encrypted using KMS
- Mostly meant for RDS integration


### #5. AWS Artifact


- Portal that provides customers with on-demand access to AWS compliance documentation and AWS agreements
- Artifact Reports - Allows you to download AWS security and compliance documents from third-party auditors, like AWS ISO certifications, Payment Card Industry (PCI), and System and Organization Control (SOC) reports
- Artifact Agreements - Allows you to review, accept, and track the status of AWS agreements such as the Business Associate Addendum (BAA) or the Health Insurance Portability and Accountability Act (HIPAA) for an individual account or in your organization
- Can be used to support internal audit or compliance


### #6. Amazon GuardDuty


- Intelligent Threat discovery to protect your AWS Account
- Uses Machine Learning algorithms, anomaly detection, 3rd party data
- One click to enable (30 days trial), no need to install software
- Input data includes:
    - CloudTrail Events Logs – unusual API calls, unauthorized deployments
     - CloudTrail Management Events – create VPC subnet, create trail, …
     - CloudTrail S3 Data Events – get object, list objects, delete object, …
    - VPC Flow Logs – unusual internal traffic, unusual IP address
    - DNS Logs – compromised EC2 instances sending encoded data within DNS queries
    - Kubernetes Audit Logs – suspicious activities and potential EKS cluster compromises
- Can setup EventBridge rules to be notified in case of findings
- EventBridge rules can target AWS Lambda or SNS
- Can protect against CryptoCurrency attacks (has a dedicated “finding” for it)


## Next Steps


- Security & Compliance Part 3 


## Date


- March 9, 2023

