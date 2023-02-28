# Meet 4 - IAM (Create User & Group)


## Introduction


- IAM Hands On


## Cloud Research


We will create a user and group according to the image below :

![image](https://user-images.githubusercontent.com/121140952/221809890-980ce8b3-e9ae-4439-a288-e946cce5c70a.png)


## Create Groups


# Group EC2-monitoring


- Go to search, find and click on IAM


![image](https://user-images.githubusercontent.com/121140952/221810404-d5ff87a5-42bc-492e-839a-f9b9b790a685.png)


- Click User Groups


![image](https://user-images.githubusercontent.com/121140952/221810516-08420492-f225-44c2-9a2a-25ea6d59f42a.png)


- Click Create Group


![image](https://user-images.githubusercontent.com/121140952/221810647-a3a1b2cc-0ea3-4e1f-a580-14509d151f4f.png)


- Enter the name of the group you want to create


![image](https://user-images.githubusercontent.com/121140952/221810791-b41a07f5-8187-499a-9482-9335b89e9178.png)


- Look for the permission you want to attach


![image](https://user-images.githubusercontent.com/121140952/221810939-d1089a62-259a-4ef9-8cfc-5655e40fcc7b.png)


- Click create group


![image](https://user-images.githubusercontent.com/121140952/221811075-c4f68e45-d11e-4f8d-9793-3698a59a6fef.png)


# Group VPC Monitoring


- Still in the User Group then click create group, enter the name of the group you want to create


![image](https://user-images.githubusercontent.com/121140952/221813285-add22930-90a4-4467-9a7d-c7ba06c176ab.png)



- Look for the permission you want to attach 


- Select the permissions you want to attach


- Click create group


![image](https://user-images.githubusercontent.com/121140952/221813452-dbfe108b-2346-44a9-b56e-4363f0514684.png)


## Create User


# User1


- Click Users and also click add users


![image](https://user-images.githubusercontent.com/121140952/221814455-8b007766-fad0-40c0-a181-9e32241c5d8f.png)


- Enter the user name and password you want to create, and click next


![image](https://user-images.githubusercontent.com/121140952/221814646-24f58be7-6ebb-491d-86aa-22fd2b88c9c1.png)


- Attach permission, here I choose attach policy directly, search for the permissions you want to attach and select the permissions that have been searched for


![image](https://user-images.githubusercontent.com/121140952/221814873-b6db634e-ef15-4f9e-8e38-bccc80b5675d.png)


- Review users that have been created then create


## Add User to Group


- Click the user you want to add
- Click Tab Groups and click Add user to groups


![image](https://user-images.githubusercontent.com/121140952/221815366-61f9b4a8-4d87-4f28-a3db-12d839b40a7d.png)


- Click the group you want and click add user to groups


![image](https://user-images.githubusercontent.com/121140952/221815957-3a0c9df8-5a0d-43ae-b173-6b4514c77db0.png)


# User 2


- Click add users


![image](https://user-images.githubusercontent.com/121140952/221816554-83420186-a0b7-4cc4-a9b1-1ad60702cd4f.png)


- Enter the user name and password you want to create, and click next


![image](https://user-images.githubusercontent.com/121140952/221816697-a014e303-0d3f-4d2b-8f6b-b8964b54d82c.png)


- In the topology user2 is in the ec2-monitoring group so for the permission options I select add user to group and select the group that you want to attach


![image](https://user-images.githubusercontent.com/121140952/221816855-8d5b6392-e502-4bfe-a473-41b81ff73616.png)


- Review users that have been created then create


![image](https://user-images.githubusercontent.com/121140952/221817068-7b55be70-ab89-429a-80a8-38f411bb45de.png)


# User 3


- Click add users


![image](https://user-images.githubusercontent.com/121140952/221817247-da1132d1-611d-45f2-85f4-89e7fbc795dd.png)



- Enter the user name and password you want to create, and click next


![image](https://user-images.githubusercontent.com/121140952/221817347-d6bc677d-3b97-4ac2-8e4b-1f45460339f9.png)


- In the topology user3 enters the ec2-monitoring and vcp-monitoring groups so for the permission options I select add user to group and select the group that you want to attach


![image](https://user-images.githubusercontent.com/121140952/221817492-03223705-238e-4c2a-a365-2f87b2ece577.png)


![image](https://user-images.githubusercontent.com/121140952/221817540-8ca55ce1-9fd6-4110-9b84-d75ce398b591.png)


- Review users that have been created then create


![image](https://user-images.githubusercontent.com/121140952/221817786-cd73d193-c25c-41b1-be87-79479fc48009.png)


## Next Steps


- 


## Date


- February 28, 2023


