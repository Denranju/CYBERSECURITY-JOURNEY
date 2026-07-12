# 🐧 03-Linux

## Overview

This folder documents the Linux concepts, commands and practical skills I have learned since beginning my cybersecurity journey in **May 2026**.

The knowledge documented here was primarily gained through **Hack The Box Academy**, where I completed the **Linux Fundamentals** and **Introduction to Bash Scripting** modules, together with practical exercises in **OverTheWire Bandit**.

Linux is one of the most widely used operating systems in cybersecurity. It powers servers, cloud infrastructure and many security tools, making Linux proficiency an essential skill for penetration testing, digital forensics, system administration and security operations.

---

# 📅 Learning Journey

I began learning Linux in **May 2026** after completing my networking studies on Hack The Box Academy.

During my studies I learned how to navigate the Linux operating system, manage files and directories, understand file permissions, connect securely using SSH, automate tasks with Bash scripting and solve practical Linux challenges through OverTheWire Bandit.

These practical exercises strengthened my understanding of the Linux command line and prepared me for more advanced cybersecurity topics.

---

# 🎓 Learning Platform

- Hack The Box Academy
- OverTheWire Bandit

---

# ✅ Modules Completed

- Linux Fundamentals
- Introduction to Bash Scripting

---

# 🎯 Learning Objectives

The objectives of these modules were to:

- Understand the Linux operating system.
- Learn the Linux file system.
- Navigate using the command line.
- Manage files and directories.
- Understand Linux permissions.
- Learn secure remote access using SSH.
- Understand SSH key authentication.
- Learn Bash scripting fundamentals.
- Develop Linux skills required for cybersecurity.

---

# 📚 Topics Covered

## Linux

Linux is a free and open-source operating system widely used in cybersecurity, cloud computing, servers and enterprise environments.

Most penetration testing distributions, including Kali Linux and Parrot OS, are Linux-based.

---

## Linux File System

The Linux file system is organized in a hierarchical structure beginning at the root directory (`/`).

Important directories include:

`/home` – User home directories.

`/etc` – System configuration files.

`/var` – Log files and variable data.

`/tmp` – Temporary files.

`/bin` – Essential user commands.

`/usr` – User applications and utilities.

`/root` – Home directory for the root user.

`/dev` – Device files.

`/proc` – Process and kernel information.

---

## Basic Linux Commands

### Navigation

```bash
pwd
```

Displays the current working directory.

```bash
ls
```

Lists files and directories.

```bash
ls -la
```

Lists all files including hidden files.

```bash
cd
```

Changes directories.

---

### File Management

```bash
mkdir
```

Creates a directory.

```bash
rmdir
```

Removes an empty directory.

```bash
touch
```

Creates a new file.

```bash
cp
```

Copies files or directories.

```bash
mv
```

Moves or renames files.

```bash
rm
```

Removes files or directories.

---

### Viewing Files

```bash
cat
```

Displays file contents.

```bash
less
```

Views large files.

```bash
head
```

Displays the beginning of a file.

```bash
tail
```

Displays the end of a file.

---

### Searching

```bash
find
```

Searches for files and directories.

```bash
grep
```

Searches for specific text inside files.

---

### User Information

```bash
whoami
```

Displays the current user.

```bash
id
```

Displays user and group information.

```bash
history
```

Displays previously executed commands.

---

## File Permissions

Linux uses file permissions to determine who can read, write and execute files.

Permission types include:

- Read (r)
- Write (w)
- Execute (x)

Permissions are assigned to:

- Owner
- Group
- Others

Common permission commands include:

```bash
chmod
```

Changes file permissions.

```bash
chown
```

Changes file ownership.

Understanding permissions is essential for securing Linux systems.

---

## SSH (Secure Shell)

SSH allows encrypted remote access to Linux systems.

Example:

```bash
ssh username@hostname
```

Using a private key:

```bash
ssh -i sshkey.private bandit14@localhost -p 2220
```

SSH provides secure authentication and encrypted communication between systems.

---

## SSH Key Management

Generate a new SSH key pair:

```bash
ssh-keygen
```

Extract the public key:

```bash
ssh-keygen -y -f sshkey.private
```

I learned the difference between public and private SSH keys and how key-based authentication improves security.

---

## Base64 Encoding

Base64 converts binary data into text and is commonly used in web applications, email and authentication.

Decode Base64:

```bash
base64 -d filename
```

Understanding Base64 is useful when analysing encoded data during security assessments.

---

## Bash Scripting

Bash scripting allows Linux users to automate repetitive tasks.

During the Hack The Box Academy module I learned how to:

- Create Bash scripts.
- Use variables.
- Accept user input.
- Work with loops.
- Use conditional statements.
- Automate command execution.
- Improve efficiency through scripting.

---

## OverTheWire Bandit

As part of my practical Linux training I completed **Bandit Level 13**.

During these challenges I learned how to:

- Navigate Linux systems.
- Search for hidden files.
- Work with permissions.
- Read sensitive files.
- Decode Base64 data.
- Connect using SSH.
- Authenticate using SSH private keys.
- Understand the difference between public and private SSH keys.

These practical exercises reinforced the Linux concepts learned in Hack The Box Academy.

---

# 🛠️ Practical Skills Developed

During these modules I developed practical skills in:

- Navigating the Linux operating system.
- Managing files and directories.
- Understanding Linux file permissions.
- Searching for files.
- Searching file contents.
- Using Linux command-line tools.
- Connecting securely using SSH.
- Managing SSH keys.
- Decoding Base64 data.
- Writing basic Bash scripts.
- Automating repetitive tasks.
- Solving Linux-based security challenges.

---

# 💻 Tools and Technologies

During this stage of my learning journey I used:

- Ubuntu Linux
- Kali Linux
- Hack The Box Academy
- OverTheWire Bandit
- Bash
- OpenSSH
- Git
- GitHub
- Visual Studio Code
- Windows Terminal

---

# 🌍 Real-World Applications

The Linux knowledge gained during these modules is directly applicable to:

- Penetration Testing
- Security Operations Centers (SOC)
- Cloud Computing
- Server Administration
- Digital Forensics
- Incident Response
- Malware Analysis
- System Administration
- Automation

---

# ✅ Best Practices

- Follow the principle of least privilege.
- Use strong passwords and SSH keys.
- Keep Linux systems updated.
- Restrict unnecessary services.
- Secure file permissions.
- Regularly monitor log files.
- Automate repetitive administrative tasks.
- Back up important system data.

---

# 📖 Source

- Hack The Box Academy – Linux Fundamentals
- Hack The Box Academy – Introduction to Bash Scripting
- OverTheWire – Bandit

---

# 📌 Summary

Completing the **Linux Fundamentals** and **Introduction to Bash Scripting** modules, together with practical exercises in **OverTheWire Bandit**, provided me with a strong foundation in Linux system administration and command-line usage.

I learned how to navigate Linux systems, manage files and permissions, connect securely using SSH, automate tasks with Bash scripting and solve practical Linux challenges. These skills form a critical foundation for penetration testing, web security, digital forensics and advanced cybersecurity studies.