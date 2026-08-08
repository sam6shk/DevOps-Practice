Here is your **corrected document with point numbers starting from 1 (properly renumbered and fixed)**:

---

# Web Application, IT Operations & DevOps – Complete Notes

## 1. What is a Data Center?

A **Data Center** is a physical facility where IT infrastructure is hosted.

A traditional data center may contain:

- Physical Servers
- Storage
- Network Switches
- Routers
- Firewalls
- Load Balancers
- Power systems
- Cooling systems
- Backup systems
- Monitoring systems

Simple representation:

```text
                 DATA CENTER
                      |
       +--------------+--------------+
       |              |              |
     Servers        Storage        Network
       |                             |
       +-------------+---------------+
                     |
                  Firewall
                     |
                  Internet
```

---

## 2. What is an On-Premises Data Center?

**On-Premises (On-Prem)** means the organization owns or manages the physical infrastructure.

For example, a company may have:

```text
Company
   |
   v
Own Data Center
   |
   +-- Physical Servers
   +-- Storage
   +-- Network
   +-- Firewall
   +-- Load Balancer
   +-- Backup
```

The company is responsible for:

- Hardware
- Power
- Cooling
- Networking
- Operating Systems
- Servers
- Security
- Maintenance
- Backup
- Disaster Recovery

---

## 3. What is a Cloud Provider?

A **Cloud Provider** provides IT infrastructure and services over the internet.

Major cloud providers include:

- Microsoft Azure
- Amazon Web Services (AWS)
- Google Cloud Platform (GCP)

Instead of purchasing physical servers, organizations can consume infrastructure from the cloud.

Example:

```text
Traditional On-Prem

Company
   |
   v
Own Data Center
   |
   v
Physical Server
```

Cloud:

```text
Company
   |
   | Internet
   v
Cloud Provider
   |
   v
Virtual Machine / Container / Managed Service
```

---

## 4. On-Prem vs Cloud

### On-Premises

```text
Company
   |
   v
Physical Data Center
   |
   +-- Servers
   +-- Storage
   +-- Network
   +-- Firewall
   +-- Applications
```

The company owns/manages the infrastructure.

### Cloud

```text
Company
   |
   v
Cloud Provider
   |
   +-- Virtual Machines
   +-- Kubernetes
   +-- Database
   +-- Storage
   +-- Load Balancer
   +-- Networking
```

The company consumes infrastructure and services provided by the cloud provider.

---

## 5. What is Development?

**Development** means designing, writing, testing and maintaining application software.

The people involved are generally called **Developers**.

A developer writes application code.

For example:

```text
Frontend Developer
       |
       v
React Application
```

```text
Backend Developer
       |
       v
Java / .NET / Python Application
```

Developers focus mainly on:

- Application functionality
- Business logic
- Code
- Features
- Bug fixes
- Unit testing
- Application performance

---

## 6. What is Operations?

**Operations** is responsible for running and maintaining IT systems.

Operations traditionally includes:

- Server Administration
- Network Administration
- Database Administration
- Infrastructure Management
- Security
- Monitoring
- Backup
- Incident Management

For example:

```text
Operations Team

   +-- Server Admin
   +-- Network Admin
   +-- DBA
   +-- Security Team
   +-- Infrastructure Team
```

Their main responsibility is:

> Keep the application and infrastructure available, secure and reliable.

---

## 7. Traditional IT Model

Historically, Development and Operations were separate teams.

```text
             DEVELOPMENT
                  |
                  |
             Writes Code
                  |
                  v
              Application
                  |
                  |
             Handover
                  |
                  v
             OPERATIONS
                  |
        +---------+---------+
        |         |         |
      Server     DBA     Network
      Admin              Admin
```

This created a gap:

Developer:

> "My application is working on my machine."

Operations:

> "But it is not working on the server."

---

## 8. What is DevOps?

**DevOps = Development + Operations**

DevOps is a combination of:

- Culture
- Practices
- Automation
- Collaboration
- Tools

Goal:

> Develop, test, deploy and operate applications faster and more reliably.

---

## 9. Who is a DevOps Engineer?

A **DevOps Engineer** builds and maintains automation, infrastructure, deployment and operational processes.

A DevOps Engineer acts as a bridge between:

