*This activity has been created as part of the 42 curriculum by raaalali.*

# 🖥️ Born2beRoot — Complete Evaluation & System Administration Guide

---

## 📖 Description

**Born2beRoot** is a system administration project from the 42 curriculum designed to introduce
students to the fundamentals of Linux system management and security.

The goal of this project is to configure a **secure Debian virtual machine** from scratch while
understanding how operating systems, users, permissions, networking, storage, and automation work
together in a real-world server environment.

By completing this project, the student demonstrates the ability to:
- Install and configure a Linux system
- Apply security best practices
- Manage users, groups, and permissions
- Configure services such as SSH, UFW, sudo, cron, and monitoring tools
- Understand disk partitioning and LVM
- Explain technical choices clearly during evaluation

---

## ⚙️ Instructions

### 🔹 Virtual Machine Setup
- Create a virtual machine using **VirtualBox**
- Install **Debian (no graphical interface)**
- Use encrypted partitions with **LVM**
- Ensure the VM boots with password authentication

### 🔹 System Configuration
- Configure **UFW** and allow only required ports (notably SSH on port 4242)
- Configure **SSH**:
  - Custom port (4242)
  - Disable root login
- Set strong **password policies**
- Enable and configure **sudo** with logging and TTY enforcement
- Create and manage users and groups using:
  - `raaalali` (main user)
  - `raad` (group name)

### 🔹 Monitoring & Automation
- Implement a monitoring script displaying system metrics
- Schedule the script using **cron** to run automatically at fixed intervals
- Ensure the script stops running if the cron rule is removed

### 🔹 Verification
- Generate a VM signature file using:
```bash
sha1sum ~/VirtualBox\ VMs/Born2beRoot/Born2beRoot.vdi > signature.txt
```
- Verify system state during evaluation using the provided commands

---

## 📚 Resources

### 📘 Documentation & References
- Debian Documentation: https://www.debian.org/doc/
- Linux Manual Pages (`man`)
- UFW Documentation: https://help.ubuntu.com/community/UFW
- OpenSSH Manual: https://www.openssh.com/manual.html
- LVM HOWTO: https://tldp.org/HOWTO/LVM-HOWTO/
- Cron Documentation: https://man7.org/linux/man-pages/man8/cron.8.html

### 🤖 Use of AI

AI tools were used **as a learning assistant**, not as a replacement for understanding.

Specifically, AI was used to:
- Help **organize documentation** in a clear and structured manner
- Rephrase explanations for clarity and evaluation readiness
- Verify command correctness and consistency
- Ensure compliance with 42 README requirements

All system configuration, commands, and implementation decisions were:
- Understood
- Executed
- Verified manually by **raaalali**

No automated system configuration was generated or blindly applied.

---

## 🧩 Additional Notes

- All examples, commands, usernames, and paths strictly use:
  - `raaalali`
  - `raad`
- This README is written to be:
  - Peer-readable
  - Recruiter-friendly
  - Evaluation-proof

---

## ✅ Conclusion

This project demonstrates a solid understanding of Linux system administration fundamentals.
Every configuration choice was made deliberately, with security, stability, and clarity in mind.

Born2beRoot is not about memorization —  
it is about **understanding how a system really works**.
