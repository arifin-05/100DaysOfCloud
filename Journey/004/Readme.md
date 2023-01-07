# AWS Access Keys, CLI and SDK


## Introduction

Access keys are long-term credentials for an IAM user or the AWS account root user. You can use access keys to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK). The journey goes something like this :

    1. Users Can Access AWS.

    2. Explanation of the AWS CLI.

    3. A Description of the AWS SDK.


## Cloud Research


### 1. How Users Can Access AWS?

  • To access AWS, you have three options:

      • AWS Management Console (protected by password + MFA)

      • AWS Command Line Interface (CLI): protected by access keys

      • AWS Software Developer Kit (SDK) - for code: protected by access keys

  • Access Keys are generated through the AWS Console

  • Users manage their own access keys

  • Access Keys are secret, just like a password. Don't share them

  • Access Key ID ~= username

  • Secret Access Key password



### 2. What's the AWS CLI?

  • A tool that enables you to interact with AWS services using commands in your command-line shell

  • Direct access to the public APIs of AWS services

  • You can develop scripts to manage your resources

  • It's open-source https://github.com/aws/aws-cli

  • Alternative to using AWS Management Console
   
![cli aws](https://user-images.githubusercontent.com/121140952/211148728-482dbc77-8b88-4836-b251-2230cfe26476.png)



### 3. What's the AWS SDK?

  • AWS Software Development Kit (AWS SDK)

  • Language-specific APIs (set of libraries)

  • Enables you to access and manage AWS services programmatically

  • Embedded within your application

  • Supports

      • SDKs (JavaScript, Python, PHP, .NET, Ruby, Java, Go, Node.js, C++)

      • Mobile SDKs (Android, iOS,...)

      • IoT Device SDKs (Embedded C, Arduino, ...)

  • Example: AWS CLI is built on AWS SDK for Python

![aws-sdk 1](https://user-images.githubusercontent.com/121140952/211148769-75af28d1-2c2b-4475-a9ad-6ea50550cd9c.png)



## Next Teps


## Social Proof

https://cahblitaran.blogspot.com/
