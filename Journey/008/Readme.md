
# Bascis EC2


## Cloud Research


### Amazon EC2

1. EC2 is one of the most popular of AWS' offering

2. EC2 = Elastic Compute Cloud Infrastructure as a Service

3. It mainly consists in the capability of:

    • Renting virtual machines (EC2)
    
    • Storing data on virtual drives (EBS)
    
    • Distributing load across machines (ELB)
    
    • Scaling the services using an auto-scaling group (ASG)

4. Knowing EC2 is fundamental to understand how the Cloud works


### EC2 sizing & configuration options

1. Operating System (OS): Linux, Windows or Mac OS

2. How much compute power & cores (CPU)

3. How much random-access memory (RAM)

4. How much storage space:
    
    • Network-attached (EBS & EFS)
    
    • hardware (EC2 Instance Store)

5. Network card: speed of the card, Public IP address

6. Firewall rules: security group

7. Bootstrap script (configure at first launch): EC2 User Data


### EC2 User Data

1. It is possible to bootstrap our instances using an EC2 User data script.

2. bootstrapping means launching commands when a machine starts

3. That script is only run once at the instance first start

4. EC2 user data is used to automate boot tasks such as:
    
    • Installing updates
    
    • Installing software
    
    • Downloading common files from the internet
    
    • Anything you can think of

5. The EC2 User Data Script runs with the root user


## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

https://cahblitaran.blogspot.com
