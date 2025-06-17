# ☁️ CloudPilot-Ansible

Automate EC2 provisioning and OS-specific instance management using Ansible.

## 🚀 Features

- Launch 2 Ubuntu + 1 Amazon Linux EC2 instances (using Ansible loops)
- Configure passwordless SSH from control node
- Conditionally shut down only Ubuntu instances using Ansible facts

## 🔧 Tech Stack

- Ansible (IaC)
- AWS EC2
- Boto3
- YAML, SSH

## 📦 Usage

```bash
ansible-playbook ec2_create.yml
ansible-playbook setup_ssh.yml
ansible-playbook ec2_stop.yml
