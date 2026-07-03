# Azure Service Mapping

This document maps business requirements to Azure services.

---

## 1. Secure hosting of internal applications

### Requirement
Host internal business applications securely.

### Azure Service
- Azure Virtual Machines

### Why
Virtual Machines provide full control over the operating system and allow hosting of custom internal applications.

---

## 2. Storage for company files

### Requirement
Store and manage company documents securely.

### Azure Service
- Azure Storage Account (Blob Storage / File Storage)

### Why
Azure Storage provides scalable, durable, and secure cloud storage for unstructured data and files.

---

## 3. Secure remote access for employees

### Requirement
Allow employees to access cloud resources securely.

### Azure Service
- Virtual Network (VNet)
- (Future improvement: Azure Bastion / VPN Gateway)

### Why
A Virtual Network provides network isolation and secure communication between resources.

---

## 4. Identity and access management

### Requirement
Control who can access the system.

### Azure Service
- Microsoft Entra ID

### Why
Entra ID provides authentication, user management, and access control for cloud resources.

---

## 5. Monitoring

### Requirement
Monitor system performance and detect issues.

### Azure Service
- Azure Monitor

### Why
Azure Monitor collects logs, metrics, and diagnostics from Azure resources.

---

## 6. Backup and recovery

### Requirement
Protect data and enable recovery in case of failure.

### Azure Service
- Azure Backup

### Why
Azure Backup provides automated backups and recovery options for virtual machines and data.
