# Lab 34: Simple Scripting for File Management

## Objective

The objective of this lab is to automate file management tasks using Python. The script lists files, copies them to a backup directory, and renames them during the backup process.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Complete Code

```python
import os
import shutil

source_directory = "source_files"
destination_directory = "backup_files"

if not os.path.exists(destination_directory):
    os.makedirs(destination_directory)

files = os.listdir(source_directory)

print("Files Found:")
print(files)

for file in files:

    source_path = os.path.join(
        source_directory,
        file
    )

    base, extension = os.path.splitext(file)

    new_name = f"{base}_backup{extension}"

    destination_path = os.path.join(
        destination_directory,
        new_name
    )

    shutil.copy(source_path, destination_path)

    print(f"Copied: {file} → {new_name}")

print("\nBackup Completed Successfully!")
```

---

## Output

```text
Files Found:
['file1.txt', 'file2.txt', 'file3.txt']

Copied: file1.txt → file1_backup.txt
Copied: file2.txt → file2_backup.txt
Copied: file3.txt → file3_backup.txt

Backup Completed Successfully!
```

---

## Key Concepts

### os Module

Used for interacting with the operating system.

### shutil Module

Used for copying and moving files.

### os.listdir()

Lists files inside a directory.

### os.makedirs()

Creates directories.

### shutil.copy()

Copies files from source to destination.

### os.path.splitext()

Separates filename and extension.

---

## Real-World Applications

* File backup automation
* Log archiving
* Security evidence collection
* Report management
* Bulk file processing

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output and backup folder contents.

---

## Skills Learned

* Listing files
* Creating directories
* Copying files
* Renaming files
* Automating repetitive tasks

---

## Conclusion

This lab demonstrated how Python can automate file management tasks. By combining the os and shutil modules, repetitive operations such as file listing, copying, and renaming can be performed efficiently and accurately.
