# Day 3 – Understanding Hard Links & Soft Links 🔗🐧

## 1. Soft Link (Symbolic Link)
- **Definition:** A soft link is a special type of file that points to another file or directory by its path. It acts like a shortcut.  
- **Command to create:**  
  ```bash
  ln -s Myfile.txt softlink
````

* **Characteristics:**

  * References the file path, not the actual data.
  * If the original file is deleted, the link becomes broken.
  * Can link to files across different filesystems.

---

## 2. Hard Link

* **Definition:** A hard link is a directory entry that points directly to the same inode (data) as the original file.
* **Command to create:**

  ```bash
  ln File.txt hardlink-file
  ```
* **Characteristics:**

  * References the actual data on disk, not the path.
  * Deleting one filename does not remove the data if another hard link exists.
  * Changes through any link reflect on all links.
  * Cannot link across different filesystems.

---

## 3. Key Differences

| Feature                  | Soft Link                | Hard Link                                      |
| ------------------------ | ------------------------ | ---------------------------------------------- |
| Reference                | File path                | Inode (actual data)                            |
| Dependency               | Original file must exist | Independent if another link exists             |
| Cross-filesystem support | Yes                      | No                                             |
| Deleting original file   | Link breaks              | Data remains via other links                   |
| Shortcut behavior        | Acts like a shortcut     | Acts as another filename pointing to same data |

---

## 4. Summary

* **Soft links** are shortcuts dependent on the original file.
* **Hard links** are equal references to the same data, independent of filenames.
* Understanding these is essential for Linux file management, backups, and system administration.
