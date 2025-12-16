# AWS Cloud Practitioner – Module 9: Security

**Complete Exam-Focused Summary**

---

## 1. Security Is a Shared Responsibility

* Security in AWS is **everyone’s responsibility**.
* Two foundational concepts:

  * **Authentication** – Who are you?
  * **Authorization** – What are you allowed to do?

| Concept        | Meaning              | Example                            |
| -------------- | -------------------- | ---------------------------------- |
| Authentication | Verifying identity   | Login with username/password       |
| Authorization  | Granting permissions | Allow user to view only their data |

Authentication gives access.
Authorization controls actions. 

---

## 2. AWS Shared Responsibility Model (EXAM CORE)

### AWS – *Security **of** the Cloud*

* Physical data centers
* Hardware & networking
* Global infrastructure
* Virtualization layer

### Customer – *Security **in** the Cloud*

* Data protection
* Identity & access management
* OS, apps, and configurations
* Network controls

📌 **Exam rule**
AWS secures the infrastructure.
You secure everything you deploy on top of it. 

---

## 3. AWS Security Controls – Three Pillars

1. **Prevent**

   * IAM permissions
   * Least privilege
2. **Protect**

   * Network, application, data encryption
3. **Detect & Respond**

   * Monitoring, alerts, incident response

Defense-in-depth is a core AWS security principle. 

---

## 4. Identity and Access Management (IAM)

### Root User (CRITICAL EXAM POINT)

* Created by default
* Has **full, unrestricted access**
* Best practices:

  * Enable MFA
  * Strong password
  * **Do NOT use for daily tasks**

---

### Principle of Least Privilege

* Grant **only minimum required permissions**
* IAM users have **no permissions by default**

---

## 5. IAM Core Components (MEMORIZE)

| Component | Purpose                            |
| --------- | ---------------------------------- |
| User      | Represents a person/app            |
| Group     | Collection of users                |
| Role      | Temporary access, no credentials   |
| Policy    | JSON document defining permissions |

---

### IAM Users

* Permanent credentials
* Best for individual humans or apps

### IAM Groups

* Easier permission management
* Users inherit group permissions

### IAM Roles (EXAM FAVORITE)

* Temporary credentials
* No username/password
* Used for:

  * AWS services
  * Cross-account access
  * Federated users

### IAM Policies

* Define **Allow / Deny**
* Attached to users, groups, or roles
* Types:

  * AWS managed
  * Customer managed 

---

## 6. Additional Access & Identity Services

| Service             | Purpose                                  |
| ------------------- | ---------------------------------------- |
| IAM Identity Center | Single Sign-On (SSO), centralized access |
| AWS Secrets Manager | Secure storage & rotation of secrets     |
| AWS Systems Manager | Manage servers & nodes at scale          |

📌 Secrets ≠ IAM users
Secrets Manager stores **passwords, keys, tokens**. 

---

## 7. Network & Application Protection

### Understanding DDoS Attacks

* **DoS**: Single attacker floods a system
* **DDoS**: Many compromised systems flood the target

Goal: Make service unavailable to legitimate users.

---

## 8. AWS Built-in Network Protections

### Security Groups

* Instance-level firewall
* Allow rules only
* Control inbound/outbound traffic

### Elastic Load Balancing (ELB)

* Distributes traffic
* Absorbs traffic spikes
* Prevents backend overload

### AWS Global Infrastructure

* Massive scale
* Distributed Regions & AZs
* Hard for attackers to overwhelm 

---

## 9. AWS Managed DDoS & App Protection Services

### AWS Shield

* **Shield Standard (free)**:

  * Automatic DDoS protection
* **Shield Advanced (paid)**:

  * Advanced mitigation
  * DDoS response team access

### AWS WAF (Web Application Firewall)

* Application-layer protection
* Filters HTTP/HTTPS traffic
* Uses Web ACLs
* Blocks malicious requests

| Service         | Protection Layer |
| --------------- | ---------------- |
| Security Groups | Network          |
| ELB             | Network + App    |
| AWS Shield      | Network + App    |
| AWS WAF         | Application      |



---

## 10. Data Protection on AWS

### Why It Matters

* Protect sensitive data:

  * PII
  * Credit cards
  * Personal records
* Prevent breaches, fraud, legal issues

---

## 11. Encryption Fundamentals (EXAM FAVORITE)

| Type                  | Meaning     |
| --------------------- | ----------- |
| Encryption at Rest    | Data stored |
| Encryption in Transit | Data moving |

---

### AWS Built-in Encryption

* Amazon S3 → encrypted by default
* Amazon EBS → encrypted volumes & snapshots
* DynamoDB → encrypted at rest

---

## 12. Key Data Protection Services

### AWS Key Management Service (KMS)

* Create & manage encryption keys
* Keys never leave AWS
* Integrated with many services

### AWS Certificate Manager (ACM)

* Manages SSL/TLS certificates
* Used for HTTPS & encryption in transit

### Amazon Macie

* Uses ML to:

  * Discover sensitive data in S3
  * Identify PII
  * Support compliance



---

## 13. Detection & Incident Response

### Why Detection Matters

* Not all threats can be prevented
* Rapid detection minimizes damage

---

## 14. AWS Security Detection Services

| Service          | Purpose                   |
| ---------------- | ------------------------- |
| Amazon Inspector | Vulnerability scanning    |
| Amazon GuardDuty | Threat detection          |
| Amazon Detective | Root-cause analysis       |
| AWS Security Hub | Centralized security view |

### Typical Flow

1. Inspector finds vulnerability
2. GuardDuty detects threat
3. Detective investigates cause
4. Security Hub centralizes alerts



---

## 15. Final Exam Takeaways (MUST MEMORIZE)

* AWS uses **shared responsibility model**
* IAM = authentication + authorization
* Least privilege is mandatory
* Roles = temporary access
* Security Groups ≠ WAF
* Shield = DDoS protection
* Encryption at rest + in transit
* KMS manages keys
* Macie finds sensitive data
* GuardDuty detects threats

---
