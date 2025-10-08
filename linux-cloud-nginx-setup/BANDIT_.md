# 🧩 OverTheWire Bandit Notes

**Purpose:**  
This file documents my progress through the [OverTheWire Bandit](https://overthewire.org/wargames/bandit/) wargame.  
The goal is to build a strong foundation in Linux command-line operations, file systems, permissions, SSH, and automation — before continuing with the main DevOps project.

---

## 📘 Overview

- **Game:** OverTheWire Bandit  
- **Total Levels:** 34 (0 → 33)  
- **Focus Areas:**  
  - Linux navigation  
  - File permissions and ownership  
  - Redirection, piping, and filters  
  - Networking and SSH  
  - Archives and compression  
  - Scripting logic  
- **Goal:** Complete all levels and record commands, concepts, and reflections to strengthen Linux fundamentals.

---

## 🗂️ Progress Log

### **Level 0 → 1**
**Objective:** Log into the game via SSH and read the contents of a file.  
**Commands Used:**  
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
cat readme
```
Concepts Learned:

Basic SSH login structure

Reading file contents with cat

Reflection:
Learned to authenticate via SSH and locate files. This level introduced the pattern of using the password from one level to access the next.

