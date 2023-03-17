
# Security & Compliance Part 3


## Introduction


- Amazon Inspector
- AWS Config
- AWS Macie
- AWS Security Hub
- Amazon Detective
- Root user privileges
- Summary


## Cloud Research


### #1. • Automated Security Assessments


- Automated Security Assessments

- For EC2 instances
    - Leveraging the AWS System Manager (SSM) agent
    - Analyze against unintended network accessibility
    - Analyze the running OS against known vulnerabilities
- For Container Images push to Amazon ECR
    - Assessment of Container Images as they are pushed
- For Lambda Functions
    - Identifies software vulnerabilities in function code and package dependencies
    - Assessment of functions as they are deployed

- Reporting & integration with AWS Security Hub
- Send findings to Amazon Event Bridge


### #2. AWS Config


- Helps with auditing and recording compliance of your AWS resources
- Helps record configurations and changes over time
- Possibility of storing the configuration data into S3 (analyzed by Athena)
- Questions that can be solved by AWS Config:
    - Is there unrestricted SSH access to my security groups?
    - Do my buckets have any public access?
    - How has my ALB configuration changed over time?
- You can receive alerts (SNS notifications) for any changes
- AWS Config is a per-region service
- Can be aggregated across regions and accounts


### #3. AWS Macie


- Amazon Macie is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect your sensitive data in AWS.
- Macie helps identify and alert you to sensitive data, such as personally identifiable information (PII)


### #4. AWS Security Hub


- Central security tool to manage security across several AWS accounts and automate security checks
- Integrated dashboards showing current security and compliance status to quickly take actions
- Automatically aggregates alerts in predefined or personal findings formats from various AWS services & AWS partner tools:
    - GuardDuty
    - Inspector
    - Macie
    - IAM Access Analyzer
    - AWS Systems Manager
    - AWS Firewall Manager
    - AWS Partner Network Solutions
- Must first enable the AWS Config Service


### #5. Amazon Detective


- GuardDuty, Macie, and Security Hub are used to identify potential security issues, or findings
- Sometimes security findings require deeper analysis to isolate the root cause and take action – it’s a complex process
- Amazon Detective analyzes, investigates, and quickly identifies the root cause of security issues or suspicious activities (using ML and graphs)
- Automatically collects and processes events from VPC Flow Logs, CloudTrail, GuardDuty and create a unified view
- Produces visualizations with details and context to get to the root cause


### #6. Root user privileges


- Root user = Account Owner (created when the account is created)
- Has complete access to all AWS services and resources
- Lock away your AWS account root user access keys!
- Do not use the root account for everyday tasks, even administrative tasks
- Actions that can be performed only by the root user:
    - Change account settings (account name, email address, root user password, root user access keys)  
    - View certain tax invoices
    - Close your AWS account
    - Restore IAM user permissions
    - Change or cancel your AWS Support plan
    - Register as a seller in the Reserved Instance Marketplace
    - Configure an Amazon S3 bucket to enable MFA
    - Edit or delete an Amazon S3 bucket policy that includes an invalid VPC ID or VPC endpoint ID
    - Sign up for GovCloud


### #7. Summary


- Shared Responsibility on AWS
- Shield: Automatic DDoS Protection + 24/7 support for advanced
- WAF: Firewall to filter incoming requests based on rules
- KMS: Encryption keys managed by AWS
- CloudHSM: Hardware encryption, we manage encryption keys
- AWS Certificate Manager: provision, manage, and deploy SSL/TLS Certificates
- Artifact: Get access to compliance reports such as PCI, ISO, etc…
- GuardDuty: Find malicious behavior with VPC, DNS & CloudTrail Logs
- Inspector: For EC2 only, install agent and find vulnerabilities

- Config: Track config changes and compliance against rules
- Macie: Find sensitive data (ex: PII data) in Amazon S3 buckets
- CloudTrail: Track API calls made by users within account
- AWS Security Hub: gather security findings from multiple AWS accounts
- Amazon Detective: find the root cause of security issues or suspicious activities
- AWS Abuse: Report AWS resources used for abusive or illegal purposes
- Root user privileges:
    - Change account settings
    - Close your AWS account
    - Change or cancel your AWS Support plan
    - Register as a seller in the Reserved Instance Marketplace


## Next Steps


 - Machine Learning


## Date 


- March 16-17, 2023

