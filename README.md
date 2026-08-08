# 💳 NimbusPay — Cloud Infrastructure & Security

NimbusPay is a fintech startup-style project focused on building a
secure and scalable cloud environment for a digital payment platform.

The goal of this project is to simulate the kind of cloud infrastructure
and security challenges a growing fintech startup would face as it
builds and scales its platform.

---

## 🎯 Project Goal

Build a secure AWS environment that can support a growing application
while keeping infrastructure, network access, and sensitive resources
properly protected.

The project focuses on:

- Secure cloud architecture
- Network segmentation
- Identity and access control
- Infrastructure security
- Monitoring and logging
- Scalability
- Troubleshooting and security improvements

---

## ☁️ Current AWS Architecture

The initial environment includes:

- **AWS VPC** — `10.0.0.0/16`
- **Public Subnet** — `10.0.1.0/24`
- **Private Subnet** — `10.0.2.0/24`
- Internet Gateway
- Route Tables
- EC2
- Security Groups
- Application Load Balancer

### Architecture

```text
                    Internet
                       │
                       ▼
              ┌─────────────────┐
              │ Application     │
              │ Load Balancer   │
              └────────┬────────┘
                       │
                Public Subnet
                 10.0.1.0/24
                       │
                       ▼
                    EC2
                       │
                 ──────┼──────
                       │
                Private Subnet
                 10.0.2.0/24
                       │
                       ▼
              Private Resources
