# AWS Learning



## 1. Amazon Athena

### Key Concept:

Amazon Athena is a **serverless query service** that allows you to analyze data stored in Amazon S3 using SQL.

### Important Exam Points:

* No infrastructure to manage (serverless)
* Uses standard SQL queries
* Charges per query scanned (not per server)
* Works directly with S3 data

### Example:

A company stores logs in S3 and wants to analyze them using SQL without setting up a database.

**Exam Tip:**
If question says *"query data in S3 using SQL without managing servers"* → choose Athena.

---

## 2. Amazon CloudFront

### Key Concept:

Amazon CloudFront is a **Content Delivery Network (CDN)** that delivers content to users with low latency by caching it at edge locations.

### Important Exam Points:

* Uses global edge locations
* Improves website speed and performance
* Works with S3, EC2, and custom origins
* Reduces latency for global users

### Example:

A website hosted in the US wants fast loading speed for users in Asia. CloudFront caches content closer to users.

**Exam Tip:**
If question mentions *faster content delivery globally* → choose CloudFront.

---

## 3. Amazon Redshift

### Key Concept:

Amazon Redshift is a **fully managed data warehouse service** used for big data analytics.

### Important Exam Points:

* Designed for OLAP (analytics), not OLTP
* Column-based storage
* High performance for large datasets
* Integrates with S3 and BI tools

### Example:

A company analyzes 10 years of sales data to find trends and business insights.

**Exam Tip:**
If question says *data analytics / business intelligence / huge datasets* → choose Redshift.

---

## 4. Amazon ECS / EKS (Containers)

### Key Concept:

* **ECS** = AWS-managed container orchestration
* **EKS** = Managed Kubernetes service

### Important Exam Points:

* Used for running Docker containers
* ECS is simpler and AWS-native
* EKS is Kubernetes-based (more complex but flexible)
* Supports microservices architecture

### Example:

A company wants to deploy microservices using Docker containers that automatically scale.

**Exam Tip:**
If question mentions *containers / Docker / microservices* → choose ECS or EKS.

---

## 5. Amazon RDS Multi-AZ & Read Replica

### Key Concept:

Amazon RDS provides relational databases with high availability and scalability options.

### Important Exam Points:

* **Multi-AZ** → High availability (automatic failover)
* **Read Replica** → Improves read performance and scaling
* Supports MySQL, PostgreSQL, Oracle, SQL Server

### Example:

A banking application needs high availability and automatic failover if the primary database fails.

**Exam Tip:**

* If question says *disaster recovery / failover* → Multi-AZ
* If question says *read scaling* → Read Replica

---

## Summary Table

| Service      | Purpose         | Exam Keyword           |
| ------------ | --------------- | ---------------------- |
| Athena       | SQL on S3       | Serverless query       |
| CloudFront   | CDN             | Fast global delivery   |
| Redshift     | Data warehouse  | Analytics / BI         |
| ECS/EKS      | Containers      | Docker / microservices |
| RDS Multi-AZ | DB availability | Failover               |


