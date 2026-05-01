<div align="center">

# 📜 Day 02 — Shell Scripting Basics & Sha-Bang

![Bash](https://img.shields.io/badge/Bash-Scripting-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Automation](https://img.shields.io/badge/Automation-Shell-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

> *"Automate the boring stuff — Shell scripting is your first superpower as a DevOps engineer."*

</div>

---

## 📌 Introduction

**Shell Scripting** is the process of writing a set of commands in a file and executing them together. It eliminates repetitive manual work and is a cornerstone skill in DevOps automation.

| Aspect | Detail |
|---|---|
| 📁 File Extension | `.sh` (e.g., `backup.sh`, `health-check.sh`) |
| ⚡ Execution | Direct — no compilation needed |
| 🔁 Use Case | Automation of daily/routine tasks |
| 🔧 Tool | Bash shell (most common) |

---

## 🧠 Key Concepts

### Scripting vs Programming

```mermaid
flowchart LR
    A[Source Code] --> B{Type?}
    B -- Programming --> C["Compiler\n(C, C++, Java, C#)"]
    B -- Scripting --> D["Direct Execution\n(Bash, Python, Perl)"]
    C --> E[Binary / Bytecode]
    D --> F[Output]
    E --> F

    style B fill:#F7931E,color:#fff
    style C fill:#E74C3C,color:#fff
    style D fill:#4EAA25,color:#fff
```

### 🔑 Sha-Bang (`#!`)

The **sha-bang** (shebang) tells the OS **which shell** to use when running the script.

```bash
#!/bin/bash    # Use Bash shell
#!/bin/sh      # Use POSIX sh shell
#!/usr/bin/env python3  # Use Python 3
```

> ⚠️ Writing sha-bang is **not mandatory** but **strongly recommended**.

---

## 💻 Commands & Examples

### Script 01 — Greet the User

```bash
#!/bin/bash

echo "Enter your name"
read NAME
echo "Good Evening, $NAME"
```

```bash
# Run the script
chmod +x script01.sh
sh script01.sh
```

---

### Script 02 — Full Name Input

```bash
#!/bin/bash

echo "Enter your first name"
read FNAME

echo "Enter your last name"
read LNAME

echo "Your Fullname : $FNAME $LNAME"
```

---

### Script 03 — Daily Routine Automation

```bash
#!/bin/bash
# Automates daily status checks

whoami
pwd
date
cal
ls -l
```

---

## 🌍 Real-World Use Cases

```mermaid
mindmap
  root((Shell Scripts in DevOps))
    Backups
      Database Backup
      File Backup
    Maintenance
      Delete Temp Files
      Log Rotation
    Monitoring
      System Health Checks
      Disk Usage Alerts
    CI/CD
      Build Triggers
      Deploy Automation
```

| Real-World Script | Purpose |
|---|---|
| `backup.sh` | Archive and backup directories |
| `log-analyzer.sh` | Parse and alert on error logs |
| `health-check.sh` | CPU, RAM, disk usage report |
| `cleanup.sh` | Remove temp/old files |
| `deploy.sh` | Pull code and restart services |

---

## 🔄 Script Execution Flow

```mermaid
sequenceDiagram
    participant User
    participant Shell
    participant Kernel
    participant Hardware

    User->>Shell: sh myscript.sh
    Shell->>Shell: Validate syntax
    Shell->>Kernel: Convert to kernel format
    Kernel->>Hardware: Execute instructions
    Hardware-->>Kernel: Result
    Kernel-->>Shell: Output
    Shell-->>User: Display result
```

---

## 📋 Summary

| Concept | Key Takeaway |
|---|---|
| **Shell Script** | A file with multiple commands executed together |
| **Sha-Bang** | Declares which shell interpreter to use |
| **`read`** | Accepts user input during script execution |
| **`echo`** | Prints output to the terminal |
| **`.sh` extension** | Standard extension for shell script files |

---

## ⏭️ What's Next?

> 🔜 **Day 03 — Variables in Shell Scripting**
> Learn Environment Variables, User-Defined Variables, `.bashrc`, and permanent variable setup!

---

## 👨‍💻 Author & Support

<div align="center">

Made with ❤️ as part of the **DevOps Zero to Hero** series

[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github)](https://github.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com)

⭐ **Star this repo** if it helped you!

</div>
