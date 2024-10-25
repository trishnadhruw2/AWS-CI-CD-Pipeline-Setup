Project  :=> "End-to-End CI/CD Pipeline Setup with Jenkins, Ansible, and Docker on AWS"

Set up an automated CI/CD pipeline using Jenkins, Maven, and Ansible for deploying a website on Docker containers hosted on AWS EC2 instances.
Managed version control with Git and GitHub, and automated deployment with Ansible.
Utilized AWS services like VPC, IAM, CloudWatch, and SNS for infrastructure management and monitoring.

1.- Configured a Virtual Private Cloud (VPC) on AWS to securely manage all EC2 instances and services, ensuring isolated network environments for the entire CI/CD pipeline setup.

     VPC Configuration: Configured a Virtual Private Cloud (VPC) on AWS, creating subnets and configuring route tables to isolate and manage network traffic securely for the entire CI/CD pipeline.
     Security Groups: Defined and implemented security groups within the VPC to control inbound and outbound traffic for EC2 instances, ensuring secure access to Jenkins, Docker, and other services.
     Subnet Allocation: Created and assigned public and private subnets in the VPC for different EC2 instances, optimizing network performance and security for Jenkins, Ansible, and Docker containers.
     Route Table and Internet Gateway: Configured route tables and attached an Internet Gateway to allow access for public-facing services, while keeping backend services isolated within private subnets.

2.Launched an EC2 instance on AWS and configured it as a "Developer Machine" for version control.

3.Installed Git on the EC2 instance to clone a free website's source code and pushed it to GitHub.

4.Set up Jenkins in Tomcat on a separate EC2 machine to pull the code from GitHub and built it using Maven.

5.Configured an Ansible server to automate the deployment of the .war file to two Docker containers across private EC2 instances.

6.Used Ansible to manage and deploy the application in Docker containers, hosting the website on AWS infrastructure.

7.Utilized AWS services like VPC for network segmentation, IAM for user management, CloudWatch for monitoring, and SNS for notifications.

8.Tools used: Git, GitHub, Jenkins, HTTPD, Maven, Ansible, Docker, AWS (EC2, VPC, IAM, CloudWatch, SNS).

### Key Components:
1. *AWS VPC:* Secure network for hosting the infrastructure.
2. *Developer Machine (EC2):* Code is written and pushed to GitHub.
3. *Jenkins & Maven Integration:* Jenkins pulls code from GitHub, builds it using Maven, and creates a .war file.
4. *Ansible:* Manages deployments and passes the .war file to the Docker container.
5. *Docker:* Application is hosted in a Docker container.
6. *CloudWatch & SNS:* Monitoring and alerting for infrastructure.



## AWS Services Used:
- *VPC:* Configured for the network.
- *EC2 Instances:* Hosted developer, Jenkins, Ansible, and Docker environments.
- *IAM:* Managed user permissions.
- *CloudWatch:* Monitored the system.
- *SNS:* Sent notifications on deployments and incidents.

## DevOps Tools:
- *Jenkins:* Automated CI/CD pipeline.
- *Maven:* Build tool for the application.
- *Ansible:* Automates the deployment process.
- *Docker:* Containerized application hosting.
-
