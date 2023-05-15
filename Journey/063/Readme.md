### #1. AWS Well-Architected Tool


- Free tool to review your architectures against the 6 pillars Well-Architected
Framework and adopt architectural best practices
- How does it work?
    - Select your workload and answer questions
    - Review your answers against the 6 pillars
    - Obtain advice: get videos and documentations, generate a report, see the results in a dashboard
- Let’s have a look: https://console.aws.amazon.com/wellarchitected


### #2.AWS Right Sizing


- EC2 has many instance types, but choosing the most powerful instance type isn’t the best choice, because the cloud is elastic
- Right sizing is the process of matching instance types and sizes to your workload performance and capacity requirements at the lowest possible cost
- Scaling up is easy so always start small
- It’s also the process of looking at deployed instances and identifying opportunities to eliminate or downsize without compromising capacity or other requirements, which results in lower costs
- It’s important to Right Size…
    - before a Cloud Migration
    - continuously after the cloud onboarding process (requirements change over time)
- CloudWatch, Cost Explorer, Trusted Advisor, 3rd party tools can help

### #3. AWS Ecosystem – Free resources


- AWS Blogs: https://aws.amazon.com/blogs/aws/
- AWS Forums (community): https://forums.aws.amazon.com/index.jspa
- AWS Whitepapers & Guides: https://aws.amazon.com/whitepapers
- AWS Quick Starts: https://aws.amazon.com/quickstart/
    - Automated, gold-standard deployments in the AWS Cloud
    - Build your production environment quickly with templates
    - Example: WordPress on AWS https://fwd.aws/P3yyv?did=qs_card&trk=qs_card
    - Leverages CloudFormation
- AWS Solutions: https://aws.amazon.com/solutions/
    - Vetted Technology Solutions for the AWS Cloud
    - Example - AWS Landing Zone: secure, multi-account AWS environment
          - https://aws.amazon.com/solutions/implementations/aws-landing-zone/
          - “Replaced” by AWS Control Tower

