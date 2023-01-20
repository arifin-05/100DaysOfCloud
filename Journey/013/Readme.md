#  EC2 Instance Purchasing Options

## Introduction

- EC2 Instances Purchasing Options
- EC2 On Demand 
- EC2 Reserved Instances 
- EC2 Savings Plans 
- EC2 Spot Instances


## Cloud Research

### 1. EC2 Instances Purchasing Options

• On-Demand Instances – short workload, predictable pricing, pay by second<br>
• Reserved (1 & 3 years)<br>

    • Reserved Instances – long workloads
    
    •Convertible Reserved Instances – long workloads with flexible instances
    
• Savings Plans (1 & 3 years) –commitment to an amount of usage, long workload<br>
• Spot Instances – short workloads, cheap, can lose instances (less reliable)<br>
• Dedicated Hosts – book an entire physical server, control instance placement<br> 
• Dedicated Instances – no other customers will share your hardware<br> 
• Capacity Reservations – reserve capacity in a specific AZ for any duration<br> 


### 2. EC2 On Demand 

• Pay for what you use:<br> 

    • Linux or Windows - billing per second, after the first minute 
    
    • All other operating systems - billing per hour 
    
• Has the highest cost but no upfront payment • No long-term commitment<br> 
• Recommended for short-term and un-interrupted workloads, where you can't predict how the application will behave

### 3. EC2 Reserved Instances 

• Up to 72% discount compared to On-demand<br>
• You reserve a specific instance attributes (Instance Type, Region, Tenancy, OS)<br>
• Reservation Period – 1 year (+discount) or 3 years (+++discount)<br>
• Payment Options – No Upfront (+), Partial Upfront (++), All Upfront (+++)<br> 
• Reserved Instance’s Scope – Regional or Zonal (reserve capacity in an AZ)<br>
• Recommended for steady-state usage applications (think database)<br>
• You can buy and sell in the Reserved Instance Marketplace<br> 
• Convertible Reserved Instance<br> 

    • Can change the EC2 instance type, instance family, OS, scope and tenancy
    
    • Up to 66% discount 
    
### 4. EC2 Savings Plans

• Get a discount based on long-term usage (up to 72% - same as RIs)<br>  
• Commit to a certain type of usage ($10/hour for 1 or 3 years)<br>  
• Usage beyond EC2 Savings Plans is billed at the On-Demand price
• Locked to a specific instance family & AWS region (e.g., M5 in us-east-1)<br>  
• Flexible across:<br>

    • Instance Size (e.g., m5.xlarge, m5.2xlarge)
    
    • OS (e.g., Linux, Windows) 
    
    • Tenancy (Host, Dedicated, Default)
    


### 5. EC2 Spot Instances

• Can get a discount of up to 90% compared to On-demand<br> 
• Instances that you can “lose” at any point of time if your max price is less than the current spot price<br> 
• The MOST cost-efficient instances in AWS

• Useful for workloads that are resilient to failure

    • Batch jobs
    
    • Data analysis
    
    • Image processing
    
    • Any distributed workloads
    
    • Workloads with a flexible start and end time

• Not suitable for critical jobs or databases


## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof
https://cahbitaran.blogspot.com/
