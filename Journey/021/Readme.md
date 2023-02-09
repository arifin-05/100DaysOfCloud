# Other Compute (Part 1)


## Introduction


- What is Docker?
- Where Docker images are stored?
- Docker versus Virtual Machines
- ECS
- Fargate
- ECR
- What’s serverless?
- Why AWS Lambda
- Benefits of AWS Lambda
- AWS Lambda language support


## Cloud Research


### #1. What is Docker?


- Docker is a software development platform to deploy apps
- Apps are packaged in containers that can be run on any OS
- Apps run the same, regardless of where they’re run
    - Any machine
    - No compatibility issues
    - Predictable behavior
    - Less work
    - Easier to maintain and deploy
    - Works with any language, any OS, any technology
- Scale containers up and down very quickly (seconds)


### # Where Docker images are stored?


- Docker images are stored in Docker Repositories
- Public: Docker Hub https://hub.docker.com/
    - Find base images for many technologies or OS:
    - Ubuntu • MySQL
    - NodeJS, Java…
- Private: Amazon ECR (Elastic Container Registry)


### # Docker versus Virtual Machines


- Docker is ”sort of” a virtualization technology, but not exactly
- Resources are shared with the host => many containers on one server


### # ECS


- ECS = Elastic Container Service
- Launch Docker containers on AWS
- You must provision & maintain the infrastructure (the EC2 instances)
- AWS takes care of starting / stopping containers
- Has integrations with the Application Load Balancer


### # Fargate


- Launch Docker containers on AWS
- You do not provision the infrastructure (no EC2 instances to manage)
– simpler!
- Serverless offering
- AWS just runs containers for you based on the CPU / RAM you need


### # ECR


- Elastic Container Registry
- Private Docker Registry on AWS
- This is where you store your Docker images so they can be run by ECS or Fargate


### # What’s serverless?


- Serverless is a new paradigm in which the developers don’t have to manage servers anymore…
- They just deploy code
- They just deploy… functions !
- Initially... Serverless == FaaS (Function as a Service)
- Serverless was pioneered by AWS Lambda but now also includes anything that’s managed: “databases, messaging, storage, etc.”
- Serverless does not mean there are no servers… 
it means you just don’t manage / provision / see them


### # Why AWS Lambda

#### 1. Amazon EC2

- Virtual Servers in the Cloud
- Limited by RAM and CPU
- Continuously running
- Scaling means intervention to add / remove servers


#### 2. Amazon Lambda

- Virtual functions – no servers to manage!
- Limited by time - short executions
- Run on-demand
- Scaling is automated! 


### # Benefits of AWS Lambda


- Easy Pricing:
    - Pay per request and compute time
    - Free tier of 1,000,000 AWS Lambda requests and 400,000 GBs of compute time
- Integrated with the whole AWS suite of services
- Event-Driven: functions get invoked by AWS when needed
- Integrated with many programming languages
- Easy monitoring through AWS CloudWatch
- Easy to get more resources per functions (up to 10GB of RAM!)
- Increasing RAM will also improve CPU and network!


### # AWS Lambda language support


- Node.js (JavaScript)
- Python
- Java (Java 8 compatible)
- C# (.NET Core)
- Golang
- C# / Powershell
- Ruby 
- Custom Runtime API (community supported, example Rust)

- Lambda Container Image
    - The container image must implement the Lambda Runtime API
    - ECS / Fargate is preferred for running arbitrary Docker images


## Next Steps

- Other Compute (Part 2)

## Date

- February 9, 2023

