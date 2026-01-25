# Day 01: SSH and Remote Access 🐧💻

**Week 2 – System Administration**

---

## Overview
Day 1 of my Linux learning journey focused on **SSH (Secure Shell)** and **remote access**—a foundational skill for managing Linux servers, especially in **cloud, DevOps, and system administration** environments.

By the end of the day, I was able to install, configure, and connect to my Ubuntu system remotely from Windows, laying the groundwork for secure server management.

---

 ## Key Activities

### 1. Installing SSH Server on Ubuntu
```bash
sudo apt update
sudo apt install openssh-server

## 2. Enabling and Starting SSH Service
sudo systemctl enable ssh
sudo systemctl start ssh

## 3. Verifying SSH Service
sudo systemctl status ssh

## 4. Configuring Firewall to Allow SSH
sudo ufw allow ssh
sudo ufw status

## 5. Connecting from Windows
ssh <username>@<Ubuntu-IP>**


✅ Successfully accessed my Ubuntu machine remotely.

## Why SSH Matters

Enables secure remote management of Linux servers

Essential for cloud, DevOps, and system administration tasks

Supports automation and scripting without physical access to the machine

## Key Learnings

SSH setup is straightforward but extremely powerful

Firewalls and IP addresses must be managed carefully

Remote access expands possibilities for real-world Linux and cloud operations

## Reflection

Day 1 gave me hands-on experience in setting up secure remote connections, a critical skill for any Linux professional. This foundation will be built upon in the following days to explore users, privileges, and system monitoring.
