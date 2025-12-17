# AWS Cloud Practitioner Notes - Domain 4: Billing, Pricing, and Support

## Domain 4 Overview

### What Domain 4 Covers:
- How AWS billing and pricing plays out in real world
- Shift from on-premises to AWS cloud cost models

---

## Fundamental Cost Shift: On-Premises vs. AWS

### On-Premises Cost Model:

**Characteristics:**
- Fixed-cost model
- Purchase hardware upfront
- Pay down over time
- Operating expenses month to month
- Predictable
- Planned for

**Example:**
- On-premises database
- Generally means fixed costs

### AWS Cost Model:

**Characteristics:**
- Variable pricing model
- Costs can change from month to month
- Pay only for what you use
- Usage may change month to month depending on usage patterns

---

## Domain 4 Task Statements

### Three Task Statements:

**Task Statement 4.1:** Compare AWS pricing models

**Task Statement 4.2:** Understand resources for billing, budget, and cost management

**Task Statement 4.3:** Identify AWS technical resources and AWS support options

---

## What Each Task Statement Covers

### Task Statement 4.1: AWS Pricing Models

**Focus:**
- AWS pricing models
- As you probably know by now: In AWS, you only pay for what you use

### Variable Pricing Model Implications:

**Challenge:**
- May be more challenging to predict costs
- Until you get used to different pricing structures within AWS

**Power:**
- Have power to influence AWS bill month to month
- By changing:
  - Architectures
  - Usage patterns
  - Approaches to solving problems

---

### Task Statement 4.2: Billing, Budget, and Cost Management

**What You Need to Know:**
- Can estimate your AWS bill
- Can track your AWS bill
- Can break down your AWS bill
- Can influence your AWS bill

**Focus:**
- Understand resources for:
  - Billing
  - Budget
  - Cost management

---

### Task Statement 4.3: Billing Support and AWS Support Options

**What You Need to Know:**
- Identify resources available for billing support
- Identify AWS support options

---

## Course Structure for Domain 4

### Approach:
- Each task statement addressed individually
- Breaking down knowledge and skills expected for success

---

## Key Concepts to Understand

### Shift from Fixed to Variable Costs:

**On-Premises (Fixed):**
- Upfront hardware purchase
- Predictable monthly costs
- Long-term commitments
- Capital expenses (CapEx)

**AWS (Variable):**
- Pay for what you use
- Costs vary month to month
- Based on usage patterns
- Operational expenses (OpEx)

### Benefits of Variable Pricing:

**Flexibility:**
- Adjust spending based on needs
- No upfront hardware costs
- Scale up or down as needed

**Control:**
- Power to influence costs
- Through architectural decisions
- Through usage optimization
- Through different pricing models

### Challenges of Variable Pricing:

**Predictability:**
- May be harder to predict exact costs initially
- Requires understanding of pricing structures
- Need to monitor and track usage

**Learning Curve:**
- Getting used to different pricing structures
- Understanding what drives costs
- Learning optimization techniques

---

## Important Mindset for Domain 4

### What You Should Know:

**1. Cost is Controllable:**
- You have power to influence AWS bill
- Through design decisions
- Through usage patterns
- Through pricing model selection

**2. Tools Are Available:**
- AWS provides tools to:
  - Estimate costs
  - Track spending
  - Manage budgets
  - Optimize costs

**3. Support is Available:**
- Resources for billing support
- Different AWS support options
- Help with cost optimization

---

## Domain 4 Learning Objectives

### By End of Domain 4, You Should Be Able To:

**1. Pricing Models:**
- Compare different AWS pricing models
- Understand when to use each model
- Know how each model affects costs

**2. Cost Management:**
- Estimate AWS costs
- Track current spending
- Break down costs by service/resource
- Influence and optimize costs

**3. Support Resources:**
- Identify billing support resources
- Understand AWS support options
- Know when to use each support option

---

## Connection to Previous Domains

### Builds on Earlier Concepts:

**From Domain 1:**
- Cloud economics
- Total Cost of Ownership (TCO)
- CapEx vs. OpEx
- Economies of scale