```text
Developers
     |
     v
  DevOps
     |
     v
Operations / Infrastructure
```

DevOps Engineer does NOT replace other roles.

---

## 10. Different IT Roles

### A. Frontend Developer

- UI / Web pages / Browser logic

### B. Backend Developer

- APIs / Business logic / Server-side code

### C. Database Administrator (DBA)

- Database installation, backup, performance, security

### D. Server Administrator

- OS, servers, patching, troubleshooting

### E. Network Administrator

- Network, routers, switches, firewalls, DNS

### F. Security Engineer

- Security, compliance, identity, access control

---

## 11. Where Does the DevOps Engineer Fit?

```text
                     BUSINESS
                        |
                        v
                  Product Owner
                        |
                        v
                   Development
                   /          \
        Frontend Developer   Backend Developer
                  \            /
                   \          /
                    \        /
                     v      v
                    DEVOPS
                      |
          +-----------+-----------+
          |           |           |
       CI/CD       Cloud       IaC
          |           |           |
       Docker       Azure      Terraform
          |
       Kubernetes
          |
          v
       Operations
          |
    +-----+-----+------+
    |           |      |
 Server       DBA   Network
 Admin               Admin
```

---

## 12. How DevOps Engineer Manages Everything

DevOps Engineer creates automation pipelines:

```text
Developer
   |
   v
Git
   |
   v
CI/CD Pipeline
   |
   +--> Build
   +--> Test
   +--> Security Scan
   +--> Docker Build
   +--> Push Image
   |
   v
Deployment
   |
   v
Kubernetes / VM
   |
   v
Application
   |
   v
Database
```

---

## 13. DevOps Engineer and Developers

```text
Developer
    |
    v
GitHub
    |
    v
CI/CD Pipeline
    |
    +-- Build
    +-- Test
    +-- Security Scan
    +-- Docker Build
    |
    v
Deployment
```

---

## 14. DevOps Engineer and Server Admin

```text
Developer
    |
    v
Terraform
    |
    v
Infrastructure
    |
    v
VM / Network / Storage
```

---

## 15. DevOps Engineer and DBA

```text
Terraform
    |
    v
Database Infrastructure
    |
    v
Application
    |
    v
Database
```

---

## 16. DevOps Engineer and Network Team

```text
Internet
   |
Firewall
   |
Load Balancer
   |
Frontend
   |
Backend
   |
Database
```

---

## 17. DevOps Engineer and Security (DevSecOps)

```text
Git
 |
 v
CI Pipeline
 |
 +--> Code Scan
 +--> Secret Scan
 +--> Dependency Scan
 +--> IaC Scan
 |
 v
Deploy
```

---

## 18. On-Prem Architecture

```text
INTERNET
   |
FIREWALL
   |
LOAD BALANCER
   |
Web Servers
   |
Backend Servers
   |
DATABASE
```

---

## 19. Cloud Architecture

```text
INTERNET
   |
Cloud Load Balancer
   |
Frontend
   |
Backend
   |
Managed Database
```

---

## 20. DevOps Lifecycle

```text
PLAN → CODE → BUILD → TEST → SECURITY → PACKAGE → DEPLOY → RELEASE → MONITOR → OPERATE
```

---

## 21. DevOps Responsibilities

- Cloud infrastructure
- CI/CD pipelines
- Docker & Kubernetes
- Terraform (IaC)
- Monitoring
- Security automation
- Scripting

---

## 22. What DevOps Engineer Actually Manages

```text
Code → Git → CI/CD → Docker → Kubernetes → App → DB → Users
```

DevOps manages:

- Automation
- Infrastructure
- Deployment pipelines
- Monitoring systems

---

## 23. DevOps vs Other Roles

| Role              | Responsibility                      |
| ----------------- | ----------------------------------- |
| Frontend Dev      | UI                                  |
| Backend Dev       | APIs                                |
| DBA               | Database                            |
| Server Admin      | Servers                             |
| Network Engineer  | Network                             |
| Security Engineer | Security                            |
| Cloud Engineer    | Cloud                               |
| DevOps Engineer   | Automation + CI/CD + Infrastructure |
| SRE               | Reliability                         |

---

If you want, I can also convert this into:\
✅ PDF notes\
✅ Interview cheat sheet\
✅ One-page revision sheet\
✅ Diagram-only version for exams
