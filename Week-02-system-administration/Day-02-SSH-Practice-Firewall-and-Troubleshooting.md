# **Day 02: SSH Practice, Firewall, IP Awareness & Troubleshooting** 🐧🔧

**Week 2 – System Administration**

---

## **Overview**
After configuring SSH on Day 1, Day 2 focused on **practice, verification, and troubleshooting**—the skills that matter most when working with real Linux servers in **cloud and production environments**.

Rather than rushing into new topics, I strengthened the fundamentals that ensure **stable, secure, and reliable remote access**.

---

## **What I Practiced**

### **1. Network Connectivity Verification**
Before using SSH, I verified that the Ubuntu system was reachable on the network.

```bash
ping <server-ip>

2. Verifying Remote SSH Session

After connecting via SSH, I confirmed the remote session by checking the current directory and listing files.

pwd
ls


✔️ These commands confirmed that:

I was logged into the remote Ubuntu system

I had access to my home directory

The SSH session was active and stable

3. Firewall Configuration for SSH (UFW)

To ensure SSH access was not blocked, I verified firewall rules.

sudo ufw allow ssh
sudo ufw status


✔️ This confirmed that:

Port 22 was allowed

Firewall rules were applied correctly

4. Checking System IP Address

Since IP addresses may change, I practiced identifying the system IP using:

ip a
hostname -I


✔️ IP awareness is critical for reliable remote access.

5. Restarting SSH Service

To simulate real-world troubleshooting, I restarted the SSH service and verified its status.

sudo systemctl restart ssh
sudo systemctl status ssh


✔️ Restarting services is a common system administration task.

6. Reconnecting from Windows

Finally, I reconnected to the Ubuntu system from Windows Command Prompt.

ssh <username>@<server-ip>


✔️ Successful login confirmed that:

SSH service was running correctly

Firewall rules were properly configured

Network connectivity was stable

Key Takeaway

Linux mastery isn’t just about memorizing commands—it’s about practice, verification, and understanding system behavior.

Repeatedly checking network connectivity, firewall rules, and SSH services improved my troubleshooting confidence and made Linux feel more predictable and powerful.

Reflection

Day 2 reinforced the importance of validating every layer of remote access. These practical checks mirror real-world production scenarios and are essential for anyone managing Linux servers in cloud and DevOps environments.
