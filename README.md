# ansible-aws-infra-automation
Ansible playbooks to automate AWS infrastructure deployment (EC2, S3, RDS, IAM, and Load Balancer).

# AWS Infrastructure Automation with Ansible

## Overview 

This project automates the deployment of an AWS infrastructure using "Ansible". It provisions "EC2 instances", configures Nginx web servers", and sets up "MySQL databases".

# Features
✅Automates EC2 provisioning  
✅ Installs and configures Nginx & MySQL  
✅ Uses **Ansible roles** for modular playbooks  
✅ Supports **dynamic inventory** from AWS  


## setup instructions

1. clone the repository

git clone https://github.com/Girishrao2002/ansible-aws-infra-automation.git

cd ansible-aws-infra-automation


2. Install dependencies

    pip install boto3 botocore
    ansible-galaxy install -r requirements.yml


3. Configure AWS Credentials

     Ensure your AWS credentials are set up in ~/.aws/credentials


4. Run the playbook
	ansible-playbook -i inventory/site.yml


5. verify deployment

	curl http://your-ec2-public-ip

