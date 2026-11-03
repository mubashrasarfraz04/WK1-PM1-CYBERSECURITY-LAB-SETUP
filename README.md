# 🛡️ Cybersecurity Lab Environment Setup

### 🚀 Building an isolated virtual lab for penetration testing and ethical hacking practice

![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white)
![Kali](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white)
![NAT](https://img.shields.io/badge/NAT_Network-10.0.0.0%2F24-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Week](https://img.shields.io/badge/Week-01-orange?style=for-the-badge)



### 🌟 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.

The main purpose of this lab is to create a controlled and isolated environment where cybersecurity tools, network scanning, vulnerability assessment, and other security testing activities can be performed safely and ethically.

This lab will serve as the foundation for all future projects. Additional vulnerable machines can be added later and used as targets for authorized security testing.

> Lab Goal: To build a safe and private lab for learning ethical hacking without harming any real network.

---

### 🎯 Objectives

The main objectives of this project are to:

- ✅ Install and configure VirtualBox as a Hypervisor.
- ✅ Import Kali Linux virtual machine.
- ✅ Create a private NAT Network for the cybersecurity lab.
- ✅ Configure network connectivity for Kali Linux.
- ✅ Assign a consistent static IP address to the Kali VM.
- ✅ Test network connectivity and DNS resolution.
- ✅ Create a clean VM snapshot for recovery.
- ✅ Document the complete setup process.
- ✅ Prepare the lab for future cybersecurity projects.


### 🔐 Purpose of the Lab
 The purpose of this lab is to provide an isolated and controlled environment for cybersecurity learning and ethical hacking practice. It will be used for security tool testing, vulnerability assessment, and penetration testing. This lab ensures all testing is performed safely without affecting any real network.


### ⚙️ Lab Configuration

| 🧩 Component | 📝 Details |
| :--- | :--- |
| Hypervisor | VirtualBox 7.x |
| Main VM | Kali Linux |
| NAT Network Name | NatNetwork |
| IPv4 Prefix| 10.0.0.0/24 |
| Gateway| 10.0.0.1 |
| DNS Server | 8.8.8.8 |
| DHCP | Enabled |
| IPv6| Disabled |

---

### 🔧 Lab Setup Procedure

#### Step 1: 📥 Install 7-Zip
7-Zip was installed to extract the Kali Linux virtual machine package, which is distributed as a .7z archive.

#### Step 2: 💿 Install VirtualBox**
VirtualBox was installed as the main Hypervisor to run virtual machines.

#### Step 3: 🌐 Create the NAT Network**
A dedicated NAT Network was created in VirtualBox.
**Configuration:** Network Name: NatNetwork, IPv4 Prefix: 10.0.0.0/24, DHCP: Enabled, IPv6: Disabled.

#### Step 4: 🐉 Import Kali VM & Connect**
Kali Linux VM was imported and its network adapter was attached to the newly created **NatNetwork**.

#### Step 5: 🔌 Assign Static IP & Test**
A consistent static IP `10.0.0.10` was assigned to Kali and connectivity was tested using `ping 8.8.8.8` and `ping google.com`.

#### Step 6: 📸 Create a Clean Snapshot**
A clean snapshot was created in VirtualBox for quick recovery to a working state if anything breaks in the future.

---

### 📸 Lab Screenshots

| File Name | Description |
| :--- | :--- |
| `nat-network.png` | NAT Network Configuration Proof |
| `kali-linux.png` | Kali Linux Running in Lab |
| `vm-image.png` | VM Import Settings |

---

### ⚠️ Problems Encountered & Solutions

Problem 1: VT-x Virtualization Error 😥
VirtualBox showed error "VT-x is disabled in BIOS".
Solution: Went into BIOS settings and Enabled Virtualization Technology (Intel VT-x / AMD-V).

Problem 2: Internet Not Working After Static IP 😥
After setting static IP, internet stopped working.
Solution: Correctly added Gateway `10.0.0.1` and DNS `8.8.8.8` in network configuration.

---

### 🛠️ Tools & Resources

*   🗜️ 7-Zip - https://www.7-zip.org/
*   📦 VirtualBox - https://www.virtualbox.org/wiki/Downloads
*   🐉 Kali Linux- https://www.kali.org/

### 👩‍💻 About Me

Mubashra Sarfraz
Cybersecurity Learner | Network Walks Intern

### 📚 Project Information

*   Program Name:Cybersecurity at Networkwalks
*   Week: 01
*   Project:Cybersecurity & Pentesting Lab Setup
*   Repository: GitHub - WK1-PM1-CYBERSECURITY-LAB-SETUP
*   LinkedIn:https://www.linkedin.com/in/mubashra-khan-981805430?utm_source=share_via&utm_content=profile&utm_medium=member_android
*   
