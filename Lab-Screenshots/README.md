# Lab 01 – Linux Setup & Orientation

## Objective
Prepare a Linux system for learning and practice by setting up a VM, user accounts, and essential tools.

---

## 1. Virtual Machine Setup
- OS: Rocky Linux 9
- Hypervisor: VirtualBox
- RAM: 4 GB
- CPU: 2 cores
- Disk: 40 GB

---

## 2. Snapshot
- Snapshot Name: Clean Install
- Purpose: Restore system if anything breaks

---

## 3. Create Non-Root User

```bash
useradd devuser
passwd devuser
usermod -aG wheel devuser

---

## 4. Verify sudo Access

sudo whoami

### Update system
```bash
sudo dnf update -y

### 5. Install Development Tools
```bash

sudo dnf groupinstall "Development Tools" -y

### 6. Install Utilities
```bash
sudo dnf install -y vim tmux git



