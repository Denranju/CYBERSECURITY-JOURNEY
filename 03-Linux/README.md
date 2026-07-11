# 03-Linux

# 🐧 03-Linux

## Overview

This folder contains the Linux concepts, commands and practical skills I have learned during my cybersecurity journey.

## Linux

Linux is an open-source operating system widely used in servers, cloud computing and cybersecurity. It provides powerful command-line tools for system administration, penetration testing and automation.

## Linux File System

The Linux file system is organized in a hierarchical structure starting from the root directory (`/`).

Some important directories include:

`/home` stores user files.

`/etc` contains system configuration files.

`/var` stores logs and variable data.

`/tmp` stores temporary files.

`/bin` contains essential user commands.

`/usr` contains user applications and utilities.

## Basic Linux Commands

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

Lists all files, including hidden files, with detailed information.

```bash
cd
```

Changes the current directory.

```bash
mkdir
```

Creates a new directory.

```bash
rmdir
```

Removes an empty directory.

```bash
touch
```

Creates an empty file.

```bash
cp
```

Copies files or directories.

```bash
mv
```

Moves or renames files and directories.

```bash
rm
```

Deletes files or directories.

```bash
cat
```

Displays the contents of a file.

```bash
less
```

Views large files one page at a time.

```bash
head
```

Displays the first lines of a file.

```bash
tail
```

Displays the last lines of a file.

```bash
find
```

Searches for files and directories.

```bash
grep
```

Searches for specific text inside files.

```bash
chmod
```

Changes file permissions.

```bash
chown
```

Changes file ownership.

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

## File Permissions

Linux permissions determine who can read, write and execute a file.

Permission types include:

Read (r)

Write (w)

Execute (x)

Permissions apply to the owner, group and others.

## SSH

Secure Shell (SSH) allows secure remote access to another computer over a network.

Example:

```bash
ssh username@hostname
```

Using a private key:

```bash
ssh -i sshkey.private bandit14@localhost -p 2220
```

## SSH Key Management

```bash
ssh-keygen
```

Generates a new SSH key pair.

```bash
ssh-keygen -y -f sshkey.private
```

Extracts the public key from a private key.

## Base64

Base64 is an encoding method used to convert binary data into text. It is commonly used in web applications, email and authentication.

Decode a Base64 string:

```bash
base64 -d filename
```

## OverTheWire Bandit

I completed Bandit Level 13.

During this level I learned how to authenticate using SSH private keys, connect securely to another account and understand the difference between public and private SSH keys.

## Skills Gained

I learned how to navigate the Linux file system, manage files and directories, work with permissions, search files, connect to remote systems using SSH, manage SSH keys, decode Base64 data and solve Linux challenges in OverTheWire Bandit.
Notes for 03-Linux go here.
