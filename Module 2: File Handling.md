# Module 2: File Handling

## Overview
This module covers basic file handling commands in Linux. These commands help you copy, move, and delete files and directories.

---

## 1. cp — Copy Files

### Description
The `cp` command is used to copy files or directories.

### Example
```bash
cp file1.txt file2.txt
```

👉 This creates a copy of `file1.txt` named `file2.txt`.

---

## 2. mv — Move or Rename Files

### Description
The `mv` command is used to move files or rename them.

### Example (Move file)
```bash
mv file2.txt dir/
```

👉 Moves `file2.txt` into the folder `dir/`.

### Example (Rename file)
```bash
mv file1.txt newfile.txt
```

👉 Renames `file1.txt` to `newfile.txt`.

---

## 3. rm — Remove Files

### Description
The `rm` command deletes files or directories.

### Example (Delete file)
```bash
rm file1.txt
```

### Example (Delete directory)
```bash
rm -r dir/
```

⚠️ Warning: Deleted files cannot be recovered.

---

## Practice

```bash
cp file1.txt file2.txt
mv file2.txt dir/
rm file1.txt
```

---

## Summary

| Command | Description |
|--------|------------|
| cp | Copy files |
| mv | Move or rename files |
| rm | Delete files or directories |
