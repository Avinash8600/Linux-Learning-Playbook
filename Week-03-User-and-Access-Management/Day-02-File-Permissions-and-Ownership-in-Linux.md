# Day-02: Linux File Permissions & Ownership

## Introduction
File permissions and ownership define how Linux controls access to files and directories.  
They are a foundational security mechanism used across **servers, cloud platforms, and production systems** to protect data and ensure correct application behavior.

Understanding these concepts helps prevent misconfigurations that commonly lead to system errors and security risks.

---

## Importance of Permissions in Linux
Proper permission management helps to:
- Restrict unauthorized file access
- Prevent accidental data modification
- Ensure applications run with correct privileges
- Maintain system integrity in multi-user environments

Linux enforces access control at the file system level through ownership and permission rules.

---

## Permission Structure

### Permission Categories
Each file or directory defines permissions for:
- **Owner** – The user who owns the file
- **Group** – Users belonging to the assigned group
- **Others** – All remaining users

---

### Permission Types
| Permission | Description |
|-----------|------------|
| Read (r) | View file content or list directory |
| Write (w) | Modify file or directory contents |
| Execute (x) | Run file or access directory |

---

## Inspecting Permissions

### `ls -l`
Displays detailed permission and ownership information:
```bash
ls -l

Example:

drwxr-x--- 2 avinash dev 4096 project/


This output shows:

Directory type

Permission bits

Owner and group association

Modifying File Permissions
Symbolic Method
chmod u+x script.sh
chmod g+r report.txt
chmod o-w data.csv

Numeric Method
Value	Access
7	Read, Write, Execute
6	Read, Write
5	Read, Execute
4	Read

Example:

chmod 750 deploy.sh
chmod 640 config.conf

Managing Ownership
Changing File Owner
sudo chown appuser file.log
sudo chown appuser:appgroup file.log


Used commonly for:

Application services

Log and configuration files

Deployment directories

Changing Group Ownership
sudo chgrp developers project/


Allows controlled access without making files publicly accessible.

Default Permission Behavior
umask

Defines default permission settings for newly created files:

umask


Example:

0027


Effect:

Files → 640

Directories → 750

This reduces unnecessary exposure by default.

Common Permission Issues
Permission Denied Errors

Often caused by:

Missing execute permission on directories

Incorrect ownership assignment

Overly restrictive default permissions

Basic checks:

ls -l
id
namei -l filename

Practical Takeaways

File permissions are a primary Linux security control

Ownership determines which users and services can access resources

Default permissions should follow the principle of least privilege

Most access-related errors can be traced to permission misconfiguration

Summary

Correct permission and ownership management is essential for building secure, stable, and maintainable Linux systems.

A strong understanding of these fundamentals is critical for System Administrators, Cloud Engineers, and DevOps professionals.