**From Domain 2:**
- AWS Shared Responsibility Model
- (Affects what you're responsible for managing and paying for)

**From Domain 3:**
- Service knowledge
- (Understanding services helps understand their pricing)

---

## Key Themes for Domain 4

### Three Main Themes:

**1. Flexibility:**
- Variable pricing provides flexibility
- Pay only for what you use
- Scale as needed

**2. Control:**
- You control your costs
- Through architectural decisions
- Through service selection
- Through usage patterns

**3. Visibility:**
- Tools to see what you're spending
- Resources to understand costs
- Support to optimize spending

---

## Exam Preparation Focus

### What to Study:

**1. Pricing Models:**
- Different pricing options
- When to use each
- How they compare

**2. Cost Management Tools:**
- How to estimate costs
- How to track spending
- How to manage budgets
- How to optimize costs

**3. Support Options:**
- Different support plans
- What each includes
- When to use each
- Resources available

---

## Practical Application

### Real-World Skills:

**Cost Estimation:**
- Ability to estimate project costs
- Understanding pricing structures
- Planning budgets

**Cost Optimization:**
- Identifying cost-saving opportunities
- Implementing cost-effective architectures
- Monitoring and adjusting spending

**Support Utilization:**
- Knowing when to seek help
- Understanding available resources
- Using support effectively

---

## Notes for Success

**Remember:**
- AWS pricing is variable (not fixed like on-premises)
- You pay only for what you use
- You have power to influence costs
- Tools and support available to help
- Understanding pricing structures takes time but is achievable

**Key Mindset:**
- Cost management is ongoing
- Optimization is always possible
- Support and resources are available
- Understanding services helps understand costs

**For the Exam:**
- Know different pricing models
- Understand cost management tools
- Know support options
- Be able to select appropriate resources for scenarios


# AWS Cloud Practitioner Notes - Task Statement 4.1: Compare AWS Pricing Models

## Cost Optimization Pillar - AWS Well-Architected Framework

### What is Cost Optimization?

**Definition:**
- The ability to run systems that deliver business value at the lowest price point

---

## AWS Cost Optimization Resources

### Multiple Ways to Run Cost-Optimized Environment:

**AWS Services:**
- AWS Budgets
- AWS Cost and Usage Reports
- AWS Cost Explorer
- Reserved Instances
- Reserved Instance Reporting
- And more

**Cost-Effective Resources:**
- Spot Instances
- Reserved Instances
- Cost-effective storage:
  - Amazon S3
  - S3 Glacier
  - Glacier Deep Archive

**Match Supply with Demand:**
- AWS Lambda
- Amazon EC2 Auto Scaling
- AWS Auto Scaling

**Optimize Over Time:**
- AWS Trusted Advisor
- Cost and Usage Reports
- And more

---

## Cost Optimization Design Principles

### Fundamentals Matter:

**Key Point:**
- Cost optimization pillar has design principles and best practices
- Help with this domain
- Especially helpful in real world

---

## 1. Rightsizing Infrastructure

### What is Rightsizing?

**Definition:**
- Picking correct instances for current resources
- Also for resources you plan to use

**Example:**
- Using larger EC2 instance size
- When all you need is small instance size to cover demand

### Benefits:

**Cost Savings:**
- Choose correct instance type
- Choose cheapest instance type that meets performance requirements
- Can save money

---

## 2. Increasing Elasticity

### Pay-for-What-You-Use Model:

**Ensure:**
- Only using resources when resources are needed

**Cost Reduction Strategies:**

**Smaller vs. Larger Instances:**
- Using smaller instances versus fewer larger instances
- Can reduce costs for your workload

**Auto Scaling:**
- Scale up instances when demand scales
- Scale back down when demand lessens
- Reduces cost even further

---

## 3. Choosing Right Pricing Model

### Focus for This Task Statement:

**When to Consider:**
- Choosing right pricing model comes into play AFTER:
  - You have right-sized your instances
  - Set up auto scaling

---

## AWS Pricing Models

### Several Different Options:

**List of Pricing Models:**
1. Reserved Instances
2. On-Demand Instances
3. Spot Instances
4. Savings Plans
5. Dedicated Hosts
6. Dedicated Instances
7. Capacity Reservations

---

## On-Demand Instances

### Characteristics:

**Just as They Sound:**
- Can choose to use when needed

**Great For:**
- Flexible start and end time
- Applications with uncertain requirements
- Short-term workloads
- Applications that CANNOT tolerate disruption (key phrase for exam)

---

## Reserved Instances

### Commitment:

**Term:**
- Come with 1-year or 3-year commitment

**Benefit:**
- With commitment: Receive lower price

### Cost Savings:

**Discount:**
- Can save up to 72% on On-Demand price

**Term Comparison:**
- 3-year term more cost effective than 1-year

### Payment Options:

**Three Options:**
1. All upfront
2. No upfront
3. Partial upfront

**Important to Know:**
- You pay this reservation whether you have instances running or not

---

## Reserved Instance Types and Features

### Regional vs. Zonal:

**Regional Reserved Instances:**
- Apply discount to any Availability Zone in Region

**Capacity Reservations:**
- Can be used across Regions or across AZs

### Convertible Reserved Instances:

**Type of Reserved Instances:**
- Add additional flexibility

**Can Change:**
- Instance families
- Operating systems
- Tenancies
- Over Reserved Instance term

### Scheduled Reserved Instances:

**How They Work:**
- Schedule your reservations
- Rate reduced during time window
- Pay for commitment within that schedule

**Use Case:**
- Match capacity reservation to predictable recurring schedule

---

## Reserved Instances - Exam Tips

### Most Significant Discount:

**Standard Reserved Instances:**
- Provide most significant discount compared to On-Demand Instances

### Consolidated Billing:

**AWS Organizations Feature:**
- Treats all accounts in organization as one

**Benefit:**
- All accounts in organization can receive hourly cost benefit
- Of Reserved Instances purchased by any other account

### Good For:

**Use Cases:**
- Applications with steady state usage
- Applications with long-term needs
- Much cheaper than On-Demand Instances

---

## Spot Instances

### Characteristics:

**Cheapest Pricing Model:**
- Up to 90% off On-Demand pricing

**How They Work:**
- AWS uses spare EC2 capacity
- Sells capacity as Spot Instances
- Price based on how much extra capacity there is
- Spot price changes as capacity changes

### Great For:

**Use Cases:**
- Flexible applications
- Applications that can withstand disruption
- Applications that can tolerate failure
- Applications that need really low price

**Important:**
- Cheapest pricing model
- But applications have to be flexible with interruptions

---

## Using Multiple Pricing Models Together

### Optimization Strategy:

**Can Use All Pricing Models at Same Time:**

**Example Setup:**
- Reserved Instances: Cover production environment
- Spot Instances: Use when you have increase in demand
- On-Demand Instances: Use as needed

**Benefit:**
- Great way to optimize environment
- By knowing and understanding pricing models
- Choosing right pricing model for environment

---

## Other Pricing Models

### Dedicated Hosts

**Characteristics:**
- More of technical difference than pricing model
- Reserved for you alone
- Pay for Dedicated Host to be dedicated to you
- NOT shared with other AWS customers
- Pay for host (not individual instances running on host)

### Dedicated Instances

**Characteristics:**
- Instances you pay per hour
- For instance running on single tenant

### Scheduled Instances

**Use Case:**
- Great for applications that need to be available on regular schedule

### Savings Plans

**Use Cases:**
- Great for compute usage
- Can use for:
  - Lambda
  - Amazon EC2

---

## Cost Optimization Tools

### AWS Trusted Advisor

**What It Does:**
- Monitors your infrastructure
- Can make recommendations on how to make infrastructure more optimized

### AWS Cost Explorer

**What It Does:**
- Monitor your cost

---

## 4. Match Storage to Usage

### Storage Optimization:

**Key Principle:**
- Reducing storage can save money
- Match storage usage to particular storage class

**Multiple Storage Classes Available:**
- Amazon S3
- Amazon EBS
- AWS Storage Gateway
- Amazon EFS
- CloudFront
- Multiple data transfer options

**Ensure:**
- Pick correct storage class

---

## 5. Calculate Data Transfer Costs

### Data Transfer Pricing:

**AWS Offers:**
- Tiered pricing for data transfer from AWS to internet
- Helps reduce data transfer costs

**Data Transfer Out:**
- Data traffic destined to on-premises data center
- Considered data transfer out
- Results in charge to monthly bill

### Architecture Optimization:

**Can Use AWS Services:**
- CloudFront
- Direct Connect

**Example - Direct Connect:**
- Eliminate data transfer out charges
- Cost associated with data traffic through private connection included in service

**Example - CloudFront:**
- If using Amazon S3 for content delivery
- Using CloudFront reduces latency between end users and S3 bucket

### Key Point:

**Continuous Assessment:**
- Continuously assess AWS architecture
- Understand where data transfer costs incurred
- Can adapt deployment to:
  - Reduce overall running costs
  - Improve end user experience

---

## 6. Measure and Monitor Infrastructure

### Why Important:

**Infrastructure Changes:**
- Most likely will be changing
- Need measures in place to monitor and measure:
  - Usage
  - Costs

### What to Monitor:

**Utilization:**
- CPU
- RAM
- Storage
- And more

**Purpose:**
- Identify instances that could be downsized
- Identify instances that may need to be increased

---

## Monitoring Tools

### AWS CloudWatch

**Use For:**
- Track metrics
- Set alarms to immediately take actions

### AWS Trusted Advisor

**Use For:**
- Infrastructure recommendations

### AWS Well-Architected Framework Tool

**Use For:**
- Architecture assessment

### AWS Cost Explorer

**Use For:**
- Cost tracking and analysis

---

## Critical Monitoring Practices

### Essential Steps:

**1. Define Metrics:**
- Know what to measure

**2. Set Target Goals:**
- Have specific objectives

**3. Define and Enforce Tagging Strategy:**
- Use cost allocation tags
- Track costs by resource/project/team

**4. Make Sure Cost Allocation Tags Are Used:**
- Essential for cost tracking

**5. Review Regularly:**
- For any infrastructure changes

---

## Cost Optimization Best Practices

### 1. Define and Enforce Cost Allocation Tagging

**Throughout Whole Environment:**
- Can see what resources are costing more

### 2. Use Effective Account Structure

**Means:**
- Know what your end goals are
- Design to meet those goals
- Define and use metrics to track progress of meeting goals

### 3. Enable Teams to Design Based on Cost

**Give Teams:**
- Knowledge of what cost is
- Access so they can see what they're building
- Access to see costs associated with that build

**Result:**
- Once you give team or person ownership of cost
- Most are much more cost conscious

### 4. Create Cloud Center of Excellence (CCOE)

**What It Is:**
- Team who stays up to date on:
  - AWS best practices
  - New releases
  - And more

**Purpose:**
- Ensure using AWS in most efficient and cost-effective ways

---

## Opening Up Expenditure

### Benefits:

**When You Open Up Expenditure:**
- Make teams more accountable
- Make teams more aware

**Results:**
- Choose more cost-effective resources
- That still match supply to demand
- Optimize AWS account and infrastructure over time

---

## Exam Preparation Summary

### Pricing Models to Know:

**On-Demand:**
- Flexible, no commitment
- Applications that cannot tolerate disruption
- Uncertain requirements, short-term workloads

**Reserved Instances:**
- 1-year or 3-year commitment
- Up to 72% savings
- Pay all upfront, partial upfront, or no upfront
- Pay whether running or not
- Regional or zonal
- Convertible (can change instance type)
- Scheduled (specific time windows)
- Standard RI = most significant discount
- Good for steady state, long-term needs

**Spot Instances:**
- Cheapest (up to 90% off)
- Uses spare capacity
- Price changes with capacity
- Applications must tolerate interruptions
- Good for flexible, fault-tolerant applications

**Savings Plans:**
- For compute usage (Lambda, EC2)

**Dedicated Hosts:**
- Pay for entire host
- Not shared with others

**Dedicated Instances:**
- Pay per hour per instance
- Single tenant

**Scheduled Instances:**
- Regular schedule needs

### Cost Optimization Principles:

**Six Key Areas:**
1. Rightsizing infrastructure
2. Increasing elasticity
3. Choosing right pricing model
4. Matching storage to usage
5. Calculating data transfer costs
6. Measuring and monitoring

### Best Practices:

**Four Main Practices:**
1. Cost allocation tagging
2. Effective account structure
3. Enable teams to design based on cost
4. Create CCOE

### Tools:

**Cost Management Tools:**
- AWS Budgets
- Cost and Usage Reports
- Cost Explorer
- Reserved Instance Reporting
- Trusted Advisor
- CloudWatch
- Well-Architected Framework Tool

### Key Concepts:

**Cost Optimization:**
- Run systems at lowest price point
- Pay for what you use
- Match supply with demand
- Continuously optimize
- Use multiple pricing models together

**Critical for Exam:**
- Standard RI = most significant discount
- Consolidated billing shares RI benefits across accounts
- Applications that cannot tolerate disruption = On-Demand
- Cheapest = Spot (but must tolerate interruptions)
- Data transfer out = charged
- Direct Connect eliminates data transfer out charges
- CloudFront reduces latency and data transfer costs

---
# AWS Cloud Practitioner Notes - Task Statement 4.2: Understand Resources for Billing, Budget, and Cost Management

## Monitoring and Cost Management Foundation

### From Previous Lesson:

**Need to Implement:**
- Good monitoring solution
- Good cost management solution

**To Understand:**
- Resource needs
- How costs are allocated
- Measure and monitor architecture

**Architecture Reality:**
- Most likely will be changing
- Need measures in place to monitor and measure:
  - Usage
  - Cost

---

## Cost Management Tools

### AWS Cost Explorer and Cost and Usage Reports

**What You Can Monitor:**
- Utilization of:
  - CPU
  - RAM
  - Storage
  - And more

**Purpose:**
- Identify instances that could be downsized
- Identify instances that may need to be increased

### Amazon CloudWatch

**Already Mentioned Several Times:**
- Track metrics
- Set alarms to immediately take actions

---

## Critical Cost Management Practices

### Essential Steps:

**Five Key Actions:**
1. Define your metrics
2. Set target goals
3. Define and enforce tagging strategy
4. Use cost allocation tags
5. Regularly review for infrastructure changes

**Requires:**
- Good understanding of cost management tools

---

## Cost Allocation Tags

### How to Use:

**Example Use:**
- Use tags to filter views in Cost Explorer
- Helps analyze costs

**Practical Application:**
- Tag resources by:
  - Project
  - Department
  - Environment (prod, dev, test)
  - Owner
  - Application

---

## AWS Cost Explorer vs. Cost and Usage Reports

### Question: High-Level Interactive Financial Reports

**AWS Cost Explorer:**
- High-level view
- Can drill down into more specifics
- Interactive
- Visual

**AWS Cost and Usage Reports:**
- Breakdown costs by:
  - Hour
  - Day
  - Month
  - Product
  - Resource tags
  - And more
- Provides most granular data about AWS cost and usage
- Can send data to:
  - Amazon Athena
  - Amazon Redshift
  - AWS QuickSight
  - Other tools
- Perform quick queries and more

---

## AWS Budgets

### What You Can Create:

**Alarm Types:**
- Billing alarms
- Free tier alarms
- Alarms with AWS Budgets

### Automated Actions:

**Know:**
- Different ways to trigger automated actions
- Based on defined budget thresholds

**Benefits:**
- Keep close eye on state of AWS bill
- Be alerted if exceeding any cost threshold set for account

---

## AWS Organizations and Control Tower

### What They Help With:

**Centrally Manage:**
- Billing
- Control access
- Compliance
- Security
- Share resources

### Consolidated Billing:

**Ensure You Know:**
- Benefits of consolidated billing

---

## Data Visualization - Amazon QuickSight

### What It Does:

**Use For:**
- Analyze AWS Cost and Usage Reports
- Create custom reports

**Know:**
- High-level functionality of Amazon QuickSight

---

## Auto Scaling for Cost Optimization

### AWS Auto Scaling and EC2 Auto Scaling

**Purpose:**
- Help minimize costs
- Ensure only appropriate number of instances
- To match customer demand

### Other Services That Auto Scale:

**Know:**
- AWS Lambda
- Amazon API Gateway
- Can automatically scale up and down

---

## AWS Trusted Advisor

### Recommendations:

**Example:**
- Gives recommendations when finds underutilized EBS volumes in account

### Rightsizing:

**Having Monitoring in Place:**
- Establish baseline of usage
- Big part of being able to rightsize volumes

**Continue to Track:**
- Correct metrics to determine if need to modify solution for cost optimization

---

## EBS Cost Optimization

### IOPS Optimization:

**Pay Attention To:**
- How many IOPS you're using
- Compare to how many IOPS you're paying for

**Optimization Opportunity:**
- If paying for most optimized, most performant volume type
- But not using that capacity
- May be able to change volume type
- Save money without taking performance hit

---

## Data Lifecycle Management

### Lifecycle Rules:

**Know How:**
- Use data lifecycle rules
- To automatically delete data no longer needed
- Reduces storage costs

**Be Prepared:**
- Choose most cost-effective storage when provided set of requirements

### Services to Check Out:

**Amazon Data Lifecycle Manager:**
- Solutions for automatically deleting old EBS snapshots

**AWS Backup:**
- Backups from other AWS services
- Could help reduce storage costs within AWS account

---

## Amazon S3 Cost Optimization

### Storage Classes:

**Optimize by:**
- Making use of different storage classes when appropriate

**Should Be Familiar With:**
- Different S3 storage classes
- How they impact both:
  - Cost
  - Retrieval times

### What You Need to Know:

**Don't Need:**
- Exact pricing for S3 storage tiers

**Do Need:**
- Trade-offs between storage costs and retrieval costs for each tier
- How that can impact AWS bill
- Given scenario for data storage and access patterns

---

## S3 Lifecycle Configuration vs. Intelligent Tiering

### Question 1: Automatic Transition After Period of Time

**Scenario:**
- S3 has wide variety of storage classes to minimize cost
- Which capability allows automatic transition of all objects in bucket after period of time?
- Options: S3 Lifecycle Configuration or Intelligent Tiering?

**Answer: S3 Lifecycle Configuration**
- Lifecycle policies can help with this

### Question 2: Move Individual Objects to Most Cost-Effective Tier

**Scenario:**
- Which S3 storage class automatically moves each individual object to most cost-effective access tier when access patterns change?

**Answer: Intelligent Tiering**
- Great storage class for this requirement

**Remember:**
- Can create lifecycle policies with other S3 storage classes too

### Study Recommendation:

**Dive Deeper into S3:**
- Most likely get few storage cost optimization questions
- Where S3 is answer or plausible distractor

---

## S3 Requester Pays

### Question:

**Scenario:**
- Is it possible to configure S3 bucket so requestor pays cost?
- Cost of request and data downloaded?
- Instead of S3 bucket owner?

**Answer: Yes**
- If you configure requester to pay for:
  - Storage transfers
  - Usage

---

## Data Migration Options for Hybrid Environments

### Need to Know:

**Different Options for Optimizing Data Migration:**
- AWS DataSync
- Snow Family
- AWS Transfer Family
- AWS Storage Gateway

---

## Data Migration Example Question

### Scenario:

**Organization Needs:**
- Move 250 terabytes of archive data
- From internal servers to S3
- What is fastest and most cost-effective way?

**Options:**
- AWS Snowmobile
- Establish Direct Connect connection to transfer data to S3
- Order multiple Snowball devices
- Upload directly using current 100 Mbps dedicated line

**Answer: Order Multiple Snowball Devices**

**Why Snowball:**
- Usually strong choice for data transfer
- Especially if need transfer to be:
  - More secure
  - Quick transfer of terabytes to petabytes of data to AWS

---

## Data Transfer Costs

### Architecting for Data Transfer:

**Purpose:**
- Ensure minimize data transfer costs

### Example Scenario: Data Lake with S3

**Question:**
- Building data lake using Amazon S3 as storage platform
- What data transfer would incur costs?

**Answer:**
- When transfer data from Amazon S3 to internet
- Charged for:
  - Storage size per month
  - Region that object will be transferred to

### Data Transfer Between Regions

**Question:**
- Will AWS charge for data transferred between two Regions?

**Answer: Yes**
- AWS charges for data transferred between two different Regions
- Similar to costs incurred from data transfer between:
  - AWS network
  - Public internet

---

## AWS Pricing Calculator

### What It Does:

**Estimate:**
- Costs to migrate and run workloads on AWS

**Provides:**
- Estimated monthly cost of AWS services
- For your use case
- Based on expected usage

---

## Consolidated Billing and Volume Discounts

### Question:

**Which service offers volume discounts when you enable consolidated billing?**

### How Consolidated Billing Works:

**Enables:**
- Share resources
- See combined view of AWS costs incurred by all accounts in department or company
- Obtain detailed cost report for each individual AWS account associated with paying account

**For Billing Purposes:**
- AWS treats all accounts in AWS Organization as if they were one account

### Volume Pricing Tiers:

**Some Services Have Volume Pricing:**
- Amazon EC2
- Amazon S3
- Have volume pricing tiers across certain usage dimensions
- Give lower prices the more you use service

**How It Works with Consolidated Billing:**
1. AWS combines usage from all accounts
2. Determines which volume pricing tier to apply
3. Gives lower overall price whenever possible
4. Allocates each linked account portion of overall volume discount
5. Based on account's usage

---

## AWS Billing Conductor

### What It Is:

**Custom Billing Service:**
- Supports showback and chargeback workflows
- For:
  - AWS Solution Providers
  - Enterprise customers

---

## Exam Preparation Summary

### Cost Management Tools:

**AWS Cost Explorer:**
- High-level view
- Interactive
- Drill down capability
- Visual reports

**AWS Cost and Usage Reports:**
- Most granular data
- Breakdown by hour/day/month/product/tags
- Send to Athena, Redshift, QuickSight
- For analysis

**AWS Budgets:**
- Create billing alarms
- Free tier alarms
- Trigger automated actions
- Based on thresholds

**Amazon CloudWatch:**
- Track metrics
- Set alarms
- Immediate actions

**AWS Trusted Advisor:**
- Recommendations for optimization
- Identify underutilized resources

**Amazon QuickSight:**
- Data visualization
- Custom reports
- Analyze Cost and Usage Reports

**AWS Pricing Calculator:**
- Estimate costs
- Based on expected usage

### Cost Allocation and Tagging:

**Best Practices:**
- Define metrics
- Set target goals
- Define and enforce tagging strategy
- Use cost allocation tags
- Regular reviews

**Cost Allocation Tags:**
- Filter views in Cost Explorer
- Analyze costs by tag
- Track by project/department/environment

### AWS Organizations:

**Consolidated Billing Benefits:**
- Centrally manage billing
- Share resources
- Combined view of costs
- Detailed reports per account
- Volume discounts across all accounts
- AWS treats all accounts as one for volume pricing

### Auto Scaling for Cost:

**Services:**
- AWS Auto Scaling
- Amazon EC2 Auto Scaling
- AWS Lambda (automatic)
- Amazon API Gateway (automatic)

**Purpose:**
- Match capacity to demand
- Only pay for what you need

### Storage Optimization:

**EBS:**
- Monitor IOPS usage vs. paid IOPS
- Rightsize volumes
- Use Trusted Advisor recommendations
- Data Lifecycle Manager for snapshot deletion
- AWS Backup for automated backups

**S3:**
- Multiple storage classes
- Lifecycle Configuration (automatic transitions after time)
- Intelligent Tiering (automatic based on access patterns)
- Understand trade-offs: storage cost vs. retrieval cost
- Requester Pays option available

### Data Transfer:

**Costs:**
- Data out to internet: Charged
- Data between Regions: Charged
- Similar to AWS network to public internet

**Migration Options:**
- DataSync
- Snow Family (Snowball for TB to PB)
- Transfer Family
- Storage Gateway

**Architecture Considerations:**
- Minimize data transfer costs
- Choose appropriate transfer method

### Critical Exam Concepts:

**When to Use What:**
- Cost Explorer: High-level, interactive, visual
- Cost and Usage Reports: Granular, detailed analysis
- Budgets: Alarms, automated actions
- Lifecycle Configuration: Automatic transitions after time period
- Intelligent Tiering: Automatic based on access patterns
- Snowball: TB to PB data transfer
- Consolidated Billing: Volume discounts

**Remember:**
- Tags enable cost tracking
- Auto scaling minimizes costs
- Regular monitoring essential
- Multiple tools work together
- Consolidated billing provides volume discounts
- Data transfer costs vary by destination

---
# AWS Cloud Practitioner Notes - Task Statement 4.3: Identify AWS Technical Resources and AWS Support Options

## Support Context and Reality

### Important Understanding:

**Reality:**
- Impossible for any one person to know absolutely everything
- About all services, features, and tools
- Even with Cloud Center of Excellence (CCOE)

**When You Need Support:**
- Run into things you can't figure out
- Can't solve for yourself
- Need something too difficult or time-consuming to build yourself

**Available:**
- AWS Managed Services
- Technology support options

---

## What Support Means

### Broader Than Just Fixing Problems:

**Support Doesn't Just Mean:**
- Something gone wrong
- Need help fixing it

**Often Involves:**
- Assisting as you design and build environments
- Get assistance and guidance you need
- Proactive help

---

## AWS Support Plans Overview

### Enterprise Support

**What It Provides:**
- Concierge service
- Main focus: Help you be successful in AWS

**Includes:**
- 24/7 technical support from engineers
- Tools and technology to automatically manage health of environment
- Designated Technical Account Manager (TAM)
  - Coordinates access to proactive and preventative programs
  - Access to AWS subject matter experts

### Business Support

**Infrastructure Event Management:**
- Can have access for additional fee

**Limitation:**
- Other proactive support programs exclusively available for Enterprise support:
  - Well-Architected reviews
  - Operations reviews

---

## Support Plan Comparison Questions

### Question 1: Support API Access

**Scenario:**
- Need most cost-effective AWS support plan
- With access to AWS support API for programmatic case management
- Options: Developer, Enterprise, Enterprise On-Ramp, Basic, or Business?

**Answer: Business Support Plan**

**Why:**
- More cost effective than Enterprise support
- Includes API access

---

## Basic Support Plan (Free)

### Automatically Available to All AWS Customers:

**Features:**
- Around-the-clock access to:
  - Customer Service
  - 1-on-1 responses to account and billing questions
  - Support forums
  - Service health checks
  - Documentation
  - Whitepapers
  - Best practice guides

---

## Business and Enterprise Support Features

### Additional Features (Beyond Basic):

**1. Use Case Guidance**
- What AWS products, features, and services to use
- To best support your specific needs

**2. AWS Trusted Advisor**
- Inspects customer environments
- Identifies opportunities to:
  - Save money
  - Close security gaps
  - Improve system reliability
  - Improve performance

**3. API for Support Center and Trusted Advisor**
- Allows for automated support case management
- Trusted Advisor operations

**4. Third-Party Software Support**
- Help with Amazon EC2 instance operating systems and configuration
- Help with performance of most popular third-party software components on AWS

---

## Question 2: Unlimited Technical Support Cases

**Scenario:**
- Which support plan allows unlimited number of technical support cases to be opened?
- Options: Basic, Business, or Developer?

**Answer: Developer Support Plan**

**Why:**
- Most cost-effective support plan
- Offers technical support with unlimited number of cases

### Developer Support Also Includes:

**Access to:**
- Seven core Trusted Advisor checks
- Personal Health Dashboard
  - Personalized view of health of AWS services
  - Alerts when your resources are impacted

---

## Other Support Resources

### Documentation and Community:

**Available Resources:**
- All AWS documentation
- AWS re:Post
- Whitepapers
- Blogs
- All other areas of AWS documentation

**Important:**
- Know where you can find answers you're looking for

---

## Real-World Tip: Search Skills

### Huge Real-World Tip (Best Advice from Mentor):

**Learn How To:**
- Google and search for answers or guidance you need
- "How is your Google kung fu?"
- Mine's pretty strong

---

## Where to Find Specific Information

### Question: Guided Instructions for First-Time Service Deployment

**First Choice: AWS Documentation**

### Question: AWS Best Practices

**First Choice:**
1. AWS Well-Architected Framework
2. Then AWS documentation for service you're interested in

### Question: Community Support for Specific Questions

**First Choice: AWS re:Post**

---

## AWS Training and Certification

### Utilize:

**AWS Training and Certification:**
- Help build knowledge and experience
- AWS Skill Builder
- Digital training
- Hands-on labs

---

## Finding Support - The Process

### Two-Step Approach:

**Step 1: Documented Answers**
- Understanding where to find documented answers
- First step in seeking support

**Step 2: Urgent Matters**
- Paths to find assistance with more urgent matters

---

## AWS Support Teams to Understand

### Evaluate How to Use:

**Various Teams Within AWS:**
1. AWS Abuse
2. Premium support
3. Billing or account support

### Additional Resources:

**Technical Account Managers (TAMs):**
- When can you utilize them?
- How can they help with your environment?

**AWS Partner Network:**
- What it is
- How you can use it

---

## Sources of Technical Assistance

### Important to Identify:

**Knowledge Sources:**
- Documented knowledge
- Community
- Professional services
- AWS Partner Network
- And more

**Purpose:**
- All there to help customers succeed

---

## Building Your Search Skills

### Practice Area:

**Where You'll Get Most Practice:**
- This area
- Your Google kung fu will grow
- As you perform searches

**Most Important Skill:**
- Knowing where to find supporting knowledge
- Probably one of most important things to learn
- As you prepare for exam
- Will greatly aid you as you use AWS

---

## Exam Preparation Summary

### Support Plans - Know the Differences:

**Basic (Free):**
- Customer service 24/7
- Account and billing questions
- Support forums
- Service health checks
- Documentation, whitepapers, best practices
- No technical support cases

**Developer:**
- Most cost-effective with technical support
- Unlimited technical support cases
- Seven core Trusted Advisor checks
- Personal Health Dashboard
- Business hours access
- General guidance

**Business:**
- All Developer features plus:
- Use case guidance
- Full Trusted Advisor
- API for Support Center and Trusted Advisor
- Third-party software support
- 24/7 technical support
- Infrastructure Event Management (additional fee)
- More cost-effective than Enterprise

**Enterprise:**
- All Business features plus:
- Concierge service
- Designated Technical Account Manager (TAM)
- Proactive programs (Well-Architected reviews, operations reviews)
- 24/7 technical support from senior engineers
- Most comprehensive support

**Enterprise On-Ramp:**
- Between Business and Enterprise
- Some proactive support
- Pool of TAMs

---

## Key Support Resources to Know:

### Documentation:
- AWS Documentation (first choice for how-to guides)
- AWS Well-Architected Framework (first choice for best practices)
- Whitepapers
- Best practice guides

### Community:
- AWS re:Post (first choice for specific questions)
- Support forums

### Training:
- AWS Training and Certification
- AWS Skill Builder
- Digital training
- Hands-on labs

### Professional:
- Technical Account Manager (TAM) - Enterprise/Enterprise On-Ramp
- Professional Services
- AWS Partner Network

### Tools:
- AWS Trusted Advisor (Business/Enterprise get full access)
- Personal Health Dashboard
- Support API (Business/Enterprise)
- Service Health Dashboard (all plans)

---

## Critical Exam Concepts:

### Support Plan Selection:
- **Need API access?** → Business or Enterprise
- **Most cost-effective with technical support?** → Developer
- **Unlimited cases?** → Developer (most cost-effective), Business, or Enterprise
- **TAM?** → Enterprise or Enterprise On-Ramp
- **Proactive programs?** → Enterprise
- **Third-party software support?** → Business or Enterprise

### Where to Find Help:
- **First-time deployment guide?** → AWS Documentation
- **Best practices?** → Well-Architected Framework, then service documentation
- **Specific community question?** → AWS re:Post
- **Build AWS knowledge?** → AWS Training and Certification, Skill Builder

### Support Teams:
- AWS Abuse
- Premium support
- Billing or account support
- Technical Account Managers (when available)
- AWS Partner Network

### Important Skills:
- Know where to find information
- Strong search skills (Google kung fu)
- Understand support resources available
- Know when to use each resource

---

## Domain 4 Complete - Summary

### Three Task Statements Covered:

**4.1: Compare AWS Pricing Models**
- On-Demand (flexible, no commitment, can't tolerate disruption)
- Reserved Instances (1-3 year, up to 72% savings, steady state)
- Spot (cheapest, up to 90% off, must tolerate interruptions)
- Savings Plans (compute usage)
- Dedicated Hosts/Instances
- Cost Optimization Pillar (rightsizing, elasticity, storage matching, data transfer, monitoring)

**4.2: Billing, Budget, and Cost Management**
- Cost Explorer (high-level, interactive, visual)
- Cost and Usage Reports (granular, detailed)
- AWS Budgets (alarms, automated actions)
- CloudWatch (metrics, alarms)
- Trusted Advisor (recommendations)
- QuickSight (visualization)
- Consolidated Billing (volume discounts)
- Cost allocation tags
- S3 storage classes and optimization
- Data transfer costs

**4.3: AWS Support Options**
- Four support plans (Basic, Developer, Business, Enterprise)
- Documentation resources
- Community resources (re:Post)
- Training (Skill Builder)
- Professional services
- AWS Partner Network
- Where to find help

---
## Final Notes for Success

**Key Themes:**
- Variable pricing (pay for what you use)
- Cost control through architecture
- Multiple tools for cost management
- Consolidated billing benefits
- Support scales with needs
- Documentation and community resources available

**For the Exam:**
- Know pricing model differences and when to use each
- Understand cost management tools and their purposes
- Know support plan features and differences
- Understand where to find different types of help
- Be able to select appropriate services for cost scenarios

**Real World:**
- Search skills are critical
- Know where to find information
- Use appropriate support resources
- Continuous cost optimization
- Monitor and adjust regularly
