# Linux Learning Journey – Day 4: File Handling & Text Processing 🐧

**Objective:**  
Learn and practice basic file handling and text processing commands in Linux, essential for daily tasks, cloud work, and DevOps automation.

---

## 1️⃣ Writing Output to Files

**Command:** `echo` + `tee`  

Create a file and display the content on the terminal:

```bash
echo "Hello friends, how are you?" | tee Myfile.txt
Tip for beginners:

echo prints text to the terminal

tee writes output to a file and shows it on the terminal

2️⃣ Editing Files with vi
Open a file in the vi editor:

vi Myfile.txt
Basic vi commands for beginners:

Action	Command
Enter Insert mode	i
Save	:w
Save & Exit	:wq
Exit without saving	:q!
Tip: vi is installed on almost all Linux systems. Learning it is very useful for editing configuration files and scripts.

3️⃣ Sorting Text Data
Command: sort

Sort lines alphabetically:

sort Myfile.txt
sort Mail.txt
Use cases:

Organizing logs

Sorting email lists

Managing structured text data

4️⃣ Extracting Specific Characters
Command: cut

Extract selected bytes or characters:

cut -b 1-3 Mail.txt
Use cases:

Extract usernames or IDs from files

Work with fixed-format text files

Tip: -b is for bytes, -c is for characters. Beginners can start with -b.

5️⃣ Comparing Files
Command: diff

Identify differences between two files:

diff Myfile.txt Mail.txt
Use cases:

Compare configuration files

Audit changes

Troubleshoot issues

📌 Key Learnings (Day 4)
Linux text commands are powerful when combined

Small commands can solve complex problems

File and text handling is the foundation for cloud and DevOps tasks

🚀 Reflection
Day 4 focused on hands-on practice. Repeating these commands built confidence in using the terminal, which is essential for working on real Linux servers.

Next step: Day 5 – More Linux learning and practical exercises.
