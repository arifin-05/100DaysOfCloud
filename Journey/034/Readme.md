
# VPC


## Introduction


- VPC & Subnets Primer
- Internet Gateway & NAT Gateways
- Network ACL & Security Groups
- Network ACLs vs Security Groups


## Cloud Research


### #1. VPC & Subnets Primer


- VPC -Virtual Private Cloud: private network to deploy your resources (regional resource)
- Subnets allow you to partition your network inside your VPC (Availability Zone resource)
- A public subnet is a subnet that is accessible from the internet
- A private subnet is a subnet that is not accessible from the internet
- To define access to the internet and between subnets, we use Route Tables.


### #2. Internet Gateway & NAT Gateways


- Internet Gateways helps our VPC instances connect with the internet
- Public Subnets have a route to the internet gateway.

- NAT Gateways (AWS-managed) & NAT Instances (self-managed) allow your instances in your Private Subnets to access the internet while remaining private.


### #3. Network ACL & Security Groups


- NACL (Network ACL)
    - A firewall which controls traffic from and to subnet
    - Can have ALLOW and DENY rules
    - Are attached at the Subnet level
    - Rules only include IP addresses

- Security Groups
    - A firewall that controls traffic to and from an ENI / an EC2 Instance
    - Can have only ALLOW rules
    - Rules include IP addresses and other security groups


### #4. Network ACLs vs Security Groups

##### Security Group

- Operates at the instance level
- Supports allow rules only
- Is stateful: Return traffic is automatically allowed, regardless of any rules 
- We evaluate all rules before deciding whether to allow traffic 
- Applies to an instance only if someone specifies the security group when launching the instance, or associates the security group with the instance later on


##### Network ACL

- Operates at the subnet level
- Supports allow rules and deny rules
- Is stateless: Return traffic must be explicitly allowed by rules
- We process rules in number order when deciding whether to allow traffic
- Automatically applies to all instances in the subnets it's associated with (therefore, you don't have to rely on users to specify the security group)


## Next Steps


- VPC Part 2 (VPC Flow Logs, VPC Peering, VPC Endpoints, AWS PrivateLink [VPC Endpoint Services]).


## Date


- February 27, 2023

