# **Day 03: SSH Key-Based Authentication & System Monitoring** 🐧🔐

**Week 2 – System Administration**

---

## **Overview**
After strengthening SSH fundamentals in the previous days, Day 3 focused on **secure access mechanisms** and **system visibility**—both critical when working with **cloud servers, production machines, and remote environments**.

The learning moved beyond basic connectivity into **authentication, trust-based access, and monitoring system behavior**.

---

## **What I Learned & Practiced**

### **1. SSH Key Generation (Password-less Authentication)**
I generated an SSH key pair using `ssh-keygen` to understand **public-key authentication**.

```bash
ssh-keygen

✔️ This created:

A private key (stored securely on the local system)

A public key (used to grant access)

Key-based authentication is:

More secure than passwords

Widely used in cloud platforms (AWS, Azure, GCP)

Essential for automation and CI/CD workflows

2. Understanding the .ssh Directory

After generating keys, I explored the .ssh directory to verify key files.

ls ~/.ssh


✔️ This helped me understand:

Where SSH stores authentication files

The role of id_rsa and id_rsa.pub

Why correct file permissions matter for SSH security

3. Accessing a Remote System Using SSH

I tested real-world usage by accessing a remote Ubuntu system over SSH.

ssh <username>@<remote-ip>


✔️ This validated that:

SSH service was working correctly

Network connectivity was stable

Authentication was successful

This step made SSH feel practical and real, not just theoretical.

4. Introduction to Disk & System Monitoring Commands

Beyond SSH, I explored essential Linux commands used daily by system administrators:

df -h
du
vmstat
ps
nohup


✔️ These tools help with:

Diagnosing disk space issues

Monitoring system load and performance

Managing long-running background processes

I focused on understanding when and why to use these commands—not just memorizing syntax.

Key Takeaway

Day 3 highlighted that Linux administration is about trust, visibility, and control.

SSH key-based authentication ensures secure access, while system monitoring commands provide insight into how a system behaves under real workloads.

Together, these skills form the foundation of reliable Linux and cloud operations.

Reflection

Learning Linux step by step is making complex systems feel structured, predictable, and powerful.

Consistency continues to be the key 🔑
