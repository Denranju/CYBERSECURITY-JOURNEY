# 📜 05-Bash-Scripting

## Overview

This folder contains the Bash scripting concepts, commands and automation techniques I have learned since beginning my cybersecurity journey in **May 2026**.

The knowledge documented here was gained primarily through **Hack The Box Academy**, practical Linux exercises and personal practice. Bash scripting enables automation of repetitive tasks, improves efficiency and is an essential skill for Linux system administration and cybersecurity.

---

# 📅 Learning Journey

After developing a foundation in Linux, I began learning Bash scripting to automate command-line tasks and improve productivity.

Bash scripts allow multiple Linux commands to be combined into reusable programs, making system administration and cybersecurity tasks faster and more efficient.

---

# 🎯 Learning Objectives

The objectives of learning Bash scripting include:

- Understanding Bash syntax.
- Writing simple Bash scripts.
- Automating repetitive tasks.
- Working with variables.
- Using conditional statements.
- Creating loops.
- Writing reusable functions.
- Managing files through scripts.
- Building a foundation for cybersecurity automation.

---

# 📚 Topics Covered

## What is Bash?

Bash (Bourne Again Shell) is the default command-line shell on many Linux systems. It provides an interface for interacting with the operating system and supports scripting for task automation.

---

## Creating a Bash Script

A Bash script is created as a text file and begins with a shebang line.

Example:

```bash
#!/bin/bash
echo "Hello World"
```

---

## Variables

Variables store data for use throughout a script.

Example:

```bash
name="Denranju"
echo $name
```

---

## User Input

Scripts can accept input from users.

Example:

```bash
read -p "Enter your name: " name
echo "Welcome $name"
```

---

## Conditional Statements

Conditional statements allow scripts to make decisions.

Example:

```bash
if [ -f file.txt ]
then
    echo "File exists."
else
    echo "File not found."
fi
```

---

## Loops

### For Loop

```bash
for i in {1..5}
do
    echo $i
done
```

### While Loop

```bash
count=1

while [ $count -le 5 ]
do
    echo $count
    count=$((count+1))
done
```

---

## Functions

Functions allow reusable blocks of code.

Example:

```bash
greet() {
    echo "Welcome to Bash!"
}

greet
```

---

## File Operations

Common operations include:

- Creating files
- Copying files
- Moving files
- Deleting files
- Checking file existence

Example:

```bash
touch file.txt
cp file.txt backup.txt
mv backup.txt newfile.txt
rm newfile.txt
```

---

## Permissions

Scripts require execute permissions before they can run.

Grant permission:

```bash
chmod +x script.sh
```

Run the script:

```bash
./script.sh
```

---

## Common Bash Commands

```bash
pwd
ls
cd
mkdir
rm
cp
mv
cat
grep
find
chmod
whoami
history
```

---

## Bash in Cybersecurity

Bash scripting is commonly used for:

- System administration
- Log analysis
- File management
- Network automation
- Security auditing
- Reconnaissance
- Automation of repetitive tasks
- Running security tools

---

# 🛠️ Practical Skills Developed

Through Bash scripting I developed skills in:

- Writing Bash scripts.
- Working with variables.
- Accepting user input.
- Creating conditional statements.
- Using loops.
- Writing functions.
- Managing files.
- Executing scripts.
- Automating Linux tasks.
- Improving command-line efficiency.

---

# 💻 Tools Used

During this stage of my learning I used:

- Hack The Box Academy
- Ubuntu Linux
- Kali Linux
- Windows Subsystem for Linux (WSL)
- Visual Studio Code
- Linux Terminal
- Git
- GitHub

---

# 📖 Learning Resources

The knowledge documented in this folder was gained through:

- Hack The Box Academy
- Linux command-line practice
- Official Bash documentation
- Personal scripting exercises

---

# 📌 Summary

Learning Bash scripting has strengthened my Linux and cybersecurity skills by enabling me to automate repetitive tasks and better understand the Linux command-line environment. As I continue my cybersecurity journey, I will expand this folder with more advanced automation scripts, system administration tasks and security-focused Bash projects.