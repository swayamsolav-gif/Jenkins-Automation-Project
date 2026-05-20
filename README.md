# 🚀 CI/CD Jenkins Automation Project using Terraform & Ansible

This project demonstrates complete automation of Jenkins CI/CD setup on AWS using:

- ☁️ Terraform for Infrastructure Provisioning
- 🔧 Ansible Collections & Roles for Configuration Management
- ⚙️ Jenkins for CI/CD Automation

The project follows Infrastructure as Code (IaC) and Configuration Management best practices.

---

# 📌 Project Overview

This project automates the complete Jenkins server setup from scratch.

## Workflow

1. Terraform launches AWS EC2 instance
2. Ansible connects to the server
3. Ansible roles configure Jenkins environment
4. Required Jenkins dependencies are installed
5. Jenkins becomes ready for CI/CD pipelines

---

# 🏗️ Architecture Diagram

```text
                    ┌────────────────────┐
                    │     Terraform      │
                    │────────────────────│
                    │ Launch AWS EC2     │
                    └─────────┬──────────┘
                              │
                              ▼
                 ┌────────────────────────┐
                 │        Ansible         │
                 │────────────────────────│
                 │ Uses Collections       │
                 │ Uses Roles             │
                 │ Automates Setup        │
                 └─────────┬──────────────┘
                           │
        ┌──────────────────┼──────────────────┐
        ▼                  ▼                  ▼
┌──────────────┐  ┌────────────────┐  ┌────────────────┐
│ Install Java │  │ Configure SSH  │  │ Install Jenkins│
└──────┬───────┘  └────────┬───────┘  └────────┬───────┘
       │                   │                   │
       └───────────────────┼───────────────────┘
                           ▼
                 ┌────────────────────┐
                 │   Jenkins Server   │
                 │     Ready for      │
                 │    CI/CD Pipelines │
                 └────────────────────┘
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Terraform | Infrastructure Provisioning |
| AWS EC2 | Cloud Server |
| Ansible | Configuration Management |
| Ansible Roles | Modular Automation |
| Ansible Collections | Reusable Modules |
| Jenkins | CI/CD Automation |
| GitHub | Source Code Repository |

---

# 🚀 Terraform Commands

## Initialize Terraform

```bash
terraform init
```

## Apply Infrastructure

```bash
terraform apply --auto-approve
```

## View Outputs

```bash
terraform output
```

---

# 🌐 Jenkins Access

```text
http://<EC2-PUBLIC-IP>:8080
```

---

# 🔐 Jenkins Credentials

```text
Username: admin
Password: admin123
```

---
