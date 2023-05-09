# Meet 11 - EasyStack (Computing, Network, Alert).


## Introduction


- Create Networks & Subnets
- Create key pair
- Create Instances
- Connect Instance to internet (Router and Floating IP).

Verivy :

- Try SSH instance on local
- Monitoring Witch Alerts
- Make Sure That get a Warning Email From Alerts.


## Cloud Research


### #1. Create Networks & Subnets


- click service catalog and choose network

![image](https://user-images.githubusercontent.com/121140952/236987378-68a33ace-cdc4-4e8e-8a62-ce2e7891eccc.png)

- Click create network.

![image](https://user-images.githubusercontent.com/121140952/236987430-10a2cd39-0505-4316-8de8-d158d38604a3.png)

- Give it name,and enter IPV4 subnet you need.

![image](https://user-images.githubusercontent.com/121140952/236987523-2dfeda32-e889-47fb-a9c4-1695bf47d6c2.png)

- Click advanced configuration and add address pool range.click create network.

![image](https://user-images.githubusercontent.com/121140952/236987619-2d1aa395-180e-4ba4-84eb-1a61cf6a2d6b.png)


### #2. Create Key Pair


- Choose SSH Key Pair on service catalog.

![image](https://user-images.githubusercontent.com/121140952/236987769-10e86e0b-8241-41dd-bbf9-3f101814fafa.png)

- Click create key pair.

![image](https://user-images.githubusercontent.com/121140952/236987871-04e6c301-4531-4940-971b-f2790131b703.png)

- Give name for key pair,click create.

![image](https://user-images.githubusercontent.com/121140952/236987927-42143724-1973-4130-9e0f-e0b9316036f5.png)

- Copy private key.

![image](https://user-images.githubusercontent.com/121140952/236988027-38909540-435c-43ce-bd81-643b5cbe310f.png)


### #3. Create Instance


- Choose instance on service catalog.

![image](https://user-images.githubusercontent.com/121140952/236988252-b026d80e-55bc-4f19-a110-f2ba0ebc6bf9.png)

- Click create instance.

![image](https://user-images.githubusercontent.com/121140952/236988325-8bea47f0-2e73-4220-afd2-8f45322b7081.png)

- Select image you needed.

![image](https://user-images.githubusercontent.com/121140952/236988426-9b4d0ef2-bba1-4e04-9764-3621e6497fa8.png)

- Then choose how much capacity you need.

![image](https://user-images.githubusercontent.com/121140952/236988610-867acd40-bf14-47e9-9a4c-95942f64cce6.png)

- Check delete with instance and click next...

![image](https://user-images.githubusercontent.com/121140952/236988686-0175f1cf-1a07-4efa-8473-5598733a3de1.png)

- Select network & subnet that we created earlier,click next.

![image](https://user-images.githubusercontent.com/121140952/236988857-157c2a48-ae5c-4013-a0a9-b2442c90390f.png)

- Give it name for instance and choose key pair we made earlier,click next.

![image](https://user-images.githubusercontent.com/121140952/236988924-423c6f91-a088-4e46-a01e-bb4d4d217972.png)

- Review and click create instance.

![image](https://user-images.githubusercontent.com/121140952/236988989-aee3b742-f73e-408f-8501-f1b162da2680.png)

- Wait until the instance status becomes active.

![image](https://user-images.githubusercontent.com/121140952/236989069-19c921aa-c886-45df-99e8-a55fbb003b18.png)

### #4. connect instance to internet (router & floating ip)

- Choose router on service catalog.

![image](https://user-images.githubusercontent.com/121140952/236989193-83b6c034-076e-4fc4-96f5-2a6518f18af4.png)

- Click the router that is already available or has been made.

![image](https://user-images.githubusercontent.com/121140952/236989292-977f5a1b-fbf8-4545-b03a-8312a53e383b.png)

- Click connect subnet.

![image](https://user-images.githubusercontent.com/121140952/236989370-74573e5c-24d6-4a90-a0ae-51ba6d873364.png)

- In tab subnet choose subnet that was created earlier,and click connect.

![image](https://user-images.githubusercontent.com/121140952/236989478-42e3db36-e0b9-46ef-913d-05589b2587ec.png)

- Click floating IP tab then click apply for IP to project.

![image](https://user-images.githubusercontent.com/121140952/236989576-469f6bea-2a46-424b-b3bc-9426df362a8a.png)

![image](https://user-images.githubusercontent.com/121140952/236989595-a6e8d2af-9483-4da6-9015-aa50b8ee189d.png)

- Enter the size you need.

![image](https://user-images.githubusercontent.com/121140952/237006107-b7f255e0-8fbf-435f-a98b-db107e38dc48.png)

- This is the public ip we get.

![image](https://user-images.githubusercontent.com/121140952/237006259-51e9e8f1-04f6-4e4d-928a-ef1d7de6ad3d.png)

- We must first attach the public ip to our instance. click more choose associate to vNIC.

![image](https://user-images.githubusercontent.com/121140952/237006334-bdc8dec3-8ec5-4325-94d7-6931d8254fd8.png)

- choose our instance and vNIC will adjust.

![image](https://user-images.githubusercontent.com/121140952/237006435-f6150fc2-1173-4ab6-881e-7be1d345872e.png)

### Verivy

### Try SSH Instance on Local

- Open PuttyGen.

![image](https://user-images.githubusercontent.com/121140952/237006602-1359dcbb-987e-4069-93df-b029a68ebfcc.png)

- On tab conversions click import key.

![image](https://user-images.githubusercontent.com/121140952/237006675-d6e7c0a2-79fb-4367-95ec-4addb4aff774.png)

- Select file where you save the private key.

![image](https://user-images.githubusercontent.com/121140952/237006739-42c5fcd2-8120-45f0-97c3-5e559c94aec0.png)

- Wait for minute and click save private key.

![image](https://user-images.githubusercontent.com/121140952/237006830-4107925f-7d1f-4de7-bdda-184f9677747e.png)

- Click yes, save without passphrase.

![image](https://user-images.githubusercontent.com/121140952/237006915-e0c79f1f-eddb-46cc-ab71-f800b2b9fbe0.png)

- Give name for public key,and format file is .ppk

![image](https://user-images.githubusercontent.com/121140952/237007106-0e024d53-5f87-4fc0-880a-889da6dbe6f9.png)

- open putty
- Choose connection, SSH, then auth, Credentials, click browser..

![image](https://user-images.githubusercontent.com/121140952/237007322-37c80ee2-acd6-4679-89d8-0ac15fa281ba.png)

- Choose key you saved earlier.

![image](https://user-images.githubusercontent.com/121140952/237007499-12f45d38-fd68-4a3d-8205-50d0998e2500.png)

- And we will ssh with this private key.

![image](https://user-images.githubusercontent.com/121140952/237007603-b4b9dff8-8b84-4c5e-8012-9efcab2a975f.png)

- Go to session tab,enter your ip public intance and click open.

![image](https://user-images.githubusercontent.com/121140952/237007695-7250d929-8343-4933-bfa7-ee3c24ff5b73.png)

- Click accept.

![image](https://user-images.githubusercontent.com/121140952/237007764-5cbf5814-4a44-4bbd-9739-5d14d14c51e7.png)

- Result, try login with user root.

![image](https://user-images.githubusercontent.com/121140952/237007826-c7414cb7-84ad-4add-b41c-0439570841d0.png)

- Try to ping google.com and make sure instance can access internet.

![image](https://user-images.githubusercontent.com/121140952/237007884-ab407ccb-666a-433b-910d-d2577213c74c.png)

- And finally instance can access internet.

### Monitoring With Alerts

- choose alerrt management on service catalog.

![image](https://user-images.githubusercontent.com/121140952/237008085-a406e807-0a79-425d-a29a-0954047282c6.png)

- click create alert.

![image](https://user-images.githubusercontent.com/121140952/237008140-9506c3d3-083b-45af-9d4e-71fe97311066.png)

- Select your instanc,click next.

![image](https://user-images.githubusercontent.com/121140952/237008239-96074cf6-f2bd-4d0d-b9d7-9481a1532d68.png)

- Give name for alert,then enter your periodic and click automatically fill in the description.then a description will appear according to the periodic that has been selected.click next.

![image](https://user-images.githubusercontent.com/121140952/237008316-2ecb8e91-1230-46c0-96fb-bfdabb74ec85.png)

- Click create contact info.

![image](https://user-images.githubusercontent.com/121140952/237008478-33245230-d1ca-4fee-bd00-81989ed3b3c5.png)

- Give name for contact,enter your email.click create.

![image](https://user-images.githubusercontent.com/121140952/237008797-dff184d8-2b27-4a7b-9b36-63fa92f89718.png)

- Setting your notification and choose your email for notify.

![image](https://user-images.githubusercontent.com/121140952/237009011-9fb0be5f-dc1a-4c00-8a42-7b303d3dafe9.png)

- Result.

![image](https://user-images.githubusercontent.com/121140952/237009092-0330a093-4c45-4ac8-b463-f891b8fba181.png)

- Wait untill get email alarm like this.

![image](https://user-images.githubusercontent.com/121140952/237009210-d8f7bf19-69b8-4b7f-89ab-b78bdb2c678b.png)

















