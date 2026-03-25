# Module 4: Permissions

## Overview
This module explains file permissions in Linux and how to control access using commands like `chmod` and `ls -l`. Understanding permissions is essential for managing files securely and running scripts.

---

## 1. ls -l — View File Permissions

### Description
The `ls -l` command shows detailed information about files, including permissions.

### Example
```bash
ls -l
```

### Output
```bash
-rw-r--r-- 1 user user 1234 file.sh
```

### Explanation

| Part | Meaning |
|------|--------|
| `-` | File type (`-` = file, `d` = directory) |
| `rw-` | Owner permissions (read, write) |
| `r--` | Group permissions (read only) |
| `r--` | Others permissions (read only) |

---

## 2. chmod — Change Permissions

### Description
The `chmod` command is used to change file permissions.

---

### Example 1: Make file executable

```bash
chmod +x file.sh
```

👉 Adds execute permission so the script can run.

---

### Example 2: Numeric permissions

```bash
chmod 777 file.sh
```

👉 Gives full permissions to:
- Owner
- Group
- Others

---

## 🔢 Understanding Numeric Permissions

| Number | Permission |
|--------|-----------|
| 7 | Read (4) + Write (2) + Execute (1) |
| 6 | Read + Write |
| 5 | Read + Execute |
| 4 | Read only |

---

### Example Breakdown

```bash
chmod 755 file.sh
```

👉 Means:
- Owner → full access (7)
- Group → read + execute (5)
- Others → read + execute (5)

---

## ⚠️ Important Notes

- `chmod 777` gives full access to everyone (not secure)
- Use safer permissions like `755` or `644`
- Always check permissions using `ls -l`

---

## Practice

```bash
ls -l
chmod +x file.sh
chmod 777 file.sh
ls -l
```

---

## Summary

| Command | Description |
|--------|------------|
| ls -l | View file permissions |
| chmod +x | Make file executable |
| chmod 777 | Give full permissions |
| chmod 755 | Common safe permission |


