# Module 5: Package Management

## Overview
This module introduces package management in Linux. Package managers help you install, update, and manage software easily. In bioinformatics and data science, tools like `conda` and `pip` are widely used.

---

## 0. Installing Conda (Miniconda)

### Description
Conda is not always pre-installed. You need to install **Miniconda** or **Anaconda** first.

---

### Step 1: Download Miniconda

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

---

### Step 2: Run Installer

```bash
bash Miniconda3-latest-Linux-x86_64.sh
```

👉 Press:
- Enter to continue  
- Type `yes` to accept license  
- Press Enter for default install location  

---

### Step 3: Activate Conda

```bash
source ~/.bashrc
```

---

### Step 4: Check Installation

```bash
conda --version
```

👉 Example output:
```
conda 23.x.x
```

---

## 1. conda — Package and Environment Manager

### Install a Package

```bash
conda install numpy
```

---

### Install from Bioinformatics Channel

```bash
conda install -c bioconda prokka
```

---

### Create Environment

```bash
conda create -n myenv python=3.8
```

---

### Activate Environment

```bash
conda activate myenv
```

---

### Deactivate Environment

```bash
conda deactivate
```

---

### List Environments

```bash
conda env list
```

---

## 2. pip — Python Package Manager

### Install a Package

```bash
pip install numpy
```

---

### Install Specific Version

```bash
pip install numpy==1.21
```

---

### Upgrade Package

```bash
pip install --upgrade numpy
```

---

### List Installed Packages

```bash
pip list
```

---

## ⚠️ Important Difference

| Feature | conda | pip |
|--------|------|-----|
| Environment support | Yes | Limited |
| Handles dependencies | Strong | Basic |
| Best for | Bioinformatics, ML | Python packages |

---

## Best Practice

- Use `conda` for environment management  
- Use `pip` inside a conda environment if needed  
- Avoid mixing randomly  

---

## Practice

```bash
conda create -n testenv python=3.8
conda activate testenv
conda install numpy
pip install pandas
conda deactivate
```

---

## Summary

| Command | Description |
|--------|------------|
| conda install | Install package |
| conda create | Create environment |
| conda activate | Activate environment |
| pip install | Install Python package |
| pip list | View installed packages |
