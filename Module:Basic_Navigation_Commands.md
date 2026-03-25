
# Module 1: Linux Basics — Commands

## Basic Navigation Commands

### 1. pwd — Print Working Directory
```bash
pwd
```
Shows the current directory you are working in.

---

### 2. ls — List Files and Directories
```bash
ls
```
Lists files and folders in the current directory.

#### Useful Options
```bash
ls -l
ls -a
```

---

### 3. cd — Change Directory

#### Go into a folder
```bash
cd folder_name
```

#### Go back one level
```bash
cd ..
```

#### Go to home directory
```bash
cd ~
```

#### Go to specific path
```bash
cd /path/to/directory
```

---

## File and Directory Commands

### 4. mkdir — Create Directory
```bash
mkdir folder_name
```

---

### 5. rmdir — Remove Empty Directory
```bash
rmdir folder_name
```

---

### 6. rm — Remove Files or Directories
```bash
rm file.txt
rm -r folder_name
```

---

### 7. touch — Create Empty File
```bash
touch file.txt
```

---

## File Viewing Commands

### 8. cat — View File Content
```bash
cat file.txt
```

---

### 9. less — View File Page by Page
```bash
less file.txt
```

---

### 10. head — Show First Lines
```bash
head file.txt
```

---

### 11. tail — Show Last Lines
```bash
tail file.txt
```

---

## Help Command

### 12. man — Manual Page
```bash
man ls
```

---

## Practice

```bash
pwd
ls
mkdir test
cd test
touch file.txt
ls
cat file.txt
cd ..
rm -r test
```

---

## Summary

| Command | Purpose |
|--------|--------|
| pwd | Show current directory |
| ls | List files |
| cd | Change directory |
| mkdir | Create directory |
| rm | Delete file/folder |
| touch | Create file |
| cat | View file |
| less | View large file |
| head | First lines |
| tail | Last lines |
| man | Help |
