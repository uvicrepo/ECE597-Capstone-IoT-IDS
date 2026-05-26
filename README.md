# ECE597 Capstone: Multi-Stage IoT Network Intrusion Detection

## Team Quick Start

[Git Workflow](docs/git_workflow.md) 
[Task Assignment](docs/task_assignment.md) 
[Progress Log](docs/progress_log.md) 

Please read these before starting development so that everyone follows the same workflow and avoids duplicated work.

## Project Overview

This repository contains our ECE597 capstone project for building a multi-stage IoT network intrusion detection system using the CIC IoT-DIAD 2024 dataset.

The project follows a two-stage IDS design:

1. **Packet-Level Unsupervised Anomaly Detection**  
   Detects suspicious packet-level traffic without using labels during training.

2. **Flow-Level Supervised False Positive Reduction**  
   Uses flow-level features to re-check suspicious alerts and reduce false positives.

The target attack categories are:

- DDoS-HTTP Flood
- DoS-HTTP Flood
- DNS Spoofing
- Cross-Site Scripting (XSS)
- Brute Force

---

## Repository Structure

```text
data/       Local dataset folders and dataset instructions
docs/       Project documentation, workflow, task assignment, and progress tracking
src/        Core source code for sampling, preprocessing, models, and evaluation
tests/      Unit tests for important modules
results/    Generated figures, tables, metrics, and selected logs
scripts/    Optional execution entry points for running project phases