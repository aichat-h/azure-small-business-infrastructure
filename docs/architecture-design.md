# Architecture Design (Version 1)

## Design Approach
This architecture was designed by analyzing five key questions:
Who uses the system, what services are needed, how components connect, what must be secured, and how failures are handled.

---

## 1. Users
The system is used by internal employees and IT administrators.

Therefore, Microsoft Entra ID is used for identity and access management.

---

## 2. Core Services
- Internal application hosted on a Virtual Machine
- File storage using Azure Storage Account
- Identity managed by Microsoft Entra ID

---

## 3. Network Design
A Virtual Network is used to isolate resources and provide secure communication between components.

---

## 4. Security Considerations
- Access controlled using Entra ID
- Resources placed inside a private virtual network
- Security groups will be introduced in future versions

---

## 5. Monitoring and Backup
- Azure Monitor will track system performance
- Azure Backup will protect critical virtual machine data

---

## Architecture Diagram

Employees
   │
   ▼
Microsoft Entra ID (Authentication Layer)

        (Access granted to resources)

Virtual Network (Network Boundary)
   ├──────────────────────┐
   ▼                      ▼
Internal Application     Storage Account
(Virtual Machine)

   │                      │
   └──────────┬───────────┘
              ▼
       Azure Monitor (Observability Layer)

              ▼
        Azure Backup (Protection Layer)

