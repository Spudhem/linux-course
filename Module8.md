# Module 7: SLURM

## Overview
SLURM (Simple Linux Utility for Resource Management) is a workload manager used on HPC (High Performance Computing) systems. It allows users to submit, monitor, and manage jobs on a cluster.

---

## 1. sbatch — Submit Job

### Description
The `sbatch` command is used to submit a job script to the cluster.

### Example

```bash
sbatch job.sh
```

👉 Submits the job script `job.sh` to the scheduler.

---

### Example Job Script

```bash
#!/bin/bash
#SBATCH --job-name=test_job
#SBATCH --output=output.txt
#SBATCH --time=00:10:00
#SBATCH --cpus-per-task=2

echo "Hello from SLURM"
```

👉 This script:
- Sets job name  
- Defines output file  
- Requests time and CPU resources  
- Runs a simple command  

---

## 2. squeue — Check Job Status

### Description
The `squeue` command shows all running and pending jobs.

### Example

```bash
squeue
```

### Output Example

```
JOBID   PARTITION   NAME       USER   ST   TIME
12345   short       test_job   user   R    00:02
```

👉 Status (ST):
- R = Running  
- PD = Pending  

---

## 3. scancel — Cancel Job

### Description
The `scancel` command is used to stop a running or pending job.

### Example

```bash
scancel 12345
```

👉 Cancels job with ID 12345.

---

## Practice

```bash
sbatch job.sh
squeue
```

👉 Submit a job and check its status.

---

## Summary

| Command | Description |
|--------|------------|
| sbatch | Submit job |
| squeue | View jobs |
| scancel | Cancel job |
