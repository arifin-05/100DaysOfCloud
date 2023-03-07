# Security & Compliance


## Introduction


- DDOS Protection on AWS
- AWS Shield
- AWS WAF – Web Application Firewall
- Penetration Testing on AWS Cloud
- Data at rest vs. Data in transit
- AWS KMS (Key Management Service)


## Cloud Research


### #1. DDOS Protection on AWS


- AWS Shield Standard: protects against DDOS attack for your website and applications, for all customers at no additional costs
- AWS Shield Advanced: 24/7 premium DDoS protection
- AWS WAF: Filter specific requests based on rules
- CloudFront and Route 53:
    - Availability protection using global edge network
    - Combined with AWS Shield, provides attack mitigation at the edge

- Be ready to scale – leverage AWS Auto Scaling


### #2. AWS Shield


- AWS Shield Standard:
    - Free service that is activated for every AWS customer
    - Provides protection from attacks such as SYN/UDP Floods, Reflection attacks and other layer 3/layer 4 attacks
- AWS Shield Advanced:
    - Optional DDoS mitigation service ($3,000 per month per organization)
    - Protect against more sophisticated attack on Amazon EC2, Elastic Load Balancing (ELB), Amazon CloudFront, AWS Global Accelerator, and Route 53
    - 24/7 access to AWS DDoS response team (DRP)
    - Protect against higher fees during usage spikes due to DDoS


### #3. AWS WAF – Web Application Firewall


- Protects your web applications from common web exploits (Layer 7)
- Layer 7 is HTTP (vs Layer 4 is TCP)
- Deploy on Application Load Balancer, API Gateway, CloudFront

- Define Web ACL (Web Access Control List):
    - Rules can include IP addresses, HTTP headers, HTTP body, or URI strings
    - Protects from common attack - SQL injection and Cross-Site Scripting (XSS)
    - Size constraints, geo-match (block countries)
    - Rate-based rules (to count occurrences of events) – for DDoS protection


### #4. Penetration Testing on AWS Cloud


- AWS customers are welcome to carry out security assessments or penetration tests against their AWS infrastructure without prior approval for 8 services:
    - Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers
    - Amazon RDS
    - Amazon CloudFront
    - Amazon Aurora
    - Amazon API Gateways
    - AWS Lambda and Lambda Edge functions
    - Amazon Lightsail resources
    - Amazon Elastic Beanstalk environments
- List can increase over time (you won’t be tested on that at the exam)

- Prohibited Activities
    - DNS zone walking via Amazon Route 53 Hosted Zones
    - Denial of Service (DoS), Distributed Denial of Service (DDoS), Simulated DoS, Simulated DDoS
    - Port flooding
    - Protocol flooding
    - Request flooding (login request flooding, API request flooding)
- For any other simulated events, contact aws-security-simulatedevent@amazon.com
- Read more: https://aws.amazon.com/security/penetration-testing/


### #5. Data at rest vs. Data in transit


- At rest: data stored or archived on a device
    - On a hard disk, on a RDS instance, in S3 Glacier Deep Archive, etc.
- In transit (in motion): data being moved from one location to another
    - Transfer from on-premises to AWS, EC2 to DynamoDB, etc.
    - Means data transferred on the network
- We want to encrypt data in both states to protect it!
- For this we leverage encryption keys


### #6. AWS KMS (Key Management Service)


- Anytime you hear “encryption” for an AWS service, it’s most likely KMS
- KMS = AWS manages the encryption keys for us
- Encryption Opt-in:
    - EBS volumes: encrypt volumes
    - S3 buckets: Server-side encryption of objects
    - Redshift database: encryption of data
    - RDS database: encryption of data
    - EFS drives: encryption of data
- Encryption Automatically enabled:
    - CloudTrail Logs
    - S3 Glacier
    - Storage Gateway


## Next Steps


-  Security & Compliance Part 1


## Date


- March 7, 2023

