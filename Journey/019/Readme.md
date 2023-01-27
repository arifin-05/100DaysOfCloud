# Databases & Analytics (Part 1)


## Introduction


- Databases Intro
- Relational Databases
- NoSQL Databases
- Databases & Shared Responsibility on AWS
- AWS RDS Overview
- Advantage over using RDS versus deploying DB on EC2
- Amazon Aurora
- Amazon ElastiCache Overview


## Cloud Research


### #1. Databases Intro


- Storing data on disk (EFS, EBS, EC2 Instance Store, S3) can have its limits
- Sometimes, you want to store data in a database…
- You can structure the data
- You build indexes to efficiently query / search through the data
- You define relationships between your datasets

- Databases are optimized for a purpose and come with different features, shapes and constraints


### #2. Rational Databases


- Looks just like Excel spreadsheets, with links between them!
- Can use the SQL language to perform queries / lookups


### #3. NoSQL Databases


- NoSQL = non-SQL = non relational databases
- NoSQL databases are purpose built for specific data models and have flexible schemas for building modern applications.
- Benefits:
    - Flexibility: easy to evolve data model
    - Scalability: designed to scale-out by using distributed clusters
    - High-performance: optimized for a specific data model
    - Highly functional: types optimized for the data model

- Examples: Key-value, document, graph, in-memory, search databases


### #4. Databases & Shared Responsibility on AWS


- AWS offers use to manage different databases
- Benefits include:
    - Quick Provisioning, High Availability, Vertical and Horizontal Scaling
    - Automated Backup & Restore, Operations, Upgrades
    - Operating System Patching is handled by AWS
    - Monitoring, alerting
    
- Note: many databases technologies could be run on EC2, but you must
handle yourself the resiliency, backup, patching, high availability, fault tolerance, scaling… 


### #5. AWS RDS Overview


- RDS stands for Relational Database Service
- It’s a managed DB service for DB use SQL as a query language.
- It allows you to create databases in the cloud that are managed by AWS
    - Postgres
    - MySQL
    - MariaDB
    - Oracle
    - Microsoft SQL Server
    - Aurora (AWS Proprietary database)


### #6. Advantage over using RDS versus deploying DB on EC2


- RDS is a managed service:
    - Automated provisioning, OS patching
    - Continuous backups and restore to specific timestamp (Point in Time Restore)!
    - Monitoring dashboards
    - Read replicas for improved read performance
    - Multi AZ setup for DR (Disaster Recovery)
    - Maintenance windows for upgrades
    - Scaling capability (vertical and horizontal)
    - Storage backed by EBS (gp2 or io1)
- BUT you can’t SSH into your instances


### #7. Amazon Aurora


- Aurora is a proprietary technology from AWS (not open sourced)
- PostgreSQL and MySQL are both supported as Aurora DB
- Aurora is “AWS cloud optimized” and claims 5x performance improvement over MySQL on RDS, over 3x the performance of Postgres on RDS
- Aurora storage automatically grows in increments of 10GB, up to 64 TB.
- Aurora costs more than RDS (20% more) – but is more efficient
- Not in the free tier


### #8. Amazon ElastiCache Overview


- The same way RDS is to get managed Relational Databases…
- ElastiCache is to get managed Redis or Memcached
- Caches are in-memory databases with high performance, low latency
- Helps reduce load off databases for read intensive workloads

- AWS takes care of OS maintenance / patching, optimizations, setup, configuration, monitoring, failure recovery and backups


## Next Steps

- Databases & Analytics (Part 2)

## Date

- January 28, 2023
