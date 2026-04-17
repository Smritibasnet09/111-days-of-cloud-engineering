# Day 03 – AWS: Cross Account Access & S3

## Overview
This session focused on understanding how AWS enables secure resource sharing between accounts and how to store and manage data using Amazon S3.

---

## Topics Covered
- Cross Account Access using IAM Roles  
- Amazon S3 fundamentals  

---

## Key Concepts

### Cross Account Access
Cross Account Access allows one AWS account to access resources in another account securely.

It is implemented using:
- IAM Roles  
- Trust Policies  

**Important Insight:**  
Access is granted temporarily through roles. No passwords or long-term credentials are shared.

---

### Amazon S3 (Simple Storage Service)
Amazon S3 is a scalable object storage service used to store and retrieve data from the cloud.

**Practical Work:**
- Created S3 buckets  
- Configured bucket permissions  
- Applied basic access control policies  

**Important Insight:**  
S3 provides reliable and secure storage with flexible access management.

---

## Concept Summary

| Concept              | Purpose           | Key Idea                     |
|---------------------|------------------|-----------------------------|
| Cross Account Access | Secure sharing    | Role-based access control   |
| S3 Bucket            | Data storage      | Cloud-based object storage  |

---

## Implementation Snapshots

## 🔐 Cross Account Access Setup

<p align="center">
  <img src="https://github.com/user-attachments/assets/d36d1d5e-9d1d-47a5-abfc-9d15681d4b17" width="260"/>
  <img src="https://github.com/user-attachments/assets/ddda72d8-b232-4ef3-85e0-5342c506f1f9" width="260"/>
</p>

<p align="center">
  <em>IAM Role creation and cross-account trust configuration</em>
</p>

---

## 🪣 S3 Bucket Configuration

<p align="center">
  <img src="https://github.com/user-attachments/assets/341ce89c-2053-43c1-bc21-d1021eadd1e9" width="260"/>
  <img src="https://github.com/user-attachments/assets/c6644cf3-3c1e-47ea-8abb-2db33e7003c5" width="260"/>
</p>

<p align="center">
  <em>Bucket creation and permission settings</em>
</p>

---

## Final Output 

<p align="center">
  <img src="https://github.com/user-attachments/assets/040c6201-cc0b-465b-8c2c-5c33b6cf0198" width="260"/>
</p>

<p align="center">
  <em>Successful configuration and access verification</em>
</p>
---

## Real-World Application
In production environments:
- One AWS account stores data (e.g., in S3)  
- Another account accesses that data through IAM Roles  
- Access is controlled, temporary, and auditable  

This approach improves both **security** and **scalability**.

---

## Progress

Day 1 – Completed  
Day 2 – Completed  
Day 3 – Completed  

Consistency matters more than perfection.
