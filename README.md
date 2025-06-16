# ☁️ CloudPilot-Ansible

Automate EC2 provisioning and OS-specific instance management using Ansible.

## 🚀 Features

- Launch 2 Ubuntu + 1 CentOS EC2 instances (with Ansible loops)
- Set up passwordless SSH access from control node
- Conditionally shut down only Ubuntu instances using Ansible facts

## 🔧 Tech Stack

- Ansible (IaC)
- AWS EC2
- Boto3
- YAML, SSH

## 📦 Usage

```bash
ansible-playbook create_ec2_instances.yml
ansible-playbook setup_ssh.yml
ansible-playbook shutdown_ubuntu.yml
