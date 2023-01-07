
# IAM Identity and Access Management


## Introduction

Identity and access management (IAM) is a framework of business processes, policies and technologies that facilitates the management of electronic or digital identities. With an IAM framework in place, information technology (IT) managers can control user access to critical information within their organizations. Systems used for IAM include single sign-on systems, two-factor authentication, multifactor authentication and privileged access management. These technologies also provide the ability to securely store identity and profile data as well as data governance functions to ensure that only data that is necessary and relevant is shared.

I've been studying IAM Users and Groups in AWS, the journey goes something like this :

1. IAM: Users & Groups

2. IAM Permissions


## Cloud Research

### 1. IAM: Users & Groups in AWS

• IAM = Identity and Access Management, Global service.

• Root account created by default, shouldn't be used or shared.

• Users are people within your organization, and can be grouped.

• Groups only contain users, not other groups.

• Users don't have to belong to a group, and user can belong to multiple groups.



### 2. IAM Permissions

![per1](https://user-images.githubusercontent.com/121140952/211130555-110ee187-cc8b-456f-9f25-533bf00bf475.png)


• Users or Groups can be assigned JSON documents called policies.

• These policies define the permissions of the users.

• In AWS you apply the least privilege principle: don't give more permissions than a user needs.


### 3. IAM Policies Inheritance

!![inter](https://user-images.githubusercontent.com/121140952/211130622-620a9215-96a6-44be-ae72-2c8277557627.png)


You can attach policies to organization entities (organization root, organizational unit (OU), or account) in your organization:

• When you attach a policy to the organization root, all OUs and accounts in the organization inherit that policy.

• When you attach a policy to a specific OU, accounts that are directly under that OU or any child OU inherit the policy.

• When you attach a policy to a specific account, it affects only that account.


### 4. IAM Policies Structure 

![stru](https://user-images.githubusercontent.com/121140952/211130794-52bc44a8-f2b1-48bc-9981-cfc160c7d133.png)

#### 1. Consists of

- Version: policy language version, always include "2012-10- 17"

- Id: an identifier for the policy (optional) .

- Statement: one or more individual statements (required)


#### 2. Statements consists of

- Sid: an identifier for the statement (optional)

- Effect: whether the statement allows or denies access (Allow, Deny)

- Principal: account/user/role to which this policy applied to

- Action: list of actions this policy allows or denies

- Resource: list of resources to which the actions applied to

- Condition: conditions for when this policy is in effect (optional)


### 5. IAM - Password Policy

IAM - Password Policy

• Strong passwords = higher security for your account

• In AWS, you can setup a password policy:

  • Set a minimum password length

  • Require specific character types:

    • including uppercase letters

    • lowercase letters

    • numbers

    • non-alphanumeric characters

  • Allow all IAM users to change their own passwords

  • Require users to change their password after some time (password expiration)

  • Prevent password re-use


### 6. Multi Factor Austhentication - MFA

Multi Factor Authentication - MFA

• Users have access to your account and can possibly change configurations or delete resources in your AWS account

• You want to protect your Root Accounts and IAM users

• MFA = password you know + security device you own

![mfa1](https://user-images.githubusercontent.com/121140952/211131423-904fdaf8-2b72-44ff-9f2a-860e6bb64f8e.png)

• Main benefit of MFA:

if a password is stolen or hacked, the account is not compromised


## Next Steps

AWS Access Keys, CLI and SDK


## Social Proof

https://cahblitaran.blogspot.com/
