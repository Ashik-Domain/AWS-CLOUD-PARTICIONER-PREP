# AWS Cloud Practitioner – Module 10: Monitoring, Governance & Compliance

**Complete Exam-Focused Summary**

---

## 1. Why Monitoring Matters in AWS

Monitoring means **observing, measuring, and reacting** to what happens in your cloud environment.

It enables:

* Proactive issue detection
* Automated alerts & scaling
* Troubleshooting & root-cause analysis
* Performance & cost optimization

Cloud environments are **dynamic** → monitoring is essential. 

---

## 2. Secure → Monitor → Audit → Comply (EXAM FLOW)

AWS governance follows a **progressive lifecycle**:

1. **Secure** – Prevent issues
2. **Monitor** – Detect issues early
3. **Audit** – Review controls & actions
4. **Comply** – Meet regulations & standards

| Stage   | Goal              | Key Services                |
| ------- | ----------------- | --------------------------- |
| Secure  | Prevent incidents | IAM, KMS, Security Groups   |
| Monitor | Observe & alert   | CloudWatch, CloudTrail      |
| Audit   | Review & validate | CloudTrail, AWS Config      |
| Comply  | Meet regulations  | AWS Artifact, Audit Manager |



---

## 3. Introduction to Monitoring (Core Concepts)

Monitoring provides:

* Metrics (numbers over time)
* Logs (detailed records)
* Alerts (notifications & automation)
* Dashboards (visualization)

Used for:

* Performance
* Availability
* Security
* Auto scaling
* Business insights 

---

## 4. Amazon CloudWatch (VERY HIGH EXAM WEIGHT)

### What is CloudWatch?

* Centralized **monitoring service** for AWS & on-prem resources.
* Real-time visibility into **performance & health**.

### Core CloudWatch Features

| Feature    | Purpose                          |
| ---------- | -------------------------------- |
| Metrics    | Track resource/app performance   |
| Alarms     | Trigger actions or notifications |
| Logs       | Collect & analyze log data       |
| Dashboards | Visualize metrics & logs         |

### Automation

* CloudWatch Alarms + SNS → email/SMS alerts
* Alarms → Auto Scaling actions

### Key Exam Rule

👉 **CloudWatch = metrics, logs, alarms, dashboards** 

---

## 5. AWS CloudTrail (AUDITING & SECURITY)

### What is CloudTrail?

* Records **every AWS API call**.
* Answers:

  * Who did what?
  * When?
  * From where?
  * Using which service?

### CloudTrail Components

| Component     | Purpose                  |
| ------------- | ------------------------ |
| Event history | View last 90 days (free) |
| Logs          | Store events in S3       |
| Insights      | Detect unusual activity  |

### Key Points

* Tracks **management & data events**
* Immutable audit trail
* Essential for compliance & forensics

👉 **CloudTrail = API activity & auditing** 

---

## 6. CloudWatch vs CloudTrail (EXAM FAVORITE)

| Feature    | CloudWatch           | CloudTrail          |
| ---------- | -------------------- | ------------------- |
| Focus      | Performance & health | API actions         |
| Data Type  | Metrics & logs       | Audit logs          |
| Alerts     | Yes                  | Via integrations    |
| Compliance | Indirect             | Direct              |
| Use Case   | Monitoring & scaling | Auditing & security |

---

## 7. AWS Compliance – Core Ideas

### Why Compliance Matters

* Regulations: GDPR, HIPAA, PCI-DSS, etc.
* Requires:

  * Evidence
  * Reports
  * Audits

### Shared Responsibility

* AWS: Compliant infrastructure
* Customer: Compliant architecture & configs

You **inherit** AWS controls but must configure services correctly. 

---

## 8. AWS Artifact (EXAM KEY)

### What is AWS Artifact?

* Central **compliance documentation portal**.

| Component           | Purpose                      |
| ------------------- | ---------------------------- |
| Artifact Reports    | Download audit reports       |
| Artifact Agreements | Accept compliance agreements |

Used for:

* Audit evidence
* Regulatory reporting

👉 **Artifact = compliance documents** 

---

## 9. Auditing & Continuous Compliance

### AWS Config

* Tracks **resource configuration changes**
* Evaluates compliance rules
* Detects configuration drift
* Can auto-remediate

### AWS Audit Manager

* Automates evidence collection
* Maps resources to compliance standards
* Generates audit-ready reports

| Service       | Purpose               |
| ------------- | --------------------- |
| AWS Config    | Continuous compliance |
| Audit Manager | Audit reporting       |



---

## 10. AWS Organizations (GOVERNANCE CORE)

### What is AWS Organizations?

* Centralized management of **multiple AWS accounts**.

### Key Components

| Component          | Description           |
| ------------------ | --------------------- |
| Management Account | Controls org          |
| Member Accounts    | Child accounts        |
| OUs                | Logical groupings     |
| SCPs               | Permission boundaries |

### Benefits

* Centralized billing
* Security & compliance enforcement
* Account isolation

👉 **SCPs set maximum permissions** (not grants). 

---

## 11. Governance Services

### AWS Control Tower

* Automated multi-account setup
* Enforces guardrails
* Best practices by default

### AWS Service Catalog

* Pre-approved resources
* Standardized provisioning

### AWS License Manager

* Tracks & enforces software licenses



---

## 12. AWS Health Dashboard

### What it Does

* Shows **service health & account-specific events**.

### Features

* Planned maintenance alerts
* Outage notifications
* EventBridge & SNS integration

👉 **Health = AWS service issues affecting you** 

---

## 13. AWS Trusted Advisor

### What It Does

* Continuous **best-practice checks**.

### 5 Categories

1. Cost optimization
2. Performance
3. Security
4. Fault tolerance
5. Service limits

Provides:

* Red/Yellow/Green status
* Actionable recommendations



---

## 14. IAM Access Analyzer

### Purpose

* Analyzes IAM policies
* Identifies **over-permissive access**
* Ensures least privilege

👉 **Access Analyzer = IAM permission review** 

---

## 15. Final Exam Takeaways (MUST MEMORIZE)

* CloudWatch → metrics, logs, alarms
* CloudTrail → API audit trail
* AWS Config → config compliance
* AWS Artifact → compliance documents
* Organizations → multi-account governance
* SCPs → permission boundaries
* Trusted Advisor → best-practice checks
* AWS Health → service events
* IAM Access Analyzer → permission analysis

---
