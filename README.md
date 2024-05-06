To create an EC2 instance, I first logged into my AWS Management Console using my credentials. Once logged in, I navigated to the EC2 service by clicking on it from the list of available services.
 

 ![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/826865e6-14d0-473a-b947-7ad3623a6c59)

 ![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/65dd4e87-becc-42d6-8e9a-cfcbade4e9f8)


 ![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/61df88c9-8a0e-4a74-a789-e60c82c5015d)

In the instance creation wizard, I chose an Amazon Machine Image (AMI) based on my requirements. For example, I selected an Amazon Linux AMI. Next, I selected an instance type based on the computing power and resources I needed. After that, I configured the instance details such as network settings, subnets, and security groups. I made sure to configure SSH access by allowing inbound traffic on port 22. 
Create a Keypair to connect to Ec2 with SSH Connect through key authentication. And launch the Instance.
 

![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/f3c83475-4e0e-4148-8eef-ae61a2bc867f)


After creation of Ec2 instance go to that instance, It takes some time to run the instance


![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/864f9d07-63eb-4a41-ae9a-052d70b7e935)

 
We can see the public IP address of the instance as shown in the fig. Copy the IP address
Open a windows terminal to connect the instance through Key_Authentication. For this first download the public_key of the instance.
Once the instance was launched, I connected to it using an SSH client. For Linux, I opened my terminal and used the SSH command followed by the public IP address of the instance and the path to the private key file. For Windows, I used PuTTY to connect to the instance by entering the public IP address and providing the private key file.

Command to connect the instance is   ssh -i <pub_key> ec2-user@<Ip address>

Here Ec3-user may change for different AMI or OS of the instance 
 

![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/01f267ce-abc1-4b2c-9448-ead629c72e44)


After successfully connecting to the instance, I followed the instructions to perform various tasks. I showed the contents of the current directory using the "ls" command, created a directory using the "mkdir" command, changed directory using the "cd" command, created a file using the "touch" command, added content to the file using a text editor like "nano" or "vim", moved the file to another directory using the "mv" command, and used the "grep" command to find the file.
1.	Show the contents of the current directory.

pwd - command used to show the current directory.
ls – command to see the file and folders in the current directory.

2.	Create a directory.

mkdir <filename> 


 ![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/a17b1535-e250-4b2f-97f1-44efb546022a)


3.	Change directory.

     cd <directory name>

4.	Create a file.

touch <filename>


![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/3f1c383b-6a29-4dbf-a022-2303a8d569b2)

 
5.	Add content to that file

To add content in the file I use nano ,vi , and echo commands.
 

![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/46c31158-8a53-4d02-8e5a-54d2ac4b87fa)


6.	Move the file from one folder to another

mv – this command is used to move the file one directory to another

mv <file name>  <the path where the file has to move >


![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/6a9389c2-c469-4331-aaa9-ed7bd4d7925a)

 
7. Use GREP to find the file.
ls <foldername> | grep <filename>


 ![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/b75bd171-d447-48c1-ae94-abbcab222476)


I have completed the above tasks, log out of the network playground by entering logout.

 

![image](https://github.com/sainakka5/Ec2_instance_creation/assets/136338958/d346c6ef-6a27-4b16-9bd8-e958ac25a974)

 





