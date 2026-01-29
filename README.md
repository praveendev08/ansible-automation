# ⚙️ Configuration Management with Ansible on AWS

## 📌 Project Overview
This project demonstrates **configuration management and server automation at scale** using **Ansible**.  
Multiple AWS EC2 instances are automatically configured to install required software, deploy an application, and start services without manual intervention.

---

## 🎯 Project Objective
- Automate server configuration across multiple EC2 instances  
- Ensure consistent and repeatable setups  
- Reduce manual SSH and configuration errors  

---

## 🧰 Tools & Technologies Used
- **Ansible**
- **AWS EC2**
- **Linux (Amazon Linux / Ubuntu)**
- **Docker**
- **Jenkins**
- **Nginx**


---

## ⚙️ What This Project Automates
- Docker installation and service setup  
- Jenkins installation and startup  
- Nginx installation and configuration  
- Sample application deployment  

---

## 🔄 Execution Flow
1. Ansible connects to EC2 instances via SSH  
2. Required packages are installed using playbooks  
3. Services are started and enabled  
4. Application files are deployed  
5. Configuration remains idempotent on re-runs  

---

## ▶️ How to Run This Project

### Step 1: Configure Inventory
Update `inventory.ini` with EC2 private IPs and SSH key.

### Step 2: Test Connectivity
```bash
ansible all -i inventory.ini -m ping

### Step 3: Run Playbook
ansible-playbook -i inventory.ini playbook.yml







