# ACS730 Final Project – Ansible EC2 Webserver Automation

## 👨‍💻 Project Title
Automated Web Server Setup on AWS EC2 using Ansible with Static Inventory

---

## 🧠 Team Information

- **Name:** Steven Mathew  
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
├── inventory_static.ini        # Static inventory defining EC2 public IP and SSH key
├── install_httpd.yml           # Ansible playbook to configure Apache webserver
├── proj_ansible.pem            # Private SSH key to access EC2 (excluded from Git)
├── README.md                   # Complete project documentation
├── output_log.txt              # (Optional) Output of successful playbook execution
├── .gitignore                  # Prevents sensitive files like .pem from being committed
└── demo_recording.mp4          # (Optional) Screen recording of project execution