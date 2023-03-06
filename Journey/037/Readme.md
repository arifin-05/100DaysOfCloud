# VPC Part 3


## Introduction


- Site-to-Site VPN
- AWS Client VPN
- Transit Gateway
- VPC Closing Comments


## Cloud Research


### #1. Site-to-Site VPN


• On-premises: must use a Customer Gateway (CGW)
• AWS: must use a Virtual Private Gateway (VGW)


### #2. AWS Client VPN


• Connect from your computer using OpenVPN to your private network in AWS and on-premises
• Allow you to connect to your EC2 instances over a private IP (just as if you were in the private VPC network)
• Goes over public Internet


### #3. Transit Gateway


• For having transitive peering between thousands of VPC and on -premises, hub-and-spoke (star) connection
• One single Gateway to provide this functionality
• Works with Direct Connect Gateway, VPN connections


### #4. VPC Closing Comments



• VPC: Virtual Private Cloud
• Subnets:Tied to an AZ, network partition of the VPC
• Internet Gateway: at the VPC level, provide Internet Access
• NAT Gateway / Instances: give internet access to private subnets
• NACL: Stateless, subnet rules for inbound and outbound
• Security Groups: Stateful, operate at the EC2 instance level or ENI
• VPC Peering: Connect two VPC with non overlapping IP ranges, nontransitive
• VPC Endpoints: Provide private access to AWS Services within VPC
• PrivateLink: Privately connect to a service in a 3rd party VPC
• VPC Flow Logs: network traffic logs
• Site to Site VPN: VPN over public internet between on-premises DC and AWS
• Client VPN: OpenVPN connection from your computer into your VPC
• Direct Connect: direct private connection to AWS
• Transit Gateway: Connect thousands of VPC and on-premises networks together


## Next Steps


- Security & Compliance


## Date


- March 6, 2023

