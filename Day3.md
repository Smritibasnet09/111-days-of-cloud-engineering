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

### Cross Account Access Setup
<p align="center">
  <img width="300" height="300" alt="WhatsApp Image 2026-04-16 at 10 50 56 PM" src="https://github.com/user-attachments/assets/d36d1d5e-9d1d-47a5-abfc-9d15681d4b17" />

  <img src="Day03/images/page2.jpeg" width="300">
</p>
<p align="center">
  <em>IAM Role and Trust Policy Configuration</em>
</p>

---

### S3 Bucket Configuration
<p align="center">
  <img src="Day03/images/page3.jpeg" width="300">
  <img src="Day03/images/page4.jpeg" width="300">
</p>
<p align="center">
  <em>Bucket creation and permission settings</em>
</p>

---

### Final Output Verification
<p align="center">
  <img src="Day03/images/page5.jpeg" width="300">
  <img src="Day03/images/page6.jpeg" width="300">
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
