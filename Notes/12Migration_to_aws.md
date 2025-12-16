# AWS Cloud Practitioner – Module 12: Migration to AWS

**Complete Exam-Focused Summary**

---

## 1. Why Migrate to AWS

Organizations migrate to AWS to:

* Reduce infrastructure costs
* Improve scalability and agility
* Increase reliability and security
* Modernize legacy applications
* Enable innovation faster

AWS provides **frameworks, strategies, and tools** to support every stage of migration. 

---

## 2. AWS Migration Process – Three Key Phases (EXAM CORE)

### Phase 1: **Assess**

**Goal:** Understand current environment and build a migration business case.

* Evaluate on-prem or existing cloud workloads
* Estimate migration cost & savings
* Optimize licensing usage

**Key Tool:**

* **AWS Migration Evaluator**

---

### Phase 2: **Mobilize**

**Goal:** Prepare for migration by understanding dependencies and planning.

* Discover applications & servers
* Map dependencies
* Choose migration strategies

**Key Tools:**

* **AWS Application Discovery Service**
* **AWS Migration Hub**

---

### Phase 3: **Migrate & Modernize**

**Goal:** Move workloads and improve architecture.

* Execute migrations
* Transfer data
* Modernize where possible

**Key Tools:**

* **AWS Application Migration Service**
* **AWS Database Migration Service (DMS)**
* **AWS DataSync, Transfer Family, Snow Family**



---

## 3. AWS Cloud Adoption Framework (AWS CAF)

### Purpose

AWS CAF helps organizations **plan and manage change** during cloud adoption by aligning:

* People
* Processes
* Technology

### Six CAF Perspectives (MEMORIZE)

| Perspective | Focus                               |
| ----------- | ----------------------------------- |
| Business    | Align IT with business goals        |
| People      | Skills, training, change management |
| Governance  | Risk, compliance, policies          |
| Platform    | Cloud architecture & infrastructure |
| Security    | Security controls & visibility      |
| Operations  | Day-to-day cloud operations         |

CAF produces an **action plan** to guide migration success. 

---

## 4. Migration Strategies – The **Seven Rs** (VERY HIGH EXAM WEIGHT)

| Strategy       | Meaning                         |
| -------------- | ------------------------------- |
| **Relocate**   | Move VMs/containers as-is       |
| **Rehost**     | Lift-and-shift (no code change) |
| **Replatform** | Minor optimizations             |
| **Refactor**   | Re-architect for cloud          |
| **Repurchase** | Replace with SaaS               |
| **Retain**     | Keep as-is                      |
| **Retire**     | Decommission                    |

📌 **Exam tip:** Most organizations use a **mix** of strategies. 

---

## 5. Core AWS Migration Services

### AWS Migration Evaluator

* Migration readiness assessment
* Cost estimation
* Licensing optimization

### AWS Application Discovery Service

* Discovers servers & dependencies
* Generates inventory reports

### AWS Migration Hub

* Central dashboard for tracking migrations
* Free service
* Integrates with discovery & migration tools

### AWS Application Migration Service

* Automates **lift-and-shift**
* Continuous replication
* Minimal downtime



---

## 6. Migrating Databases to AWS

### AWS Database Migration Service (DMS)

* Migrates databases with **minimal downtime**
* Supports:

  * Homogeneous migrations
  * Heterogeneous migrations
* Keeps source DB running during migration

### AWS Schema Conversion Tool (SCT)

* Converts:

  * Database schema
  * Stored procedures
  * Views & functions
* Used for **heterogeneous migrations**

📌 **Exam rule:**

* **DMS moves data**
* **SCT converts schema/code** 

---

## 7. Migrating Data to AWS – Online Transfer

### AWS DataSync

* Automated large-scale data transfer
* Secure & encrypted
* On-prem ↔ AWS

### AWS Transfer Family

* Managed file transfer
* Supports:

  * FTP
  * FTPS
  * SFTP

### AWS Direct Connect

* Dedicated private network
* High bandwidth, low latency
* Used for hybrid or large migrations



---

## 8. Migrating Data to AWS – Offline Transfer

### AWS Snow Family

* Physical devices for large-scale migration
* Used when:

  * Internet is slow
  * Data is in petabytes

### Snowball Edge

* Storage-optimized device
* Secure, rugged
* Can perform edge computing

📌 **Exam rule:**
Huge data + poor internet → **Snowball** 

---

## 9. Migration Tools – Quick Mapping Table

| Use Case             | AWS Tool                      |
| -------------------- | ----------------------------- |
| Cost assessment      | Migration Evaluator           |
| App discovery        | Application Discovery Service |
| Migration tracking   | Migration Hub                 |
| Lift-and-shift       | Application Migration Service |
| DB migration         | DMS + SCT                     |
| Online data transfer | DataSync / Transfer Family    |
| Offline transfer     | Snow Family                   |

---

## 10. Final Exam Takeaways (MUST MEMORIZE)

* Migration has **3 phases**: Assess → Mobilize → Migrate
* AWS CAF = people + process + technology
* Seven Rs define migration approach
* Migration Hub = tracking
* Application Migration Service = lift-and-shift
* DMS + SCT for database migration
* Snowball for petabyte-scale offline migration

---
