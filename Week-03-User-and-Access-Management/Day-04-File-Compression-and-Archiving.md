# Day-04: File Compression & Archiving in Ubuntu

## Overview
File compression and archiving are essential Linux skills used daily by **System Administrators, DevOps Engineers, and Cloud Professionals**.  
They help optimize storage, simplify backups, and improve data transfer efficiency across systems.

This session focused on understanding **when and how to compress data effectively** in real-world environments.

---

## Why Compression & Archiving Matter
In production and cloud systems, administrators frequently handle:
- Application source code
- Backup archives
- Log files
- Deployment artifacts
- Server-to-server data transfers

Proper compression helps to:
- Reduce disk usage
- Speed up file transfers
- Bundle multiple files into a single archive
- Maintain organized and manageable systems

---

## Archiving vs Compression
- **Archiving** combines multiple files into one file
- **Compression** reduces file size

Linux commonly uses **tar for archiving** and **gzip for compression**, often together.

---

## Commands Practiced

### zip — Cross-Platform Compression
Creates `.zip` archives compatible across operating systems.

Common use:

Sharing files with Windows or macOS users

unzip — Extract ZIP Archives
unzip project.zip


Used to extract .zip files.

tar -cvzf — Create Compressed Archive

Creates a .tar.gz archive using gzip compression.

tar -cvzf backup.tar.gz backup/


Flags:

c → create archive

v → verbose output

z → gzip compression

f → file name

Used for:

Server backups

Application packaging

Cloud deployments

tar -xvzf — Extract tar.gz Archive
tar -xvzf backup.tar.gz


Safely extracts compressed tar files.

gzip — Compress Files

Compresses a file and replaces it with .gz.

gzip logfile.txt


Result:

logfile.txt.gz

gunzip — Decompress Files

Restores original file from .gz.

gunzip logfile.txt.gz

Practical Learnings

.tar.gz is the standard for Linux servers

.zip is best for cross-platform sharing

Compression improves backup and deployment workflows

Large directories must be handled carefully to avoid data loss

These tools are foundational for DevOps operations

Summary

File compression is not optional in Linux environments—it is a core operational skill.

Efficient storage, faster transfers, and clean system organization depend on using the right tools correctly.

Small skills, practiced daily, build Linux mastery.

```bash
zip -r project.zip project/
