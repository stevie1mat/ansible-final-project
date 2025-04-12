# ACS730 Final Project – Ansible EC2 Webserver Automation

## 👨‍💻 Project Title
Automated Web Server Setup on AWS EC2 using Ansible with Static Inventory

---

## 🧠 Team Information

- **Name:** Deepika Paneer Selvam
- **Student Id:** 141586248
- **GitHub Repo:** [ansible-final-project](https://github.com/stevie1mat/ansible-final-project)  
- **Institution:** Seneca College  
- **Course:** ACS730 – Cloud Automation and Control Systems  
- **Semester:** Winter 2025

- **Name:** Steven Mathew  
- **Student Id:** 170069231
- **GitHub Repo:** [ansible-final-project](https://github.com/stevie1mat/ansible-final-project)  
- **Institution:** Seneca College  
- **Course:** ACS730 – Cloud Automation and Control Systems  
- **Semester:** Winter 2025



---

## 🎯 Objective

The goal of this project is to use **Ansible** to automate the configuration of a web server (Apache) on an AWS EC2 instance. The automation includes installing the web server, enabling it on boot, and creating a custom homepage.

---

## 📂 Project Structure

ansible-final-project/
- inventory_static.ini        # Static inventory defining EC2 public IP and SSH key
- install_httpd.yml           # Ansible playbook to configure Apache webserver
-  proj_ansible.pem            # Private SSH key to access EC2 (excluded from Git)
-  README.md                   # Complete project documentation
-  output_log.txt              # (Optional) Output of successful playbook execution
- .gitignore                  # Prevents sensitive files like .pem from being committed
-  demo_recording.mp4          # (Optional) Screen recording of project execution

## 🚀 Steps to Run the Ansible Playbook

### 1. Connect to Cloud9 or EC2 Instance
Make sure you’re on a machine with Ansible installed and access to your `.pem` file.

---

### 2. Set Proper Permissions for SSH Key

```bash
chmod 400 ./proj_ansible.pem
```

### 3. Run the Ansible code
```bash
ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i inventory_static.ini install_httpd.yml
```
