
# IAM Guidilines & Best Practices, Shared Responsibility Model for IAM, and  IAM Summary.


## Introduction

• IAM Guidilines & Best Practices 

• Shared Responsibility Model for IAM 

• IAM Summary

## Cloud Research


### IAM Guidilines & Best Practices 

• Don't use the root account except for AWS account setup

• One physical user = One AWS user

• Assign users to groups and assign permissions to groups

• Create a strong password policy

• Use and enforce the use of Multi Factor Authentication (MFA)

• Create and use Roles for giving permissions to AWS services

• Use Access Keys for Programmatic Access (CLI/SDK)

• Audit permissions of your account with the IAM Credentials Report

• Never share IAM users & Access Keys



### Shared Responsibility Model for IAM



![aws](https://user-images.githubusercontent.com/121140952/211448974-e036af0a-3682-4526-a538-2056005164d4.png)


• Infrastructure (global network security)

• Configuration and vulnerability analysis

• Compliance validation



![you](https://user-images.githubusercontent.com/121140952/211448997-d2e4f814-2511-4d46-80c2-968ce5661f2a.png)


• Users, Groups, Roles, Policies management and monitoring

• Enable MFA on all accounts

• Rotate all your keys often

• Use IAM tools to apply appropriate permissions

• Analyze access patterns & review permissions

### IAM Summary


• Users: mapped to a physical user, has a password for AWS Console

• Groups: contains users only

• Policies: JSON document that outlines permissions for users or groups

• Roles: for EC2 instances or AWS services

• Security: MFA + Password Policy

• AWS CLI: manage your AWS services using the command-line

• AWS SDK: manage your AWS services using a programming language

• Access Keys: access AWS using the CLI or SDK

• Audit: IAM Credential Reports & IAM Access Advisor



## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

https://cahblitaran.blogspot.com/
