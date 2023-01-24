# (EC2 Instance Storage Part 1)


## Introduction

- What’s an EBS Volume?
- EBS Volume
- EBS Volume- Example
- EBS – Delete on Termination attribute
- EBS Snapshots
- EBS Snapshots Features

- AMI Overview
- AMI Process (from an EC2 instance)
- EC2 Image Builder
- EC2 Instance Store


## Cloud Research


### What’s an EBS Volume?

- An EBS (Elastic Block Store) Volume is a network drive you can attach to your instances while they run
- It allows your instances to persist data, even after their termination
- They can only be mounted to one instance at a time (at the CCP level)
- They are bound to a specific availability zone

- Analogy: Think of them as a “network USB stick”
- Free tier: 30 GB of free EBS storage of type General Purpose (SSD) or Magnetic per month


### EBS Volume

- It’s a network drive (i.e. not a physical drive)
  - It uses the network to communicate the instance, which means there might be a bit of latency
  - It can be detached from an EC2 instance and attached to another one quickly
- It’s locked to an Availability Zone (AZ) 
  - An EBS Volume in us-east-1a cannot be attached to us east-1b
  - To move a volume across, you first need to snapshot it
-  Have a provisioned capacity (size in GBs, and IOPS)
  -  You get billed for all the provisioned capacity
  - You can increase the capacity of the drive over tim


### EBS Volume- Example

- US -EAST-1A

![image](https://user-images.githubusercontent.com/121140952/214186924-dbbbc0eb-6062-4f60-91d8-768ac27bb031.png)

- US -EAST-1B

![image](https://user-images.githubusercontent.com/121140952/214187015-547604a8-b202-4ef5-8593-680443cf1497.png)


### EBS – Delete on Termination attribute

![image](https://user-images.githubusercontent.com/121140952/214187223-95a2eb7d-d456-4de7-8789-5966651c4dba.png)

- Controls the EBS behaviour when an EC2 instance terminates 
  - By default, the root EBS volume is deleted (attribute enabled) 
  - By default, any other attached EBS volume is not deleted (attribute disabled) 
- This can be controlled by the AWS console / AWS CLI 
- Use case: preserve root volume when instance is terminated EBS Snapshots 


### EBS Snapshots

- Make a backup (snapshot) of your EBS volume at a point in time 
- Not necessary to detach volume to do snapshot, but recommended 
- Can copy snapshots across AZ or Region

### EBS Snapshots Features

- EBS Snapshot Archive
  - Move a Snapshot to an ”archive tier” that is 75% cheaper
  - Takes within 24 to 72 hours for restoring the archive
- Recycle Bin for EBS Snapshots
  - Setup rules to retain deleted snapshots so you can recover them after an accidental deletion
  - Specify retention (from 1 day to 1 year)


### AMI Overview

- AMI = Amazon Machine Image
- AMI are a customization of an EC2 instance
  - You add your own software, configuration, operating system, monitoring…
  - Faster boot / configuration time because all your software is pre-packaged
- AMI are built for a specific region (and can be copied across regions)
- You can launch EC2 instances from:
  - A Public AMI: AWS provided
  - Your own AMI: you make and maintain them yourself
  - An AWS Marketplace AMI: an AMI someone else made (and potentially sells)


### AMI Process (from an EC2 instance)

- Start an EC2 instance and customize it
- Stop the instance (for data integrity)
- Build an AMI – this will also create EBS snapshots
- Launch instances from other AMIs


### EC2 Image Builder

- Used to automate the creation of Virtual Machines or container images
- => Automate the creation, maintain, validate and test EC2 AMIs
- Can be run on a schedule (weekly, whenever packages are updated, etc…)
- Free service (only pay for the underlying resources)


### EC2 Instance Store

- EBS volumes are network drives with good but “limited” performance
- If you need a high-performance hardware disk, use EC2 Instance Store

- Better I/O performance
- EC2 Instance Store lose their storage if they’re stopped (ephemeral)
- Good for buffer / cache / scratch data / temporary content
- Risk of data loss if hardware fails
- Backups and Replication are your responsibility 


## Next Steps

(EC2 Instance Storage Part 1)


## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)

## Date

- January 24, 2023
