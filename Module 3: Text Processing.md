# Module 3: Text Processing

## Overview
This module introduces basic text processing commands in Linux. These tools are very powerful for handling large data files, especially in bioinformatics.

---

## 1. grep — Search Text

### Description
The `grep` command is used to search for a specific pattern or text in a file.

### Example
```bash
grep "text" file.txt
```

👉 Displays all lines in `file.txt` that contain the word "text".

---

## 2. awk — Process and Extract Columns

### Description
The `awk` command is used for pattern scanning and processing, especially useful for extracting columns.

### Example
```bash
awk '{print $1}' file.txt
```

👉 Prints the first column of each line in `file.txt`.

---

## 3. sed — Stream Editor

### Description
The `sed` command is used to search, replace, and edit text in a file.

### Example
```bash
sed 's/a/b/g' file.txt
```

👉 Replaces all occurrences of "a" with "b" in `file.txt`.

---

## Practice

```bash
grep "gene" data.txt
```

---

## Summary

| Command | Description |
|--------|------------|
| grep | Search text in files |
| awk | Extract and process columns |
| sed | Edit and replace text |
