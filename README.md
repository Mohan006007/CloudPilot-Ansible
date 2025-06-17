# ☁️ CloudPilot-Ansible

Automate EC2 instance provisioning and OS-specific management using Ansible on AWS.

## 🚀 Features

- Launch 2 Ubuntu and 1 Amazon Linux EC2 instances using Ansible loops
- Manual setup of passwordless SSH using `ssh-copy-id` and `.pem` file
- Conditionally shut down only Ubuntu instances using Ansible facts

## 🔧 Tech Stack

- Ansible (Infrastructure as Code)
- AWS EC2
- Boto3
- SSH, YAML

## 📦 Usage

```bash
# Launch EC2 instances
ansible-playbook ec2_create.yml

# Enable passwordless SSH (run for each instance)
ssh-copy-id -f "-o IdentityFile=<PATH TO PEM FILE>" ubuntu@<INSTANCE-PUBLIC-IP>

# Shutdown only Ubuntu instances
ansible-playbook ec2_stop.yml
