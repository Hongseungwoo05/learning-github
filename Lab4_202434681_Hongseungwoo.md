# Lecture 4: CLI (Command Line Interface) - Part 1
**202434681 Hong Seung Woo**  

---


## 1. Kernel and Shell

- **Kernel**: Core of the OS that communicates with hardware.
- **Shell**: Interface for users to interact with the kernel (e.g., bash, zsh).

---

## 2. CLI vs GUI

| **CLI (Command Line Interface)**           | **GUI (Graphical User Interface)**        |
|--------------------------------------------|-------------------------------------------|
| Requires memorizing commands               | Easy to use and intuitive                 |
| Primarily uses keyboard                    | Primarily uses mouse (with some shortcuts)|
| Relatively fast                            | Relatively slow                           |
| Enables automation and scripting           | Requires manual labor for repetitive tasks|
| Preferred by developers                    | Preferred by daily users                  |

---

## 3. Basic Shell Commands

### 3.1 `pwd` – Print Working Directory
Shows the current path in a hierarchical directory.

### 3.2 `cd` – Change Directory
- **Usage**: `cd [directory name]`
- **Special arguments**:
  - `/`: Root directory
  - `. `: Current directory
  - `..`: Parent directory
  - `~`: Home directory
  - `/[directory name]`: Absolute path
  - `./[directory name]`, `../[directory name]`: Relative path

### 3.3 `ls` – List Files and Directories
- **Usage**: `ls`
- **Options**:
  - `-l`: Show detailed information (long format)
  - `-lh`: Same as above, but size is shown in human-readable units.

---

## 4. Tips for Shell Usage

- **Autocompletion**: Press the `Tab` key.
- **Previous Commands**: Use the `Up Arrow` key to view past commands.
- **Clear Screen**: Use the command `clear`.

---

## 5. File and Directory Manipulation

**Warning**: Some commands may delete or overwrite your files! Backup important data before using them.

### 5.1 `cp` – Copy Files and Directories
- **Usage**: `cp [options] [source] [destination]`
- Copies files or directories from the source path to the destination.
- **Common Options**:
  - `-r` (recursive): Required when copying directories (i.e., includes all subdirectories and files).
  - `-i` (interactive): Prompts the user before overwriting files.


### 5.2 `mv` – Move or Rename Files and Directories
- Usage: mv [options] [source] [destination]
Moves files or directories from the source to the destination. Can also be used to rename files or directories.
- **Common Options**:
-`i` (interactive): Prompts the user before overwriting files.
-`v` (verbose): Shows the process of moving files.


### 5.3 `rm` – Remove Files and Directories
- Usage: rm [options] [file/directory]
Deletes files or directories permanently. Use with caution as this action cannot be undone.
- **Common Options**:
-`r` (recursive): Deletes directories and their contents.
-`i` (interactive): Prompts before each file deletion.


### 5.4 `mkdir` – Make a New Directory
- **Usage**: `mkdir [directory name]`

### 5.5 Wildcards

#### Common Wildcards:
- `*` (Asterisk): Matches zero or more characters.
  - Example: `*.txt` matches all files ending with `.txt`, such as `file1.txt`, `notes.txt`, etc.
  
- `?` (Question Mark): Matches exactly one character.
  - Example: `file?.txt` matches `file1.txt`, `file2.txt`, but not `file10.txt` (as it has more than one character after `file`).

- `[ ]` (Brackets): Matches any one of the enclosed characters.
  - Example: `file[12].txt` matches `file1.txt` and `file2.txt`, but not `file3.txt`.

- `[ - ]` (Hyphen): Used inside brackets to specify a range of characters.
  - Example: `file[a-z].txt` matches `filea.txt`, `fileb.txt`, ..., `filez.txt`.
  - Example: `file[1-9].txt` matches `file1.txt`, `file2.txt`, ..., `file9.txt`.
---

## 6. Help Commands

- `help`: Basic help for shell built-in commands.
- `man`: Detailed manual for shell commands.

---

## 7. Exiting the Terminal
- Use the `exit` command to close the terminal.

---
