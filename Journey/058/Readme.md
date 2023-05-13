# Other AWS Services Part 2


## Introduction


- Amazon Elastic Transcoder
- AWS AppSync
- AWS Amplify
- AWS Device Farm
- AWS Backup
- AWS Elastic Disaster Recovery (DRS)
- AWS DataSync


## Cloud Research


### #1. Amazon Elastic Transcoder


- Elastic Transcoder is used to convert media files stored in S3 into media files in the formats required by consumer playback devices (phones etc..)
- Benefits:
    - Easy to use
    - Highly scalable – can handle large volumes of media files and large file sizes
    - Cost effective – duration-based pricing model
    - Fully managed & secure, pay for what you use


### #2. AWS AppSync


- Store and sync data across mobile and web apps in real-time
- Makes use of GraphQL (mobile technology from Facebook)
- Client Code can be generated automatically
- Integrations with DynamoDB / Lambda
- Real-time subscriptions
- Offline data synchronization (replaces Cognito Sync)
- Fine Grained Security
- AWS Amplify can leverage AWS AppSync in the background!


### #3. AWS Amplify


- A set of tools and services that helps you develop and deploy scalable full stack web and mobile applications
- Authentication, Storage, API (REST, GraphQL), CI/CD, PubSub, Analytics, AI/ML Predictions, Monitoring, Source Code from AWS, GitHub, etc…


### #4. AWS Device Farm


- Fully-managed service that tests your web and mobile apps against desktop browsers, real mobile devices, and tablets
- Run tests concurrently on multiple devices (speed up execution)
- Ability to configure device settings (GPS, language, Wi-Fi, Bluetooth, …)


### #5. AWS Backup


- Fully-managed service to centrally manage and automate backups across AWS services
- On-demand and scheduled backups
- Supports PITR (Point-in-time Recovery)
- Retention Periods, Lifecycle Management, Backup Policies, …
- Cross-Region Backup
- Cross-Account Backup (using AWS Organizations)


### #6. AWS Elastic Disaster Recovery (DRS)


- Used to be named “CloudEndure Disaster Recovery”

- Quickly and easily recover your physical, virtual, and cloud-based servers into AWS
- Example: protect your most critical databases (including Oracle, MySQL, and SQL Server), enterprise apps (SAP), protect your data from ransomware attacks, …
- Continuous block-level replication for your servers


### #7. AWS DataSync


- Move large amount of data from on-premises to AWS
- Can synchronize to: Amazon S3 (any storage classes – including Glacier), Amazon EFS, Amazon FSx for Windows

- Replication tasks can be scheduled hourly, daily, weekly
- The replication tasks are incremental after the first full load


## Next Steps


- Other AWS Services Part 3

