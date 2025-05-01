# Provisioning of 2 EC2 Instances within a Custom Network via AWS CloudFormation

This project uses AWS CloudFormation to provision two EC2 instances inside a custom VPC, including a public and private subnet, Internet Gateway, and routing setup.

#Goal:
Create a simple AWS infrastructure using Infrastructure as Code (IaC) to automatically set up:
1 VPC
2 Subnets (Public and Private)
1 Internet Gateway
1 Route Table
2 EC2 Instances (1 in each subnet)

#Files Included:
`CBAProjectTemplate.yml` – The main CloudFormation YAML template.

#How to Deploy This Lab:

#Step 1: Log into AWS Console

Go to [https://aws.amazon.com](https://aws.amazon.com)

Open the CloudFormation service.

#Step 2: Upload the Template
Click Create Stack
Choose With new resources (standard)
Select Upload a template file
Upload `CBAProjectTemplate.yml` from your computer.

#Step 3: Fill in Stack Details
Stack Name: `Custom-EC2-Network-Lab`
Leave other parameters as default (or customize as needed).

#Step 4: Click Next, Next, Create
Review settings and click **Create Stack**.

Wait a few minutes while CloudFormation builds your infrastructure.

#What You’ll See After Deployment:
A new VPC with subnets
2 EC2 Instances (1 in public, 1 in private subnet)
Internet access for the public instance

#Clean Up:
When done testing:
1. Go to CloudFormation
2. Select your stack
3. Click Delete

#Notes:
Ensure your AWS account has the necessary permissions.
This template is for learning and lab purposes only.
