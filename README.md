# AWS Ansible Docker Monitoring

This project automates the setup and deployment of Docker containers and monitoring services on AWS instances using Ansible playbooks.

## 📁 Repository Structure

- `playbook.yml`: Ansible playbook for provisioning and configuring Docker services.
- `inventory.ioi`: Inventory file defining target hosts and connection details.
- `.gitignore`: Specifies ignored files and sensitive tracking data.

## 🚀 Prerequisites

Before running the playbook, ensure you have:
- Ansible installed on your control node (WSL/Linux).
- SSH access configured for target AWS instances.
- Valid AWS credentials and security group rules configured.

## 🛠️ How to Run

1. **Update Inventory:** Update `inventory.ioi` with your AWS instance IP addresses and SSH private key path.
2. **Execute Playbook:**
   ```bash
   ansible-playbook -i inventory.ioi playbook.yml
