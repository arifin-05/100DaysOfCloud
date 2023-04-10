# Meet8 - Create Bucket & Static Website


## Introduction


- For example case scenarios, see the following Link


## Cloud Research


### Create Bucket


- The first step we have to do is enter the aws console first.

![image](https://user-images.githubusercontent.com/121140952/230871222-3cb6fb7b-7e6a-4b1c-933a-c80baf6e74bf.png)

- Enter the search field, and type s3.

![image](https://user-images.githubusercontent.com/121140952/230871311-73613a9b-aa66-4add-97bc-c7c57ff5d735.png)

- Click Create Bucket.

![image](https://user-images.githubusercontent.com/121140952/230871397-ebabd663-5383-42a2-9a92-59417d53508f.png)

- Give your bucket name and in Region I chose US East (N.Virgia) us-east-1.

![image](https://user-images.githubusercontent.com/121140952/230871446-0800ae3b-d04f-4620-9aec-d1e698d03a2e.png)

- Follow below:

![image](https://user-images.githubusercontent.com/121140952/230871505-c54974eb-aeaa-4d60-a3ea-b2c69d5cabba.png)

![image](https://user-images.githubusercontent.com/121140952/230871647-90cf3ca4-1028-464a-9944-638031391ae0.png)

- Here in the example case scenario, we are instructed to retrieve content from the website Link and upload it to our bucket.

![image](https://user-images.githubusercontent.com/121140952/230871864-968e52b8-6965-40c2-b7a2-c5029d5e8c80.png)

- Click Upload.

![image](https://user-images.githubusercontent.com/121140952/230871954-a4821149-c2f4-45c7-bcb9-cc51bbd66221.png)

- Upload everything needed

![image](https://user-images.githubusercontent.com/121140952/230872070-dc02282a-1871-4861-8a68-5fa653f23bee.png)

- Scroll down and click Upload

![image](https://user-images.githubusercontent.com/121140952/230872176-5727f6b3-25a5-4854-9c9f-2c475b5aedf6.png)

- Here we give permission so that it can be accessed by public

- First we go to the permissions tab\

![image](https://user-images.githubusercontent.com/121140952/230872403-3bcab529-1b3f-4b61-ac2f-d6ae61ef7222.png)

- Then scroll down until there is a Bukcet Policy, click edit

![image](https://user-images.githubusercontent.com/121140952/230872487-010d5440-2952-4e64-8761-8571774fe98a.png)

- Click Policy generator.

![image](https://user-images.githubusercontent.com/121140952/230872590-bd19a189-2978-447b-8863-a7393b76b693.png)

- Type we choose S3 and on the Principal we give the * sign which means for all

![image](https://user-images.githubusercontent.com/121140952/230872712-b789c4aa-da06-4e5c-98f3-47c96ab194ec.png)

- In the Action section select GetObject

![image](https://user-images.githubusercontent.com/121140952/230872800-4120a3ae-3bfb-4247-9e9b-3264d8fa8e95.png)

- In this section we copy the ARN and paste it here

![image](https://user-images.githubusercontent.com/121140952/230872933-3ea92b42-a1f9-4704-ba9b-394cf0f23231.png)

![image](https://user-images.githubusercontent.com/121140952/230873082-1ea4a130-b0de-4e1c-b56b-d38fcb5618be.png)

- Add /* at the end of the ARN link

![image](https://user-images.githubusercontent.com/121140952/230873126-31b8e326-a592-43aa-9a7c-7f1105f68e84.png)

- Click Add Statement

![image](https://user-images.githubusercontent.com/121140952/230873220-fc8e8562-2faf-4a91-b623-d63ceca03a76.png)

- Click Generate Policy

![image](https://user-images.githubusercontent.com/121140952/230873283-61890bfa-27a1-4bc3-b73e-b91fd18c9455.png)

- Copy the JSON

![image](https://user-images.githubusercontent.com/121140952/230873373-60d285a5-acc6-4f39-b837-b4e1464a895e.png)

- Copy the JSON earlier in this section

![image](https://user-images.githubusercontent.com/121140952/230873434-ea38464a-6f33-4553-a02c-dc7bc3a2d2e2.png)

- Click Save changes

![image](https://user-images.githubusercontent.com/121140952/230873515-d8a72ad3-98f8-4860-9b88-0e72838a35ce.png)

![image](https://user-images.githubusercontent.com/121140952/230873779-7ea645fb-31a8-4c9a-a8d5-33a864ace4e5.png)


### Enable Bucket Versioning

- First, in the Properties section and in the Bucket Versioning section, click edit

![image](https://user-images.githubusercontent.com/121140952/230873716-ec66ecbb-5e67-4f0b-9f8d-1e9afd42e99e.png)

- Select Enable then save changes

![image](https://user-images.githubusercontent.com/121140952/230873860-de0d3f14-163c-4a81-bd05-40c63a6ad7ab.png)

- Later it will appear like this

![image](https://user-images.githubusercontent.com/121140952/230873939-0dcd940d-f0dc-45f3-ada9-58da47b3b59d.png)

- 
## Next Steps


- Meet 9 - VPC.


## Date

- Wadnesday, 11 April 2023.



