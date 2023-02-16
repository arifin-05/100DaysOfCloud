# Global Infrastructure (Part 2)


## Introduction


- AWS Global Accelerator
- AWS Global Accelerator vs CloudFront
- AWS Outposts


## Cloud Research


### #1. AWS Global Accelerator


- Improve global application availability and performance using the AWS global network
- Leverage the AWS internal network to optimize the route to your application (60% improvement)
- 2 Anycast IP are created for your application and traffic is sent through Edge Locations
- The Edge locations send the traffic to your application


### #2. AWS Global Accelerator vs CloudFront


- They both use the AWS global network and its edge locations around the world
- Both services integrate with AWS Shield for DDoS protection.
- CloudFront – Content Delivery Network
    - Improves performance for your cacheable content (such as images and videos)
    - Content is served at the edge

- Global Accelerator
    - No caching, proxying packets at the edge to applications running in one or more AWS Regions.
    - Improves performance for a wide range of applications over TCP or UDP
    - Good for HTTP use cases that require static IP addresses
    - Good for HTTP use cases that required deterministic, fast regional failover


### #3. AWS Outposts


- Hybrid Cloud: businesses that keep an on
- premises infrastructure alongside a cloud infrastructure
    - Therefore, two ways of dealing with IT systems:
    - One for the AWS cloud (using the AWS console, CLI, and AWS APIs)
- One for their on-premises infrastructure
- AWS Outposts are “server racks” that offers the same AWS infrastructure, services, APIs & tools to build your own applications on-premises just as in the cloud
- AWS will setup and manage “Outposts Racks” within your on-premises infrastructure and you can start leveraging AWS services on-premises
- You are responsible for the Outposts Rack physical security


### #4. AWS Outposts


- Benefits:
    - Low-latency access to on-premises systems
    - Local data processing
    - Data residency
    - Easier migration from on-premises to the cloud
    - Fully managed service
- Some services that work on Outposts:


## Next Steps

- Meet 3 | Setting Adapter, IP Address, Hostname, Host.

## Date

- February 16, 2023
