# AWS Cloud Practitioner – Module 5: Networking
**Exam-Focused Professional Summary**
---

## 1. Purpose of Networking in AWS

* AWS networking defines **how resources communicate** with each other and with the outside world.
* Core objective:

  * **Expose only what must be public**
  * **Protect internal resources**
* Public components interact with customers.
* Private components remain isolated for security and stability.
* This separation is **fundamental to AWS security and architecture design**. 

---

## 2. Amazon Virtual Private Cloud (Amazon VPC)

* **Amazon VPC** is a **logically isolated virtual network** inside AWS.
* You fully control:

  * IP address ranges (CIDR blocks)
  * Subnets
  * Routing
  * Security rules
* AWS resources like **EC2, Load Balancers, RDS** are launched inside a VPC.
* Benefits:

  * High security and isolation
  * Full control over network design
  * Easier than managing traditional on-prem networks 

---

## 3. Public vs Private Resources in a VPC

### Public Resources

* Have **direct internet access**
* Use cases:

  * Web servers
  * Load balancers
  * Public APIs

### Private Resources

* **No direct internet access**
* Use cases:

  * Databases
  * Internal services
  * Backend applications

✅ This separation:

* Reduces attack surface
* Improves security
* Is a **common exam concept** 

---

## 4. Subnets

* A **subnet** is a logical subdivision of a VPC.
* Each subnet exists in **one Availability Zone (AZ)**.
* Types:

  * **Public Subnet** → has route to Internet Gateway
  * **Private Subnet** → no direct internet route
* Purpose:

  * Organize resources
  * Control routing and access
* Public and private subnets **can communicate internally** if allowed 

---

## 5. Internet Connectivity Options

### A. Internet Gateway (IGW)

* Enables **internet access** for public subnets.
* Required for inbound & outbound internet traffic.
* Used by:

  * Public websites
  * Public APIs

### B. Virtual Private Gateway (VGW)

* AWS endpoint for **VPN connections**.
* Used with **Site-to-Site VPN**.
* Creates encrypted tunnel over the internet.
* Secure but performance depends on internet quality.

### C. AWS Direct Connect

* Dedicated **private physical connection** to AWS.
* Bypasses public internet.
* Benefits:

  * Low latency
  * High bandwidth
  * Consistent performance
* Used for:

  * Compliance workloads
  * Large data transfers 

---

## 6. AWS Hybrid Connectivity Services

### AWS Client VPN

* Managed VPN for **remote users**.
* Scales automatically.
* No hardware needed.
* Used for remote workforce access.

### Site-to-Site VPN

* Encrypted tunnel between on-premises network and AWS VPC.
* Uses public internet.
* Quick and cost-effective.

### AWS PrivateLink

* Private access to:

  * AWS services
  * Other VPCs
  * Partner services
* No need for:

  * IGW
  * NAT
  * VPN
* Traffic stays inside AWS network.

### AWS Direct Connect

* Best for:

  * High-bandwidth
  * Low-latency
  * Compliance workloads 

---

## 7. Additional Networking Components

### NAT Gateway

* Allows **private subnet instances** to access the internet **outbound only**.
* Prevents inbound internet access.

### AWS Transit Gateway

* Central hub to connect:

  * Multiple VPCs
  * On-prem networks
  * Multiple Regions
* Used in large enterprise architectures.

### Amazon API Gateway

* Create and manage APIs.
* Supports:

  * Authentication
  * Throttling
  * Monitoring 

---

## 8. Network Security Inside a VPC

### Network ACLs (NACLs)

* Operate at **subnet level**.
* **Stateless**:

  * Inbound & outbound rules required.
* Supports:

  * Allow
  * Deny
* Default NACL:

  * Allows all traffic.
* Custom NACL:

  * Denies all until rules added.

### Security Groups

* Operate at **instance level**.
* **Stateful**:

  * Return traffic automatically allowed.
* Supports:

  * Allow rules only
* Default:

  * Inbound denied
  * Outbound allowed 

---

## 9. Security Groups vs Network ACLs (EXAM FAVORITE)

| Feature        | Security Groups | Network ACLs     |
| -------------- | --------------- | ---------------- |
| Scope          | Instance        | Subnet           |
| State          | Stateful        | Stateless        |
| Rules          | Allow only      | Allow + Deny     |
| Return Traffic | Automatic       | Must be explicit |
| Use Case       | Fine-grained    | Broad control    |

---

## 10. AWS Global Networking Services

### Amazon Route 53

* DNS service.
* Converts domain names → IP addresses.
* Routing policies:

  * Latency-based
  * Geolocation
  * Geoproximity
  * Weighted routing

### Amazon CloudFront

* Content Delivery Network (CDN).
* Caches content at **edge locations**.
* Reduces latency and origin load.

### AWS Global Accelerator

* Routes traffic over AWS global private network.
* Improves:

  * Performance
  * Availability
  * Failover speed 

---

## 11. Global Architecture Patterns

* Single VPC → Multi-VPC → Multi-Region → Hybrid Cloud
* VPN:

  * Flexible
  * Internet-based
* Direct Connect:

  * Dedicated
  * High performance
* VPN + Direct Connect:

  * VPN used as failover
* Route 53 + CloudFront:

  * Low latency
  * Global availability
  * Multi-AZ reliability 

---

## 12. Final Exam Takeaways

* VPC = isolated virtual network.
* Public vs Private subnets = security foundation.
* Security Groups = stateful, instance-level.
* NACLs = stateless, subnet-level.
* IGW vs NAT vs VPN vs Direct Connect = **very common exam traps**.
* Route 53 + CloudFront = global performance.
* Direct Connect = **private, consistent, compliant networking**.

---
