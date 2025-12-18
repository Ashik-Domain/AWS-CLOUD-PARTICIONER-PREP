# **📘 MODULE 4 — Going Global (FULL SUMMARY)**

### *(Regions • Edge Locations • Global Infra • CDN • Route 53 • Outposts • IaC • CloudFormation)*

---

# **1. Introduction — Going Global with AWS**

* Expanding applications globally requires:

  * Right Region selection
  * Using edge locations for performance
  * Standardized automation for consistency
* AWS Global Infrastructure helps achieve:

  * Low latency
  * High availability
  * Compliance with local laws
  * Scalable operations across the world

---

# **2. AWS Regions (Choosing the Right One)**

Choosing a Region is like selecting where to open a new international store—consider demand, regulations, and cost.

### **Factors to consider when choosing a Region:**

## **1. Compliance (MOST IMPORTANT)**

* Laws may dictate where data must reside.
* Examples:

  * Germany (Frankfurt Region) — strict financial laws
  * UK customers → London Region
  * China → AWS China Regions
  * GDPR requirements in EU

## **2. Proximity**

* Choose the Region nearest to customers to reduce latency.
* Example: Serving Singapore users from Singapore Region vs. Virginia.

## **3. Feature Availability**

* Not every AWS service exists in every Region.
* GovCloud includes special compliance features.

## **4. Pricing**

* Prices vary by Region due to taxes, energy, and operational costs.

---

### **Region Selection Summary Table**

| Factor               | Why It Matters                   | Example                    |
| -------------------- | -------------------------------- | -------------------------- |
| Compliance           | Legal/regulatory rules           | GDPR, Frankfurt data laws  |
| Proximity            | Lower latency                    | Asia customers → Singapore |
| Feature Availability | Service support varies by Region | GovCloud features          |
| Pricing              | Cost optimization                | Choose lower-cost Regions  |

---

# **3. AWS Global Infrastructure Concepts**

## **1. AWS Regions**

* Geographic areas containing **3+ Availability Zones**.
* Each Region is isolated for security and legal control.
* You choose Regions based on latency, compliance, and cost.

---

## **2. Availability Zones (AZs)**

* Separate data centers with:

  * Independent power
  * Independent networking
  * Independent cooling
* Designed as isolated failure zones.
* Multi-AZ deployment improves resilience and availability.

---

## **3. Edge Locations**

Analogy: Like “coffee carts” near customers for fast service.

* Cached content served locally for **low latency**.
* Used by services like:

  * **Amazon CloudFront (CDN)**
  * AWS Global Accelerator
  * Amazon Route 53
* Improves load times for images, videos, static content, APIs.

---

## **4. Multi-AZ vs Multi-Region Deployments**

### **Multi-AZ (Within Same Region)**

* Protects against AZ-level failures.
* Improves HA (high availability).

### **Multi-Region (Across Regions)**

* Protects against full Region outages.
* Ensures extreme fault tolerance.
* Used for mission-critical global apps.

**Best practice:** Combine Multi-AZ + Multi-Region.

---

# **4. CloudFront (AWS CDN)**

* Distributed network of edge locations delivering content close to users.
* Reduces latency by caching content.
* Speeds up:

  * Images
  * Videos
  * APIs
  * Web apps
  * Software downloads

---

# **5. Supporting Global Edge Services**

### **1. Amazon Route 53 (DNS)**

* Converts domain names → IP addresses.
* Routes users to the **nearest healthy endpoint**.
* Supports geo-routing for performance and compliance.

### **2. AWS Global Accelerator**

* Improves performance by routing traffic over AWS global network instead of the public internet.
* Enhances:

  * Availability
  * Throughput
  * Latency

---

# **6. AWS Outposts**

* AWS infrastructure installed **on-premises**.
* Extends AWS services to local data centers.
* Ideal for:

  * Low-latency requirements
  * Data residency compliance
  * Hybrid cloud workloads

Provides:

* Same AWS APIs
* Same tools
* Same services
  But running locally within your building.

---

# **7. Infrastructure and Automation**

## **1. Why Automation?**

Manual setup across many Regions is:

* Slow
* Error-prone
* Not scalable
* Not repeatable

Automation ensures:

* Consistency
* Repeatability
* Faster deployments
* Version control

---

## **2. Infrastructure as Code (IaC)**

* Write infrastructure definitions as **code**.
* Blueprint-style deployments.
* Automatically creates consistent resources.
* Enables multi-Region deployments with zero manual errors.

---

## **3. AWS CloudFormation**

* Main AWS IaC service.
* Uses templates to:

  * Create
  * Modify
  * Delete
    AWS resources automatically.

CloudFormation benefits:

* Repeatable infrastructure
* Fast deployments
* Reduced errors
* Version-controlled architecture
* Scalable for global operations

---

## **4. Ways to Interact with AWS APIs**

* **AWS Management Console** — GUI, beginner-friendly.
* **CLI** — Automation via scripts.
* **SDKs** — Add AWS control directly into applications.
* **CloudFormation (IaC)** — Large-scale, consistent automation.

---

# **8. Putting It All Together — Global Architecture Strategy**

* Choose **Region** based on compliance → proximity → features → cost.
* Use **Edge Locations & CloudFront** to place content close to users.
* Use **Multi-AZ + Multi-Region** for fault tolerance.
* Use **Route 53 / Global Accelerator** for optimized routing.
* Use **CloudFormation** to automate resource provisioning globally.

This combination gives:

* Global performance
* High availability
* Consistent deployments
* Cost optimization
* Compliance with laws

---

