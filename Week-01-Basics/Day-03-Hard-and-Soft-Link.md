# 🐧 Day 3 – Understanding Hard Links & Soft Links in Linux

## 📌 Objective
To understand how Linux links work at the filesystem level by exploring the differences between **Soft (Symbolic) Links** and **Hard Links**, supported by hands-on command-line demonstrations.

---

## 🔹 Soft Link (Symbolic Link)

A **soft link** (symbolic link) acts like a shortcut that points to the **file path** of the original file.

### 🛠️ Command Used
```bash
ln -s Myfile.txt softlink
🔍 Verification
ls
cat softlink
👀 Observations
The symbolic link appears alongside the original file

Accessing the soft link displays the same content as the original file

If the original file is deleted, the soft link becomes broken

✅ Key Points
References the file path

Can work across different filesystems

Similar to shortcuts in Windows

Dependent on the original file’s existence

🔹 Hard Link
A hard link directly points to the same inode (actual data) on disk.

🛠️ Command Used
ln File.txt hardlink-file
🔍 Verification
ls
cat hardlink-file
👀 Observations
Both filenames appear as independent files

Both point to the same underlying data

Deleting one filename does not remove the data

✅ Key Points
Shares the same inode

Cannot cross different filesystems

Changes via one link are reflected in the other

Data exists as long as at least one hard link remains

🔁 Soft Link vs Hard Link
Feature	Soft Link (Symbolic)	Hard Link
References	File path	Inode
Cross filesystem	✅ Yes	❌ No
Breaks if original deleted	✅ Yes	❌ No
Shares inode	❌ No	✅ Yes
Acts like shortcut	✅ Yes	❌ No
🧠 Learning Outcome
This exercise helped me understand how Linux manages files internally, the importance of inodes, and how links are used in real-world Linux systems.

Some days are about depth, not speed 🚀
This topic strengthened my foundation for advanced Linux concepts.

⏭️ Next Step
➡️ Day 4 – Exploring more core Linux commands to improve daily terminal confidence.

📌 Part of My Linux Learning Playbook
📘 Daily terminal practice
✍️ Dev.to technical articles
📂 GitHub documentation & playbooks
