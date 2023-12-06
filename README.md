# aws_capstone-project
Aws-Capstone-Project-Secure_VPC
Introduction
This project was created to showcase how VPC security works also how we can use VPC for security and load balancer and autoscalaing for high availability in real time scenarios. Also, we can integrate multiple services with VPC such as EC2, Load balancer, and Autoscaling, and create a secure and scalable application.

Architecture of the project
![image](https://github.com/techieshailendra/aws_capstone-project/assets/139354445/36f1b942-9148-4975-a7a0-3ecff546bfc8)


Steps to execute the project
Design and configure a VPC: Create a VPC with custom IP ranges. Set up public and private subnets. Configure route tables and associate subnets.
VPC2
Implement network security: Set up network access control lists (ACLs) to control inbound and outbound traffic. Configure security groups for EC2 instances to allow specific ports and protocols.

Provision of EC2 instances: Launch EC2 instances in both the public and private subnets. Configure security groups for the instances to allow necessary traffic.

ec2
Setting up and running Ec2 : Setting up and running EC2 and created one host in public subnet access private ec2 using host and run and host sample server on port 8000 private1

Networking and routing: Set up an internet gateway to allow internet access for instances in the public subnet.Configure NAT gateway or NAT instance to enable outbound internet access for instances in the private subnet. Create appropriate route tables and associate them with the subnets.

Load balancer and autoscaling: Create a load balancer and attach it to an autoscaling group to make the application highly available in the same VPC that is created for the project. autoscaling

load balancer
SSH key pair and access control: Generate an SSH key pair and securely store the private key. Configure the instances to allow SSH access only with the generated key pair. Also, give port 8000 access in the security group so that the application will be able to load in it. port enabled1

Test and validate the setup: Test and run the link given by the load balancer and test the output on the browser also we can check the health of servers and if the server load increases the autoscaling group will increase the number of servers.

desired output
Advantages of the setup
Getting high availability for the application hosting because of the load balancer and autoscaling group.
Getting high security because of the VPC configuration.
