# AMAZON S3 (Part 2)



## Introduction


- S3 Storage Classes
- S3 Durability and Availability
- S3 Standard – General Purpose
- S3 Storage Classes – Infrequent Access
- Amazon S3 Glacier Storage Classes
- S3 Intelligent-Tiering
- Amazon S3 – Summary


## CLOUD RESEARCH

### #1. S3 Storage Classes


- Amazon S3 Standard - General Purpose
- Amazon S3 Standard-Infrequent Access (IA)
- Amazon S3 One Zone-Infrequent Access
- Amazon S3 Glacier Instant Retrieval
- Amazon S3 Glacier Flexible Retrieval
- Amazon S3 Glacier Deep Archive
- Amazon S3 Intelligent Tiering

- Can move between classes manually or using S3 Lifecycle configurations


### #2. S3 Durability and Availability


- Durability:
    - High durability (99.999999999%, 11 9’s) of objects across multiple AZ
    - If you store 10,000,000 objects with Amazon S3, you can on average expect to incur a loss of a single object once every 10,000 years
    - Same for all storage classes
    
- Availability:
    - Measures how readily available a service is
    - Varies depending on storage class
    - Example: S3 standard has 99.99% availability = not available 53 minutes a year


### #3. S3 Standard – General Purpose


- 99.99% Availability
- Used for frequently accessed data
- Low latency and high throughput
- Sustain 2 concurrent facility failures

- Use Cases: Big Data analytics, mobile & gaming applications, content distribution…


### #4. S3 Storage Classes – Infrequent Access


- For data that is less frequently accessed, but requires rapid access when needed
- Lower cost than S3 Standard

-  Amazon S3 Standard-Infrequent Access (S3 Standard-IA)
    - 99.9% Availability
    - Use cases: Disaster Recovery, backups

- Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA)
    - High durability (99.999999999%) in a single AZ; data lost when AZ is destroyed
    - 99.5% Availability  
    - Use Cases: Storing secondary backup copies of on-premise data, or data you can recreate


### #5. Amazon S3 Glacier Storage Classes



### #6. S3 Intelligent-Tiering

### #7. Amazon S3 – Summary



## Next Steps


- Databases & Analystics

## Date

- January 27, 2023


