# Deployment Steps for Web App on AWS EC2

## 1. Launch EC2 Instance
- Amazon Linux 2 AMI
- t3.micro instance
- Create new key pair (saved .pem file)

## 2. Configure Security Group
- Allow inbound SSH (port 22) from my IP
- Allow inbound HTTP (port 80) from anywhere (0.0.0.0/0)

## 3. Connect to Instance via SSH
```bash
chmod 400 my-key.pem
ssh -i "my-key pem" ec2-user@ec2-16-170-163-186.eu-north-1.compute.amazonaws.com
