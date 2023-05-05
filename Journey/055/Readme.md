# Meet 10 - EasyStack (Compute, Network, Alert)


## Introduction 


- In this journey, we will study the services available on EasyStack. EasyStack is a cloud computing service based on OpenStack, and EasyStack provides cloud platform solutions during the current hybrid cloud era in Asia. And at this time we will learn Upload Image, computing, network and alerts in EasyStack.


## Cloud Research


- The first step here we will try to upload the Image first.
- Go to Service Catalog and click Instance Image.


![image](https://user-images.githubusercontent.com/121140952/236387925-82474137-6c03-498f-ad56-053d6dc37930.png)

- Then click Create Image.

![image](https://user-images.githubusercontent.com/121140952/236387944-afa1c4e7-19a6-4d12-993c-f2536b53fc30.png)

- Give it a name and click Upload File then select ISO, here I'm using Debian 11.

![image](https://user-images.githubusercontent.com/121140952/236387975-acb4c93d-ee90-4527-9750-2f137a1d7369.png)


![image](https://user-images.githubusercontent.com/121140952/236388013-890098a1-cc10-4a6e-a516-a6fa438b9a40.png)

- Then select the operating system, CPU, and Hypervisor. Also fill in Minimum Root and Minimum RAM, then click Create.

![image](https://user-images.githubusercontent.com/121140952/236388033-1638b0e7-9d46-4539-a0e8-6e7820da626f.png)

- Okay now we enter the Network section, click Service Catalog then click network.

![image](https://user-images.githubusercontent.com/121140952/236388061-24e86fce-2d25-4657-a61e-ee42d1102dec.png)

- Click Create Network.

![image](https://user-images.githubusercontent.com/121140952/236388086-bbe61206-3c84-4dc7-b30e-3209ac1376c1.png)

- Give it a name and IPv4 subnets and click create network

![image](https://user-images.githubusercontent.com/121140952/236388119-7336c9e7-5cdb-4125-9b14-d6a795c26b21.png)


![image](https://user-images.githubusercontent.com/121140952/236388131-4b539ef5-e242-4b7b-aeb1-e9fe2193c356.png)

- Then here we will create a subnet, move to the subnet tab then click create subnet.

![image](https://user-images.githubusercontent.com/121140952/236388154-87bc29a9-e6bc-4a8c-b9ef-58fa8001d513.png)

- Then select the newly created network.
- Click Advanced Configuration then give DNS Server and give Address Pool Range and click create subnet.

![image](https://user-images.githubusercontent.com/121140952/236388172-4983021c-bf8d-444e-86cf-3e8fb81a814f.png)

- Ok, now let's create an Instance, click Service Catalog then select Instance.

![image](https://user-images.githubusercontent.com/121140952/236388192-c48b3fe7-44c7-4aff-8d23-75ea23210d54.png)

- Click Create Instance.

![image](https://user-images.githubusercontent.com/121140952/236388294-56520edf-940a-47e0-a11f-2df50c60d006.png)

- Select the image you want to attach. 

![image](https://user-images.githubusercontent.com/121140952/236388316-60e4dd9f-d9b5-4ce5-bafb-40f99d36ae4e.png)


![image](https://user-images.githubusercontent.com/121140952/236388335-71abeb48-1606-4c65-a464-642525a2d2f9.png)

- Check Delete with Instance, then click network configuration.

![image](https://user-images.githubusercontent.com/121140952/236388463-535fef11-cf02-4781-a9d1-7ccd5f7e1845.png)

- Choose network and klik next.
![image](https://user-images.githubusercontent.com/121140952/236388484-a61888c1-ffdb-47f0-a56a-087baa069777.png)

- We're going to pair it, so we're going to go back to e service catalog again, then click SSH To Pair.

![image](https://user-images.githubusercontent.com/121140952/236388516-af5ee4af-ca13-42e1-aeb9-f4fa4181e535.png)

- Click create key pair.

![image](https://user-images.githubusercontent.com/121140952/236388536-f35604c1-34ce-4657-87a5-e03f711161c2.png)

- Give it a name then click create.

![image](https://user-images.githubusercontent.com/121140952/236388557-51e73400-50b5-4520-b7c5-d396825f1152.png)

- Copy public key and save.

![image](https://user-images.githubusercontent.com/121140952/236388577-b789aa39-7e2b-436d-a9d7-b684be45fc3a.png)

- Enter the key you just created.

![image](https://user-images.githubusercontent.com/121140952/236388603-f16d505e-9592-4956-bf59-77904715758b.png)

- Check it and click create instance

![image](https://user-images.githubusercontent.com/121140952/236388630-559142d4-f0e2-4ae8-9a89-e48487f6e2c4.png)

- Okay, we'll try alerts, go to the service catalog and select alert management.

![image](https://user-images.githubusercontent.com/121140952/236388646-5da1d354-23a4-40d2-9ee5-714a6d2942ae.png)

- Click create Alert.

![image](https://user-images.githubusercontent.com/121140952/236388668-6e3e407d-4a4c-4809-a08c-9b7d7fe7d7a2.png)

- Select the selected instance.

![image](https://user-images.githubusercontent.com/121140952/236388690-4aeaa94b-afde-4170-89fe-b3719c6eeb59.png)

- Give it a name and click Automatically fill in the description.

![image](https://user-images.githubusercontent.com/121140952/236388723-1e74af2c-23c6-4316-8d22-279cd812c1ee.png)


![image](https://user-images.githubusercontent.com/121140952/236388737-ce65db83-12f9-412a-ab72-4a67b860ef99.png)


![image](https://user-images.githubusercontent.com/121140952/236388762-ee62979a-3f88-499d-aa8b-06ce58ddff4a.png)

