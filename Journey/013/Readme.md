#  EC2 Instance Purchasing Options & Shared Responsibility Model for EC2 & EC2 Section – Summary

## Introduction

- EC2 Instances Purchasing Options
- EC2 On Demand 
- EC2 Reserved Instances 
- EC2 Savings Plans 
- EC2 Spot Instances
- EC2 Dedicated Hosts 
- EC2 Dedicated Instances 
- EC2 Capacity Reservations 
- Which purchasing option is right for me?
- Shared Responsibility Model for EC2
- EC2 Section – Summary 


## Cloud Research

### 1. EC2 Instances Purchasing Options

- On-Demand Instances – short workload, predictable pricing, pay by second<br>
- Reserved (1 & 3 years)<br>
    - Reserved Instances – long workloads
    - Convertible Reserved Instances – long workloads with flexible instances
- Savings Plans (1 & 3 years) –commitment to an amount of usage, long workload<br>
- Spot Instances – short workloads, cheap, can lose instances (less reliable)<br>
- Dedicated Hosts – book an entire physical server, control instance placement<br> 
- Dedicated Instances – no other customers will share your hardware<br> 
- Capacity Reservations – reserve capacity in a specific AZ for any duration<br> 


### 2. EC2 On Demand 

- Pay for what you use:<br> 
    - Linux or Windows - billing per second, after the first minute 
    - All other operating systems - billing per hour 
- Has the highest cost but no upfront payment • No long-term commitment<br> 
- Recommended for short-term and un-interrupted workloads, where you can't predict how the application will behave

### 3. EC2 Reserved Instances 

- Up to 72% discount compared to On-demand<br>
- You reserve a specific instance attributes (Instance Type, Region, Tenancy, OS)<br>
- Reservation Period – 1 year (+discount) or 3 years (+++discount)<br>
- Payment Options – No Upfront (+), Partial Upfront (++), All Upfront (+++)<br> 
- Reserved Instance’s Scope – Regional or Zonal (reserve capacity in an AZ)<br>
- Recommended for steady-state usage applications (think database)<br>
- You can buy and sell in the Reserved Instance Marketplace<br> 
- Convertible Reserved Instance<br> 
    - Can change the EC2 instance type, instance family, OS, scope and tenancy
    - Up to 66% discount 
    
    
### 4. EC2 Savings Plans

- Get a discount based on long-term usage (up to 72% - same as RIs)<br>  
- Commit to a certain type of usage ($10/hour for 1 or 3 years)<br>  
- Usage beyond EC2 Savings Plans is billed at the On-Demand price
- Locked to a specific instance family & AWS region (e.g., M5 in us-east-1)<br>  
- Flexible across:<br>
    - Instance Size (e.g., m5.xlarge, m5.2xlarge)
    - OS (e.g., Linux, Windows) 
    - Tenancy (Host, Dedicated, Default)
    

### 5. EC2 Spot Instances

- Can get a discount of up to 90% compared to On-demand<br> 
- Instances that you can “lose” at any point of time if your max price is less than the current spot price<br> 
- The MOST cost-efficient instances in AWS

- Useful for workloads that are resilient to failure
    - Batch jobs
    - Data analysis
    - Image processing
    - Any distributed workloads 
    - Workloads with a flexible start and end time
- Not suitable for critical jobs or databases


### 6. EC2 Dedicated Hosts 

- A physical server with EC2 instance capacity fully dedicated to your use
- Allows you address compliance requirements and use your existing server- bound software licenses (per-socket, per-core, pe—VM software licenses) 
- Purchasing Options: 
    - On-demand – pay per second for active Dedicated Host 
    - Reserved - 1 or 3 years (No Upfront, Partial Upfront, All Upfront) 
- The most expensive option 
- Useful for software that have complicated licensing model (BYOL – Bring Your Own License) 
- Or for companies that have strong regulatory or compliance needs


### 7. EC2 Dedicated Instances 

- Instances run on hardware that’s dedicated to you 

- May share hardware with other instances in same account 

- No control over instance placement (can move hardware after Stop / Start)


### 8. EC2 Capacity Reservations 

- Reserve On-Demand instances capacity in a specific AZ for any duration 
- You always have access to EC2 capacity when you need it 
- No time commitment (create/cancel anytime), no billing discounts 
- Combine with Regional Reserved Instances and Savings Plans to benefit from billing discounts 
- You’re charged at On-Demand rate whether you run instances or not 
- Suitable for short-term, uninterrupted workloads that needs to be in a specific AZ


### 9. Which purchasing option is right for me?

- On demand      : coming and staying in resort whenever we like, we pay the full price
- Reserved       : like planning ahead and if we plan to stay for a long time, we may get a good discount.
- Savings Plans  : pay a certain amount per hour for certain period and stay in any room type (e.g.,
King, Suite, Sea View, …)
- Spot instances : the hotel allows people to bid for the empty rooms and the highest bidder keeps the
rooms. You can get kicked out at any time
- Dedicated Hosts: We book an entire building of the resort
- Capacity Reservations: you book a room for a period with full price even you don’t stay in it


### 10. Shared Responsibility Model for EC2

![image](https://user-images.githubusercontent.com/121140952/214017277-ea415bc6-0c2e-4de1-bf69-519e8f3c197b.png)

- Infrastructure (global network security)
- Isolation on physical hosts
- Replacing faulty hardware
- Compliance validation


![image](https://user-images.githubusercontent.com/121140952/214017339-bbdfef39-30ff-4ba3-a267-0db89c118516.png)

- Security Groups rules
- Operating-system patches and updates
- Software and utilities installed on the EC2 instance
- IAM Roles assigned to EC2 & IAM user access management
- Data security on your instance

### 11. EC2 Section – Summary 

- EC2 Instance: AMI (OS) + Instance Size (CPU + RAM) + Storage +
security groups + EC2 User Data
- Security Groups: Firewall attached to the EC2 instance
- EC2 User Data: Script launched at the first start of an instance
- SSH: start a terminal into our EC2 Instances (port 22)
- EC2 Instance Role: link to IAM roles
- Purchasing Options: On-Demand, Spot, Reserved (Standard +
Convertible + Scheduled), Dedicated Host, Dedicated Instance


## Next Steps

EC2 Instance Storage Section

## Social Proof
https://cahbitaran.blogspot.com/
