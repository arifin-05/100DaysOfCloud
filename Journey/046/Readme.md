# Meet 6 - EBS & AMI


## Introduction

- Amazon Elastic Block Store (Amazon EBS) is an easy-to-use, scalable, high-performance block-storage service designed for Amazon Elastic Compute Cloud (Amazon EC2).

- An Amazon Machine Image (AMI) is a template that contains a software configuration (for example, an operating system, an application server, and applications). From an AMI, you launch an instance, which is a copy of the AMI running as a virtual server in the cloud.


## Cloud Research


- Immediately we practice.
- Here I have provided 1 instance named webserver-1 with the us-east-1a availability zone.

![image](https://user-images.githubusercontent.com/121140952/230835299-14a58f35-b4c1-44aa-bbd6-22246d3633ca.png)

- Then go to the volumes tab.

![image](https://user-images.githubusercontent.com/121140952/230835336-00bc3de8-7235-45ef-a023-f6b05303ce11.png)

- Then click Create Volumes.

![image](https://user-images.githubusercontent.com/121140952/230835370-7e307bef-d1c1-4ec6-b121-7c65b484974f.png)

- For volume type is gp2. and the size is 2 GB, then for the availability zone it is us-east-1a.

![image](https://user-images.githubusercontent.com/121140952/230835393-59a89a1e-8c6d-4908-bc72-dfe7c26e2b2a.png)

- Next click Create Volume.

![image](https://user-images.githubusercontent.com/121140952/230835564-f8d303eb-a7cb-4989-ae3b-f8eb431b98ec.png)

- After that, click the volume we created earlier, then click Action, and select Attach Volume.

![image](https://user-images.githubusercontent.com/121140952/230835591-e13625a4-f594-4b77-9a3f-fe65bece45c7.png)

![image](https://user-images.githubusercontent.com/121140952/230835624-ec558828-1dc9-4b17-8e8c-59d8bcdea15a.png)

- Follow like this, click Attach Volume:

![image](https://user-images.githubusercontent.com/121140952/230835642-68ca85e2-b299-4c47-b05d-f27628232165.png)

- Now we have successfully attached the volume.

![image](https://user-images.githubusercontent.com/121140952/230838749-ec7b314f-7f2e-4dc7-9fee-2936e59db2ba.png)

- Take a look at the storage example and see that there are 2 volumes already attached.

![image](https://user-images.githubusercontent.com/121140952/230838776-5e6e7db1-90d7-4539-88d3-75fc64b7aa66.png)


- Next, we will create a second instance with the availability zone conditions us-east-1b or more details as follows.

![image](https://user-images.githubusercontent.com/121140952/230839133-708a97db-97d0-40f0-82cf-4b63c72c7c27.png)

![image](https://user-images.githubusercontent.com/121140952/230839158-fc8d7ead-052b-4279-adad-668b68e2fb92.png)

- It can be seen that I chose us-east-1b before.

![image](https://user-images.githubusercontent.com/121140952/230839265-63dfda43-9e34-4f83-a21a-11bfc3ed0874.png)

- Go to Volumes, and Detach the volume that was mounted in the previous instance.

![image](https://user-images.githubusercontent.com/121140952/230839319-5d1b17d8-1862-49e3-ba41-91807d4f3b71.png)

![image](https://user-images.githubusercontent.com/121140952/230839341-dd2854fa-1b89-4bee-af87-45eeebd4676f.png)

- Then click Volumes.

![image](https://user-images.githubusercontent.com/121140952/230839358-f5ab254c-36a8-4af6-a9e6-e8bf348f151b.png)

- Click Action and select Create snapshot

![image](https://user-images.githubusercontent.com/121140952/230839394-0b5220f0-d29e-42a2-aa3c-c5d6ceb07bfe.png)

- For the Create Snapshot section, see the conditions as below. If you have clicked Create Snapshot:

![image](https://user-images.githubusercontent.com/121140952/230839426-b597ff4e-fe87-4b2e-a720-6493521f5d27.png)

- After that go to the Snapshot section.

- Select the new Snapshot that we have created, then click Action, and select Create volume from snapshot.

![image](https://user-images.githubusercontent.com/121140952/230839446-7d04acd9-cf9f-4312-841f-9e7c511725ad.png)

![image](https://user-images.githubusercontent.com/121140952/230839470-6d6a5433-bc27-4c1d-aa07-29831d931403.png)

- these are the conditions, then click Create Volume:

![image](https://user-images.githubusercontent.com/121140952/230839500-067a1074-f4f6-4324-acd5-7c3b5c633b22.png)

- Then go to the Volume section, and select the volume that has availability zone 1a, then click Actions, then select Attach Volume.

![image](https://user-images.githubusercontent.com/121140952/230839524-b7895250-8b36-4275-aa15-0246ae98d169.png)

![image](https://user-images.githubusercontent.com/121140952/230839546-a129af45-f9ee-4979-bb35-4d1aa75dd4de.png)

- For Instance, select the instance that has the us-east-1a availability zone, then click Attach Volume.

![image](https://user-images.githubusercontent.com/121140952/230839869-05a3ea24-8c6f-44ea-b620-9f947da7cae9.png)

- If we check the instance section, it will have 2 volumes. That's a sign that it's been successful.

![image](https://user-images.githubusercontent.com/121140952/230839906-bfa611fc-aa75-483a-a42d-8f48dc8cf58a.png)

![image](https://user-images.githubusercontent.com/121140952/230839942-e8b8a9a1-842f-4689-9e22-b524761bfdfc.png)

![image](https://user-images.githubusercontent.com/121140952/230840333-5a7ef9cc-2d95-47d1-95e9-b0a8b7a270d3.png)

AMI 

- First Create new Instance and also in security group Allow traffic from http (or use your security group in same rules).
- 
![image](https://user-images.githubusercontent.com/121140952/230840378-e4f55b1a-eb0b-43c1-bb26-0bfa62f89b76.png)

![image](https://user-images.githubusercontent.com/121140952/230840399-3a396555-fbe5-41a0-80fd-6a07164cba85.png)

- In your user data, use the script to start your web server application and click on launch instance.

![image](https://user-images.githubusercontent.com/121140952/230840427-75fc53bd-ac09-4d91-9988-b966e2c474c0.png)

![image](https://user-images.githubusercontent.com/121140952/230840515-15c98c97-1dac-4fd3-b752-6a4f6df0394e.png)

- Once done, copy your instance public ip and paste it in your browser.

![image](https://user-images.githubusercontent.com/121140952/230840550-6177bd92-8587-42ea-ac82-c8ed022dbba4.png)

- Select your instance, click Actions and select an Monitor and Troubleshoot, click Create Image.

![image](https://user-images.githubusercontent.com/121140952/230840583-bb72daef-31c7-4791-bcf1-25b72aded04d.png)

- Enter a name for the image & click create image.

![image](https://user-images.githubusercontent.com/121140952/230840622-6a5373f3-73cb-495b-8e34-17e89c4036b2.png)

![image](https://user-images.githubusercontent.com/121140952/230840662-65f07874-6119-45d2-8ace-6e8b5dca8564.png)

- Enter AMIs, select the AMI that was created earlier, then click Launch instance from AMI

![image](https://user-images.githubusercontent.com/121140952/230840767-339e6503-015b-46f3-809f-5c954664aae5.png)

- In the application and OS images, they will be addressed by default in your AMI.

![image](https://user-images.githubusercontent.com/121140952/230840802-099ba52f-4e76-4f42-bc69-c86467fe52f3.png)

- Choose your security group to allow http traffic.

![image](https://user-images.githubusercontent.com/121140952/230840824-211909e9-b92d-48aa-ac2e-92905d216ad7.png)

- On user data, Add script to create html file & click on launch instance.

![image](https://user-images.githubusercontent.com/121140952/230840851-f7051937-bdb9-4d7b-ad8f-5ce01598a5c5.png)

![image](https://user-images.githubusercontent.com/121140952/230840875-2786e56d-0354-4fbc-a7d9-4e7cb96a365a.png)

- Copy your Instance public IP and paste it in your browser then see what will happen in your browser web page .


## Next Steps


- Meet 4 - ELB & ASG



## Date


- Tuesday, 11 April 2023.

