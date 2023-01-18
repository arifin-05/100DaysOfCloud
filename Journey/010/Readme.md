

# Security Groups & Classic Ports Overview

## Introduction

- Introduction to Security Groups
- Security Groups Deeper Dive
- Security Groups Diagram
- Security groups Good to Know
- Referencing other security groups Diagram
- Classic Ports to know


## Cloud Research

### Introduction to Security Groups

- Security Groups are the fundamental of network security in AWS
- They control how traffic is allowed into or out of our EC2 Instances.
 
 ![image](https://user-images.githubusercontent.com/121140952/213086744-baf1f56e-bb53-41ff-aee5-9ad93869e35f.png)

 
- Security groups only contain allow rules 
- Security groups rules can reference by IP or by security group


### Security Groups Deeper Dive

- Security groups are acting as a "firewall" on EC2 instances<br>
- They regulate:
   - Access to Ports
   - Authorised IP ranges - IPv4 and IPv6
   - Control of inbound network (from other to the instance)
   - Control of outbound network (from the instance to other)
   - 

![image](https://user-images.githubusercontent.com/121140952/213087305-cf668264-aa00-4cfa-9db9-9b205c39473b.png)


### Security Groups Diagram

![image](https://user-images.githubusercontent.com/121140952/213087359-d000f95e-7f34-47a9-bd6f-48e58792c393.png)


### Security groups Good to Know

- Can be attached to multiple instances
- Locked down to a region /VPC combination
- Does live "outside" the EC2 - if traffic is blocked the EC2 instance won't see it
- It's good to maintain one separate security group for SSH access
- If your application is not accessible (time out), then it's a security group issue
- If your application gives a "connection refused" error, then it's an application error or it's not launched
- All inbound traffic is blocked by default
- All outbound traffic is authorised by default


### Referencing other security groups Diagram

![image](https://user-images.githubusercontent.com/121140952/213087749-856978f5-f0ea-4f3e-a537-a39e4bb319e1.png)


### Classic Ports to know

- 22 = SSH (Secure Shell) - log into a Linux instance
- 21 FTP (File Transfer Protocol) - upload files into a file share
- 22 = SFTP (Secure File Transfer Protocol) - upload files using SSH
- 80 HTTP access unsecured websites
- 443 = HTTPS - access secured websites
- 3389 = RDP (Remote Desktop Protocol) - log into a Windows instance


## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

https://cahblitaran.blogspot.com/
