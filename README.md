# 🖥️ Enterprise Active Directory Infrastructure Project (MCSA Lab)

## 📌 Overview
This project is a complete enterprise Windows Server infrastructure designed to simulate a real corporate IT environment.  
It implements Active Directory Domain Services (AD DS), DHCP, Group Policy Objects (GPO), VPN (RRAS), and file server management.

The goal of this project is to demonstrate advanced system administration skills, including user management, network configuration, security policies, and enterprise-level infrastructure design.

---

## 🏗️ Infrastructure Components
The environment consists of the following servers and services:

- Primary Domain Controller (PDC)
- Child Domain Controller (NEWGRC)
- DHCP Server
- File Server (E: Drive Storage)
- RRAS VPN Server
- Client Machines (Domain Joined)

**Domain Name:**
ITISYSADMIN.com

---

## 👨‍💼 Active Directory Structure

Three Organizational Units (OUs) were created:

### 📁 IT Department
- IT1, IT2, IT3, IT4, IT5 (IT5 = Manager)

### 📁 HR Department
- HR1, HR2, HR3, HR4, HR5 (HR5 = Manager)

### 📁 Sales Department
- Sales1, Sales2, Sales3, Sales4, Sales5 (Sales5 = Manager)

Each department is isolated in its own OU for better management and security control.

---

## 🔐 Active Directory Features

- User and Group Management
- OU-based delegation of control
- Department Manager permissions:
  - Reset user passwords
  - Create and manage users within department
- Logon restrictions per user and workstation

---

## 🌐 DHCP Configuration

- IP Scope: 10.0.0.0/24
- Excluded IP: 10.0.0.1
- MAC Address Filtering Enabled
- IP Reservation configured for specific devices
- DHCP configuration backup completed

---

## ⏰ Logon Security Policy

- Allowed Logon Hours:
  - Saturday → Thursday
  - 09:00 AM → 04:00 PM

- Users restricted to log in only from assigned computers

---

## 📁 File Server Configuration

A centralized shared folder was configured on the E: Drive with role-based access control:

- IT Department → Full Control
- Sales Department → Modify Access
- HR Department → Read Only Access

---

## 📊 Storage Management

Implemented advanced disk configurations:

- Spanned Volume for storage expansion
- Striped Volume for high-performance write operations
- Fault-tolerant volume for data redundancy and reliability

---

## 🛡️ Group Policy Objects (GPO)

The following policies were applied:

- Block access to local drives (This PC restriction)
- Custom desktop wallpaper applied to all users
- Startup script to launch Calculator for all users
- GPO backup for disaster recovery

---

## 🌍 Network Services

- RRAS (Routing and Remote Access Service) configured
- VPN access enabled for secure remote connectivity
- Remote client testing completed successfully

---

## 🌲 Child Domain Controller

A child domain controller was successfully configured:

NEWGRC.ITISYSADMIN.com

- Trust relationship established with parent domain
- Replication between domains enabled and verified

---

## 🧪 Testing & Validation

All services were tested successfully on domain-joined client machines:

- User authentication verified
- Group policies applied successfully
- DHCP IP assignment working correctly
- File sharing permissions validated
- VPN connection tested successfully
- Domain replication confirmed

---

## 🧠 Skills Demonstrated

- Windows Server Administration
- Active Directory Design & Management
- DHCP Configuration & Security
- Group Policy Management (GPO)
- File Server Administration
- RRAS VPN Setup
- Enterprise Network Architecture
- System Security & Access Control
- Multi-domain Infrastructure Management

---

## 🚀 Business Value
This project simulates a real enterprise IT environment and demonstrates the ability to:

- Design and manage secure corporate infrastructures
- Centralize user and resource management
- Enforce security policies across departments
- Implement scalable enterprise network architecture
- Provide secure remote access solutions

---

## 👨‍💻 Author
Mohamed Gamal Nasser
