# Linux Learning Journey – Week 03 | Day 01  
## Auditing Users & Groups in Linux

### Overview
After learning how to create, manage, and secure users and groups in the previous module, **Day 01 of Week 03** focuses on **querying, auditing, and verifying user and group information** in Linux.

In real-world Linux servers and cloud environments, administrators must not only manage identities but also **inspect, validate, and troubleshoot access-related issues**.  
This day covers the essential commands used to safely retrieve user and group information from the system.

---

## 📂 User & Group Databases in Linux

Linux stores identity-related data in centralized system databases:

- `/etc/passwd` – User account information
- `/etc/group` – Group information
- `/etc/shadow` – Encrypted passwords and aging data

⚠️ **Note:**  
Directly reading or modifying these files is **not recommended**. Linux provides standard utilities to safely access this information.

---

## 🔍 User & Group Lookup Commands

The following commands are used to query user and group data:

## List Users

```bash
getent passwd

Displays all system users.

getent passwd <username>


Displays details of a specific user.

List Groups
getent group


Displays all system groups.

getent group <groupname>


Displays details of a specific group.

Check Group Membership
groups


Shows groups of the current user.

groups <username>


Shows groups of a specific user.

✅ Key Learnings

Through hands-on practice, I learned:

How Linux retrieves user and group information from system databases

How to verify whether a user or group exists

How to confirm group memberships in production environments

How these commands assist in auditing and debugging permission issues

🔐 Why These Commands Matter

These commands are critical because:

Editing system files directly is unsafe

Cloud and enterprise systems require strict access verification

Most permission-related issues start with user or group misconfiguration

These tools work consistently across Linux distributions

🚀 Day 01 Takeaway

This session strengthened my ability to inspect and validate Linux user and group configurations.

I now have clarity on:

Safely viewing all users and groups

Verifying group memberships for any user

Troubleshooting access and permission issues

Preparing for real-world system administration and DevOps tasks

User and group management doesn’t end with creation—visibility and verification are equally important in secure Linux environments.

Consistency is the real superpower 🔑💪
