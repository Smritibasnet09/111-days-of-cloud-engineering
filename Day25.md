## **Day 25 of Learning AWS (Devops  Engineer)**

# AWS Concepts

## 1. Snapshots

### Simple Explanation
A Snapshot in AWS is a backup copy of a storage volume.  
It is mainly used to save data so it can be restored later if needed.

Snapshots are commonly used with Amazon EBS (Elastic Block Store).

### Key Points
- Used for backup and recovery
- Stored in Amazon S3 internally
- Helps recover lost or damaged data
- Can create new volumes from snapshots

### Example
A company stores important application data in an EC2 instance.  
They create daily EBS snapshots so the data can be restored if the server fails.

---

## 2. VPC (Virtual Private Cloud)

### Simple Explanation
A VPC is a private virtual network inside AWS.  
It allows users to securely launch AWS resources like EC2 instances.

It works similar to a private network in a real office.

### Key Points
- Provides network isolation
- Allows control over IP addresses
- Supports public and private subnets
- Improves security and networking control

### Example
A company creates:
- Public subnet for web servers
- Private subnet for databases

This keeps the database secure from direct internet access.

---

## 3. Elastic IP

### Simple Explanation
An Elastic IP is a fixed public IP address in AWS.  
It can be attached to an EC2 instance.

Unlike normal public IPs, it does not change after restarting the instance.

### Key Points
- Static public IP address
- Can be moved between EC2 instances
- Useful for production servers
- Helps maintain consistent connectivity

### Example
A website server uses an Elastic IP so users can always access the same IP address even if the server changes.

---

## 4. CORS (Cross-Origin Resource Sharing)

### Simple Explanation
CORS is a security feature used in web browsers.  
It controls whether a website can request resources from another domain.

### Key Points
- Prevents unauthorized cross-domain access
- Controlled using HTTP headers
- Commonly used in APIs
- Improves web security

### Example
Frontend:
```text
https://myapp.com