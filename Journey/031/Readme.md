# Cloud Monitoring


## Introduction


- Amazon CloudWatch Metrics
- Important Metrics 
- Amazon CloudWatch Alarms
- Amazon CloudWatch Logs
- CloudWatch Logs for EC2


## Cloud Research


### #1. Amazon CloudWatch Metrics


- CloudWatch provides metrics for every services in AWS
- Metric is a variable to monitor (CPUUtilization, NetworkIn…)
- Metrics have timestamps
- Can create CloudWatch dashboards of metrics


### #2. Important Metrics 


- EC2 instances: CPU Utilization, Status Checks, Network (not RAM)
    - Default metrics every 5 minutes
    - Option for Detailed Monitoring ($$$): metrics every 1 minute
- EBS volumes: Disk Read/Writes
- S3 buckets: BucketSizeBytes, NumberOfObjects, AllRequests
- Billing:Total Estimated Charge (only in us-east-1)
- Service Limits: how much you’ve been using a service API
- Custom metrics: push your own metrics


### #3. Amazon CloudWatch Alarms


- Alarms are used to trigger notifications for any metric
- Alarms actions…
    - Auto Scaling: increase or decrease EC2 instances “desired” count
    - EC2 Actions: stop, terminate, reboot or recover an EC2 instance
    - SNS notifications: send a notification into an SNS topic
- Various options (sampling, %, max, min, etc…)
- Can choose the period on which to evaluate an alarm
- Example: create a billing alarm on the CloudWatch Billing metric
- Alarm States: OK. INSUFFICIENT_DATA, ALARM


### #4. Amazon CloudWatch Logs


- CloudWatch Logs can collect log from:
    - Elastic Beanstalk: collection of logs from application
    - ECS: collection from containers
    - AWS Lambda: collection from function logs
    - CloudTrail based on filter
    - CloudWatch log agents: on EC2 machines or on-premises servers
    - Route53: Log DNS queries

- Enables real-time monitoring of logs
- Adjustable CloudWatch Logs retention


### #5. CloudWatch Logs for EC2


- By default, no logs from your EC2 instance will go to CloudWatch
- You need to run a CloudWatch agent on EC2 to push the log files you want
- Make sure IAM permissions are correct
- The CloudWatch log agent can be setup on-premises too


![image](https://user-images.githubusercontent.com/121140952/220506930-5c238e19-8bde-48c1-a6b1-944d6073e4bf.png)


## Next Steps


- AWS CloudTrail,  AWS X-Ray, AWS X Ray advantages, Amazon CodeGuru.


## Date


- February 22, 2023.

