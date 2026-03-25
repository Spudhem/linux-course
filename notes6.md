# Module 6: Bioinformatics

## Overview
This module introduces basic bioinformatics operations using Linux. You will learn how to work with FASTA files, count sequences, and install common bioinformatics tools such as samtools and bwa.

---

## 1. Understanding FASTA Files

### Description
FASTA is a common file format used to store biological sequences.

### Example

```bash
cat genome.fasta
```

### Output Example
```
>seq1
ATGCGTACGTAG
>seq2
TTGACGTAGCTA
```

👉 Lines starting with `>` represent sequence headers.

---

## 2. Counting Sequences in FASTA

### Method 1: Using grep

```bash
grep ">" genome.fasta
```

👉 Shows all sequence headers.

---

### Count number of sequences

```bash
grep -c ">" genome.fasta
```

👉 Counts number of sequences in FASTA file.

---

## 3. Count Lines in File

```bash
wc -l genome.fasta
```

👉 Counts total number of lines in the file.

---

## 4. Installing Bioinformatics Tools

### Install samtools

```bash
conda install -c bioconda samtools
```

👉 Used for handling BAM/SAM files.

---

### Install bwa

```bash
conda install -c bioconda bwa
```

👉 Used for sequence alignment.

---

### Install prokka (annotation tool)

```bash
conda install -c bioconda prokka
```

👉 Used for genome annotation.

---

## 5. Check Installation

```bash
samtools --version
bwa
prokka --version
```

---

## Practice

```bash
grep -c ">" genome.fasta
wc -l genome.fasta
```

👉 Count number of sequences in FASTA file.

---

## Summary

| Command | Description |
|--------|------------|
| grep ">" | View sequence headers |
| grep -c ">" | Count sequences |
| wc -l | Count lines |
| samtools | Work with sequence alignments |
| bwa | Perform alignment |
| prokka | Genome annotation |
