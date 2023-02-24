# Cloud Monitoring Part 3


## Introduction


- Amazon CodeGuru
- Amazon CodeGuru Reviewer
- Amazon CodeGuru Profiler
- AWS Health Dashboard
- Monitoring Summary


## Cloud Research


### #1. Amazon CodeGuru


- An ML-powered service for automated code reviews and application performance recommendations
- Provides two functionalities
    - CodeGuru Reviewer: automated code reviews for static code analysis (development)
    - CodeGuru Profiler: visibility/recommendations about application performance during runtime (production)


### #2. Amazon CodeGuru Reviewer


- Identify critical issues, security vulnerabilities, and hard-to-find bugs
- Example: common coding best practices, resource leaks, security detection, input validation
- Uses Machine Learning and automated reasoning
- Hard-learned lessons across millions of code reviews on 1000s of open-source and Amazon repositories
- Supports Java and Python
- Integrates with GitHub, Bitbucket, and AWS CodeCommit


### #3. Amazon CodeGuru Profiler


- Helps understand the runtime behavior of your application
- Example: identify if your application is consuming excessive CPU capacity on a logging routine
- Features:
    - Identify and remove code inefficiencies
    - Improve application performance (e.g., reduce CPU utilization)
    - Decrease compute costs
    - Provides heap summary (identify which objects using up memory)
    - Anomaly Detection
- Support applications running on AWS or on- premise
- Minimal overhead on application


### #4. AWS Health Dashboard


#### #A. Service History


- Shows all regions, all services health
- Shows historical information for each day
- Has an RSS feed you can subscribe to
- Previously called AWS Service Health Dashboard


#### #B. Your Account


- Global service
- Shows how AWS outages directly impact you & your AWS resources
- Alert, remediation, proactive, scheduled activities


### #4. Monitoring Summary


- CloudWatch:
    - Metrics: monitor the performance of AWS services and billing metrics  
    - Alarms: automate notification, perform EC2 action, notify to SNS based on metric
    - Logs: collect log files from EC2 instances, servers, Lambda functions…
    - Events (or EventBridge): react to events in AWS, or trigger a rule on a schedule
- CloudTrail: audit API calls made within your AWS account
- CloudTrail Insights: automated analysis of your CloudTrail Events
- X-Ray: trace requests made through your distributed applications
- Service Health Dashboard: status of all AWS services across all regions
- Personal Health Dashboard: AWS events that impact your infrastructure
- Amazon CodeGuru: automated code reviews and application performance recommendations


## Next Steps


- VPC

