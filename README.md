# CMD Challenge Solutions

This repository contains my personal solutions to the [CMD Challenge](https://cmdchallenge.com) exercises.  
Questions are from [cmdchallenge.com](https://cmdchallenge.com).

## 📑 Table of Contents
1.  [Hello World](#1-hello-world)  
2.  [Current Working Directory](#2-current-working-directory)
3.  [List Files](#3-list-files)
4.  [File Contents](#4-file-contents)
5.  [Last Lines](#5-last-lines)
6.  [Create a File](#6-create-a-file)
7.  [Create a Directory](#7-create-a-directory)
8.  [Copy File](#8-copy-file)
9.  [Move File](#9-move-file)
10. [Symbolic Link](#10-symbolic-link)

       
---

## 📑 Table of Contents

| 1. [Hello World](#1-hello-world) | 2. [Current Working Directory](#2-current-working-directory) | 3. [List Files](#3-list-files) | 4. [File Contents](#4-file-contents) |
|----------------------------------|--------------------------------------------------------------|--------------------------------|--------------------------------------|
| 5. [Last Lines](#5-last-lines)   | 6. [Create a File](#6-create-a-file)                        | 7. [Create a Directory](#7-create-a-directory) | 8. [Copy a File](#8-copy-a-file) |
| 9. [Move a File](#9-move-a-file) | 10. [Symbolic Link](#10-symbolic-link)                      | 


---

## 1) Hello World
**Task:** Print "hello world" on the terminal in a single command.  

**My Solution:**
```bash
echo "hello world"
```

---

## 2) Current Working Directory
**Task:** Print the path of the current working directory.  

**My Solution:**
```bash
pwd
```

---

## 3) List Files
**Task:** List names of all the files in the current directory, one file per line.  

**My Solution:**
```bash
ls
```

---

## 4) File Contents
**Task:** There is a file named `access.log` in the current directory. Print the contents.  

**My Solution:**
```bash
cat access.log
```

---

## 5) Last Lines
**Task:** Print the last 5 lines of the file `access.log`.  

**My Solution:**
```bash
tail -n 5 access.log
```
Note:
By default, tail prints the last 10 lines of a file.
The -n option lets you specify how many lines you want.

---

## 6) Create a File
**Task:** Create an empty file named `take-the-command-challenge` in the current working directory.  

**My Solution:**
```bash
touch take-the-command-challenge
```

---

## 7) Create a Directory
**Task:** Create a directory named `tmp/files` in the current working directory.  

**My Solution:**
```bash
mkdir -p tmp/files
```
Note:
Without -p, the command would fail if tmp doesn’t exist.

---

## 8) Copy File
**Task:** Copy the file named `take-the-command-challenge` to the directory `tmp/files`.  

**My Solution:**
```bash
cp take-the-command-challenge tmp/files
```

---

## 9) Move File
**Task:** Move the file named `take-the-command-challenge` to the directory `tmp/files`.  

**My Solution:**
```bash
mv take-the-command-challenge tmp/files
```

---

## 10) Symbolic Link
**Task:** Create a symbolic link named `take-the-command-challenge` that points to the file `tmp/files/take-the-command-challenge`.  

**My Solution:**
```bash
ln -s tmp/files/take-the-command-challenge take-the-command-challenge
```
Note:
"ln -s" a symbolic (soft) link command, similar to a shortcut.
If the original file is deleted, the symlink becomes broken.
Unlike symlinks, hard links point directly to the file’s content (inode).
Editing the file through a hard link also changes the original, since they share the same data.

---



