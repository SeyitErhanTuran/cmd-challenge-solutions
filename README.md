# CMD Challenge Solutions

This repository contains my personal solutions to the [CMD Challenge](https://cmdchallenge.com) exercises.  
Questions are from [cmdchallenge.com](https://cmdchallenge.com).

## 📑 Table of Contents
1. [Print "hello world"](#1-print-hello-world)  
2. [Print the current working directory](#2-print-the-current-working-directory)
3. [List files in the current directory](#3-list-files-in-the-current-directory)
4. [Display the contents of access.log](#4-display-the-contents-of-accesslog)
5. [Print the last 5 lines of access.log](#5-print-the-last-5-lines-of-accesslog)
6. [Create an empty file named take-the-command-challenge](#6-create-an-empty-file-named-take-the-command-challenge)
7. [Create a directory tmp/files](#7-create-a-directory-tmpfiles)






---

## 1) Print "hello world"
**Task:** Print "hello world" on the terminal in a single command.  

**My Solution:**
```bash
echo "hello world"
```

---

## 2) Print the current working directory
**Task:** Print the path of the current working directory.  

**My Solution:**
```bash
pwd
```

---

## 3) List files in the current directory
**Task:** List names of all the files in the current directory, one file per line.  

**My Solution:**
```bash
ls
```

---

## 4) Display the contents of access.log
**Task:** There is a file named `access.log` in the current directory. Print the contents.  

**My Solution:**
```bash
cat access.log
```

---

## 5) Print the last 5 lines of access.log
**Task:** Print the last 5 lines of the file `access.log`.  

**My Solution:**
```bash
tail -n 5 access.log
```
Note:
By default, tail prints the last 10 lines of a file.
The -n option lets you specify how many lines you want.

---

## 6) Create an empty file named take-the-command-challenge
**Task:** Create an empty file named `take-the-command-challenge` in the current working directory.  

**My Solution:**
```bash
touch take-the-command-challenge
```

---

## 7) Create a directory tmp/files
**Task:** Create a directory named `tmp/files` in the current working directory.  

**My Solution:**
```bash
mkdir -p tmp/files
```
Note:
Without -p, the command would fail if tmp doesn’t exist.

---



