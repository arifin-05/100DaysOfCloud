# Cloud Monitoring (Part 1)


## Introduction


- Amazon EventBridge Rules
- Amazon EventBridge
- AWS CloudTrail
- AWS X-Ray
- AWS X Ray advantages


## Cloud Research


### #1. Amazon EventBridge Rules


![image](https://user-images.githubusercontent.com/121140952/220841259-91bf696b-aafb-499b-9697-8e9d0a510c03.png)


### #2. Amazon EventBridge


- Schema Registry: model event schema
- You can archive events (all/filter) sent to an event bus (indefinitely or set period)
- Ability to replay archived events


### #3.  AWS CloudTrail


- Provides governance, compliance and audit for your AWS Account
- CloudTrail is enabled by default!
- Get an history of events / API calls made within your AWS Account by:
    - Console
    - SDK
    - CLI
    - AWS Services
- Can put logs from CloudTrail into CloudWatch Logs or S3
- A trail can be applied to All Regions (default) or a single Region.
- If a resource is deleted in AWS, investigate CloudTrail first!


### #4. AWS X-Ray 


- Debugging in Production, the good old way:
    - Test locally
    - Add log statements everywhere
    - Re-deploy in production
- Log formats differ across applications and log analysis is hard.
- Debugging: one big monolith “easy”, distributed services “hard”
- No common views of your entire architecture

- Enter… AWS X-Ray!


### #5. AWS X Ray advantages


- Troubleshooting performance (bottlenecks)
- Understand dependencies in a microservice architecture
- Pinpoint service issues
- Review request behavior
- Find errors and exceptions
- Are we meeting time SLA?
- Where I am throttled?
- Identify users that are impacted 


## Next Steps


- Cloud Monitoring (Part 3)


## Date


- February 23, 2023

