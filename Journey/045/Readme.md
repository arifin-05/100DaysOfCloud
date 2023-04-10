# Meet 5 - Amazon EC2


## Introduction


Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.



## Cloud Research


- First of all, please login to the main aws console.

![image](https://user-images.githubusercontent.com/121140952/230818062-f3f7bc88-7021-475c-ba20-f1c94054f716.png)

- Enter the search field and type ec2, if you have selected the EC2 section.

![image](https://user-images.githubusercontent.com/121140952/230818247-c67b99f1-a17a-4285-a64e-665edf813064.png)

- After that, go to the same EC2 Dashboard / Instances section, then click launch instance.

![image](https://user-images.githubusercontent.com/121140952/230818487-349815ce-45bf-44f7-9f4c-30ea1a28b56b.png)


- In the name section, please fill in according to the name of the instance we want, and in the OS Images we select Amazon Linux.

![image](https://user-images.githubusercontent.com/121140952/230818513-983016c0-77b8-4e44-a546-12ab07059265.png)

- And for its 64-bit architecture (x86).

![image](https://user-images.githubusercontent.com/121140952/230819612-3a19cc15-7333-4345-93a2-dd1efe3074ff.png)

- In the instance type select t2.micro

![image](https://user-images.githubusercontent.com/121140952/230819694-e69edcd5-5122-4273-aebd-cd9631a6fc29.png)

- And in Key Pair, this is what we can use later to remotely our instance via ssh, because I have never created a key pair, so I choose create new key pair.

![image](https://user-images.githubusercontent.com/121140952/230819764-96287fca-f3a7-4c27-b565-213a48d2a77d.png)

- like before, in the name section enter what we want, and for the key pair type select RSA, and the key file format is .pem, then click the key pair.

![image](https://user-images.githubusercontent.com/121140952/230819944-86cdd9af-cda4-4000-944c-29a6cd046086.png)

- After the key pair has been created, our device will automatically download the key pair we just created.

![image](https://user-images.githubusercontent.com/121140952/230820032-92dabeeb-400e-4cdb-9797-3c1e2810d796.png)

- then we click the refresh button, the key pair selection that we made will appear.

![image](https://user-images.githubusercontent.com/121140952/230820153-2c01e68b-bd8d-43dc-9ad7-e6987547796b.png)

- then, in the network settings section check all the columns on the left, and we will also create a security group.

![image](https://user-images.githubusercontent.com/121140952/230820214-f70587b1-9190-44f6-95ce-630465b314c5.png)

- Click Edit.

![image](https://user-images.githubusercontent.com/121140952/230820342-73b01aa6-7581-48d8-8124-8e68fe2364dc.png)

- in the VPC section we leave it as default, and for the subnet we select Avaibility Zone us-ueast-1a, and public ip must be enabled.

![image](https://user-images.githubusercontent.com/121140952/230825519-ff70a4b9-a1ad-45a4-b57e-9f1439b04616.png)

- swipe down, this is the security group display for the first rule, the type is ssh, the source type is anywhere, after that, we will click Add security group rule, to create a second security group.

![image](https://user-images.githubusercontent.com/121140952/230825948-190df190-31ba-4f0f-8793-5f9498b83cd2.png)

- Make sure the type is http.

![image](https://user-images.githubusercontent.com/121140952/230826127-1381e8fc-9047-4f1b-b6e2-2605d5251022.png)

- just leave it for Configure Storage.

![image](https://user-images.githubusercontent.com/121140952/230826190-4126bc69-241e-4008-91b7-a94473ced8c8.png)

- Click Advanced Details, and scroll down until you find User data.

![image](https://user-images.githubusercontent.com/121140952/230826240-2f49ef9d-9182-4f06-a6c2-116948694a15.png)

- In the User data column, we will enter a script like this:

![image](https://user-images.githubusercontent.com/121140952/230826275-3a5404d7-b2ce-424f-a952-aeba514dd298.png)



![image](https://user-images.githubusercontent.com/121140952/230826297-89ff73f1-b789-4f98-b3bc-7293b42ee7d9.png)

- If you have clicked launch instance.

![image](https://user-images.githubusercontent.com/121140952/230826397-15864e85-172a-420d-9076-15aba6e03f87.png)

- Make sure the result is Success. then click on the blue one, to go to our new instance.

![image](https://user-images.githubusercontent.com/121140952/230826409-38b3e1db-7346-4658-b984-a7ff6fda9fe3.png)

- click on the instance, go to the details section, and copy the Public IPv4 Address.

![image](https://user-images.githubusercontent.com/121140952/230827575-8ab6d676-800a-4f89-90b4-b4e4bc5533b9.png)

- For testing, we can access it in a web browser/firefox.


### Remote Instance Via SSH

- You do this by clicking on the instance we created earlier, then clicking Connect.

![image](https://user-images.githubusercontent.com/121140952/230826501-4b232594-e665-4858-96f9-fc89cfa28aed.png)

- Enter the SSH Client tab, then copy the text I marked in red below.

![image](https://user-images.githubusercontent.com/121140952/230826514-4b3555a5-be42-4db2-a8e0-559e5624380d.png)

- After that, all we have to do is enter CMD, and enter the directory you saved the key pair.

- Then, paste the text you copied while in AWS earlier. Then Enter.

- Finished.



## Next Steps


- Meet 3 - EBS & AMI



## Date


- Monday,  10 April 2023


