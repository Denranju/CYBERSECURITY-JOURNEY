# 📜 08-Scripting

## Overview

This folder documents the Bash scripting concepts, syntax and automation skills I have learned since beginning my cybersecurity journey in **May 2026**.

The knowledge documented here was primarily gained through the **Hack The Box Academy – Introduction to Bash Scripting** module together with practical exercises performed in Linux.

Bash scripting is an essential skill in cybersecurity because it allows professionals to automate repetitive tasks, manage systems efficiently and develop custom tools for security assessments.

---

# 📅 Learning Journey

After developing a solid foundation in Linux, I began learning Bash scripting to improve my ability to automate tasks and interact more efficiently with Linux systems.

Through Hack The Box Academy, I learned how to create executable scripts, use variables, perform calculations, accept user input and automate command execution.

These scripting skills have improved my productivity and prepared me for more advanced penetration testing and system administration tasks.

---

# 🎓 Learning Platform

- Hack The Box Academy

---

# ✅ Module Completed

- Introduction to Bash Scripting

---

# 🎯 Learning Objectives

The objectives of this module were to:

- Understand Bash scripting fundamentals.
- Create executable Bash scripts.
- Use variables.
- Accept user input.
- Work with conditional statements.
- Use loops for automation.
- Create reusable scripts.
- Automate repetitive Linux tasks.

---

# 📚 Topics Covered

## What is Bash?

Bash (Bourne Again Shell) is the default command-line shell used on many Linux systems.

It allows users to execute commands, manage files and create scripts to automate tasks.

---

## Creating a Bash Script

Every Bash script begins with a shebang.

Example:

```bash
#!/bin/bash
```

This tells Linux to execute the script using the Bash interpreter.

---

## Variables

Variables store information that can be reused throughout a script.

Example:

```bash
name="Denran"
echo $name
```

---

## User Input

Scripts can accept input from users.

Example:

```bash
read username
echo "Welcome $username"
```

---

## Conditional Statements

Conditional statements allow scripts to make decisions.

Example:

```bash
if [ "$age" -ge 18 ]
then
    echo "Adult"
else
    echo "Minor"
fi
```

---

## Loops

Loops repeat commands multiple times.

### For Loop

```bash
for i in 1 2 3 4 5
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
    echo "Hello!"
}

greet
```

---

## Command-Line Arguments

Scripts can accept parameters passed from the command line.

Example:

```bash
echo $1
```

---

## File Permissions

Scripts must have execute permission before they can run.

Grant permission using:

```bash
chmod +x script.sh
```

Run the script:

```bash
./script.sh
```

---

## Useful Bash Commands

Display the current directory:

```bash
pwd
```

List files:

```bash
ls
```

Print text:

```bash
echo "Hello World"
```

Read a file:

```bash
cat filename
```

Display the current user:

```bash
whoami
```

Display the current date:

```bash
date
```

---

# 🛠️ Practical Skills Developed

During this module I developed practical skills in:

- Creating Bash scripts.
- Executing scripts.
- Using variables.
- Accepting user input.
- Creating conditional statements.
- Using loops.
- Writing reusable functions.
- Passing command-line arguments.
- Managing script permissions.
- Automating repetitive Linux tasks.

---

# 💻 Tools and Technologies

During this stage of my learning journey I used:

- Ubuntu Linux
- Kali Linux
- Bash
- Linux Terminal
- Visual Studio Code
- Hack The Box Academy
- Git
- GitHub

---

# 🌍 Real-World Applications

The Bash scripting knowledge gained during this module is applicable to:

- Linux System Administration
- Penetration Testing
- Security Automation
- Log Analysis
- File Management
- Task Automation
- Security Operations
- Incident Response

---

# ✅ Best Practices

- Keep scripts simple and readable.
- Use meaningful variable names.
- Add comments to explain code.
- Test scripts before deployment.
- Validate user input.
- Apply the principle of least privilege.
- Store scripts securely.
- Use version control with Git.

---

# 📖 Source

- Hack The Box Academy – Introduction to Bash Scripting

---

# 📌 Summary

Completing the **Introduction to Bash Scripting** module provided me with a strong foundation in Linux automation and scripting. I learned how to create executable scripts, use variables, accept user input, implement conditional logic, build loops and automate repetitive tasks.

These scripting skills improve efficiency when working in Linux environments and provide an essential foundation for penetration testing, system administration and cybersecurity automation.