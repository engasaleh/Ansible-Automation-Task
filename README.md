<!-- # Ansible-Simple-Automation-Task
This repository contains an Ansible playbook and configurations for automating the deployment of [web servers]. The playbook includes tasks for setting up a [Install Apache web server, start and enable Apache service and copy custom index.html to web server].

Also this repo, it contains files such as playbook.yml, ansible.cfg, inventory, index.html. --->


# 🚀 Ansible Simple Automation Task

## 📌 Project Overview

This repository contains an Ansible automation project that provisions and configures Apache web servers automatically.

The playbook performs the following actions:

- Installs Apache (httpd)
- Starts and enables the Apache service
- Deploys a custom `index.html` file to the web server

This project demonstrates fundamental DevOps automation practices and Infrastructure as Code (IaC) principles using Ansible.

---

## 🎯 Project Objectives

- Automate Apache installation
- Configure and manage system services
- Deploy static web content automatically
- Manage multiple servers using Ansible Inventory
- Apply idempotent configuration management

---

## 🛠 Technologies Used

- Ansible
- Linux (Target Servers)
- Apache (httpd)
- SSH Authentication

---

## 📂 Project Structure

```text
Ansible-Automation-Task/
│
├── ansible.cfg        # Ansible configuration file
├── inventory          # Target hosts definition
├── playbook.yml       # Main automation playbook
├── index.html         # Custom web page
└── README.md          # Project documentation
```

---

## ⚙️ Prerequisites

Before running this project, ensure you have:

- Ansible installed on the Control Node
- SSH access to the target servers
- SSH key-based authentication configured (recommended)
- Linux-based target machines (e.g., CentOS / RHEL)

---

### ✔️ Check Ansible installation

```bash
ansible --version
```

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/engasaleh/Ansible-Automation-Task.git
```

### 2️⃣ Navigate into the Project Directory

```bash
cd Ansible-Automation-Task
```

### 3️⃣ Update the Inventory File

Edit the `inventory` file and replace the IP addresses with your target servers.

Example:

```ini
[webservers]
192.168.1.10 ansible_user=ec2-user
```

### 4️⃣ Run the Playbook

```bash
ansible-playbook -i inventory playbook.yml
```

---

## 🌐 Expected Result

After successful execution:

- Apache will be installed
- Apache service will be running and enabled
- The custom `index.html` page will be deployed to the web root directory

You can access the web server using:

```
http://<server-ip>
```
