# AWS Outposts, AWS WaveLength, AWS Local Zones, Global Applications in AWS - Summary


## Introduction


- AWS Outposts
- AWS WaveLength
- AWS Local Zones
- Global Applications in AWS - Summary


## Cloud Research


### #1. AWS Outposts


- Benefits:
- Low-latency access to on-premises systems
- Local data processing
- Data residency
- Easier migration from on-premises to the cloud
- Fully managed service
- Some services that work on Outposts:
    - Amazon EC2, EBS, S3, EKS, ECS, RDS, EMR.

### #2. AWS WaveLength


- WaveLength Zones are infrastructure deployments embedded within the telecommunications providers’ datacenters at the edge of the 5G networks
- Brings AWS services to the edge of the 5G networks
- Example: EC2, EBS, VPC…
- Ultra-low latency applications through 5G networks
- Traffic doesn’t leave the Communication Service Provider’s (CSP) network
- High-bandwidth and secure connection to the parent AWS Region
- No additional charges or service agreements
- Use cases: Smart Cities, ML-assisted diagnostics, Connected Vehicles, Interactive Live Video Streams, AR/VR, Real-time Gaming, …


### #3. AWS Local Zones


- Places AWS compute, storage, database, and other selected AWS services closer to end users to run latency-sensitive applications
- Extend your VPC to more locations – “Extension of an AWS Region”
- Compatible with EC2, RDS, ECS, EBS, ElastiCache, Direct Connect …
- Example:
    - AWS Region: N. Virginia (us-east-1)
    - AWS Local Zones: Boston, Chicago, Dallas, Houston, Miami, …


### #4. Global Applications in AWS - Summary


- Global DNS: Route 53
    - Great to route users to the closest deployment with least latency
    - Great for disaster recovery strategies
- Global Content Delivery Network (CDN): CloudFront
    - Replicate part of your application to AWS Edge Locations – decrease latency
    - Cache common requests – improved user experience and decreased latency
- S3 Transfer Acceleration
    - Accelerate global uploads & downloads into Amazon S3
- AWS Global Accelerator
    - Improve global application availability and performance using the AWS global network

- AWS Outposts
    - Deploy Outposts Racks in your own Data Centers to extend AWS services
- AWS WaveLength
    - Brings AWS services to the edge of the 5G networks
    - Ultra-low latency applications
- AWS Local Zones
    - Bring AWS resources (compute, database, storage, …) closer to your users
    - Good for latency-sensitive applications


## Next Steps


- Cloud Integration (Part 1)


## Date


- 17.2.2023
