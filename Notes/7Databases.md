# AWS Cloud Practitioner – Module 7: Databases

**Complete Exam-Focused Summary**

---

## 1. Why Databases Matter

* Databases store and manage **critical business data**:

  * Customers
  * Orders
  * Payments
  * Loyalty programs
  * Analytics data
* Enable:

  * Data-driven decisions
  * Personalization
  * Reliable transactions
* AWS provides **purpose-built databases** so you don’t use one database for all workloads. 

---

## 2. AWS Shared Responsibility Model for Databases

AWS database services fall into **three responsibility levels**.

### 1️⃣ Fully Managed Databases

AWS handles:

* Provisioning
* Patching & upgrades
* Backups
* Scaling
* Monitoring
* High availability

You handle:

* Data models (tables, items)
* Access control

Examples:

* Amazon RDS
* Amazon Aurora
* Amazon DynamoDB
* Amazon DocumentDB

### 2️⃣ Managed Databases

AWS handles:

* Infrastructure
* Backups
* Patching

You handle:

* Database configuration
* Query optimization
* Performance tuning

### 3️⃣ Unmanaged Databases

You manage **everything**:

* Installation
* Patching
* Backups
* High availability
* Security

Example:

* Installing MySQL on EC2

✅ **Exam takeaway**: Most AWS databases are **fully managed** to reduce operational burden. 

---

## 3. Relational Databases (SQL)

### What Are Relational Databases?

* Data stored in **tables (rows & columns)**.
* Relationships enforced using **keys**.
* Use **SQL** for querying.
* Fixed (rigid) schema.

### Best For

* Transactional workloads
* Structured data
* Applications needing joins and relationships

Examples:

* Orders ↔ Customers
* Inventory systems
* Billing systems 

---

## 4. Amazon Relational Database Service (Amazon RDS)

### What is RDS?

* **Managed relational database service**.
* AWS handles:

  * Backups
  * Patching
  * Monitoring
  * Infrastructure

### Supported Engines

* MySQL
* PostgreSQL
* MariaDB
* Oracle
* Microsoft SQL Server
* Amazon Aurora

### Key Features

* Automated backups & snapshots
* Point-in-time recovery
* Multi-AZ deployments (automatic failover)
* Read replicas for scaling reads
* Encryption at rest & in transit
* VPC isolation

### Best For

* Web & enterprise applications
* Structured transactional data 

---

## 5. Amazon Aurora (Advanced RDS)

### What Makes Aurora Special?

* AWS-built, cloud-native relational database.
* Compatible with:

  * MySQL
  * PostgreSQL

### Key Benefits

* Up to **5× faster than MySQL**
* Storage auto-scales **10 GB → 128 TB**
* Data replicated:

  * 6 copies
  * Across 3 AZs
* 99.99% availability
* Up to 15 read replicas
* Continuous backup to S3 (up to 35 days PITR)

### Best For

* High-performance workloads
* Gaming
* Media platforms
* Real-time analytics 

---

## 6. RDS vs Aurora (VERY COMMON EXAM QUESTION)

| Feature         | Amazon RDS       | Amazon Aurora             |
| --------------- | ---------------- | ------------------------- |
| Engine          | Multiple engines | MySQL/Postgres compatible |
| Performance     | High             | Very high                 |
| Storage Scaling | Manual resize    | Automatic                 |
| Replication     | Limited          | Up to 15 replicas         |
| Availability    | Multi-AZ         | Multi-AZ (99.99%)         |

---

## 7. NoSQL Databases – Amazon DynamoDB

### What is DynamoDB?

* Fully managed, **serverless NoSQL** database.
* Key-value and document data model.
* **No fixed schema**.
* Single-digit millisecond latency at any scale.

### Key Features

* Automatic scaling
* 99.999% availability
* Data replicated across 3 facilities per Region
* Global tables (multi-Region replication)
* Encryption at rest & in transit
* Pay-per-use pricing

### Best For

* High-traffic apps
* Mobile & web apps
* Gaming leaderboards
* Session storage
* Global applications 

---

## 8. DynamoDB vs RDS (EXAM FAVORITE)

| Feature     | DynamoDB             | RDS                   |
| ----------- | -------------------- | --------------------- |
| Type        | NoSQL                | Relational (SQL)      |
| Schema      | Flexible             | Rigid                 |
| Scaling     | Automatic            | Manual/instance-based |
| Performance | Millisecond at scale | Depends on config     |
| Joins       | ❌ Not supported      | ✅ Supported           |
| Maintenance | Fully serverless     | Managed               |

✅ **Rule of thumb**

* Structured + relationships → **RDS/Aurora**
* Massive scale + flexible schema → **DynamoDB**

---

## 9. In-Memory Databases – Amazon ElastiCache

### Why In-Memory Caching?

* Databases become slow under heavy read traffic.
* Cache frequently accessed data in **RAM**.

### Amazon ElastiCache

* Fully managed in-memory data store.
* Engines:

  * Redis
  * Memcached
* Microsecond-level latency.

### Benefits

* Reduces database load
* Improves application speed
* Automatic failover
* Multi-AZ replication
* Encryption at rest & in transit

### Use Cases

* Session storage
* Query caching
* Gaming leaderboards
* Real-time analytics 

---

## 10. Database Accelerators

### DynamoDB Accelerator (DAX)

* In-memory cache for DynamoDB.
* Dramatically reduces read latency.
* Transparent to applications.

---

## 11. Additional Purpose-Built Databases

| Service                   | Description                    | Use Case               |
| ------------------------- | ------------------------------ | ---------------------- |
| Amazon DocumentDB         | MongoDB-compatible document DB | JSON data, catalogs    |
| Amazon Neptune            | Graph database                 | Social networks, fraud |
| Amazon Managed Blockchain | Blockchain service             | Supply chains          |
| AWS Backup                | Centralized backup service     | Compliance & DR        |



---

## 12. Database Selection – Real-Life Mapping

* Orders & customers → **RDS / Aurora**
* Massive scale, flexible data → **DynamoDB**
* Repeated reads → **ElastiCache**
* Graph relationships → **Neptune**
* JSON documents → **DocumentDB**

---

## 13. Final Exam Takeaways (MEMORIZE)

* AWS databases are **purpose-built**.
* RDS = managed SQL databases.
* Aurora = high-performance RDS.
* DynamoDB = serverless NoSQL at scale.
* ElastiCache = in-memory speed booster.
* Flexible schema → NoSQL.
* Fixed schema + joins → SQL.

---

Just say **“Next module”** or upload **Module 8** 🚀
