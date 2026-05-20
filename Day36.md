# Amazon EC2 (Elastic Compute Cloud)

## Introduction
Amazon EC2 is a web service provided by Amazon Web Services (AWS) that allows users to launch virtual servers in the cloud. These virtual servers are called **instances**. EC2 helps businesses run applications without buying physical hardware.

It provides scalable computing capacity, meaning users can increase or decrease resources based on demand.

---

# Key Features of EC2

## 1. Virtual Servers (Instances)
EC2 allows users to create different types of virtual machines depending on workload requirements such as:
- General purpose
- Compute optimized
- Memory optimized
- Storage optimized

### Example
- A small website may use a `t2.micro` instance.
- A machine learning project may use a GPU-based instance.

---

## 2. Scalability
EC2 can automatically scale resources using **Auto Scaling Groups**.

### Benefits
- Handles traffic spikes automatically
- Reduces cost during low traffic
- Improves application availability

### Example
If a shopping website gets heavy traffic during a sale, EC2 automatically launches additional instances.

---

## 3. Security
EC2 provides security using:
- Security Groups (virtual firewall)
- Network ACLs
- IAM Roles and Policies

### Example
A Security Group can allow only HTTP (port 80) and HTTPS (port 443) traffic.

---

## 4. Elastic IP Address
An Elastic IP is a static public IPv4 address designed for dynamic cloud computing.

### Benefits
- Fixed public IP
- Useful for hosting websites or servers

---

## 5. Storage Integration
EC2 integrates with:
- Amazon EBS (Elastic Block Store)
- Amazon S3
- Amazon EFS

### Example
A database server can use EBS volumes for persistent storage.

---

# Advantages of EC2
- Pay only for what you use
- Easy to scale
- Highly available
- Secure infrastructure
- Supports multiple operating systems

---

# Real-Life Use Cases

## Web Hosting
Companies host websites and applications on EC2 instances.

## Machine Learning
Developers use GPU instances for AI and deep learning models.

## Gaming Servers
Online multiplayer games use EC2 for scalable server infrastructure.

## Big Data Processing
Organizations process large datasets using EC2 clusters.

---

# Example Architecture

User → Load Balancer → EC2 Instances → Database

### Explanation
1. Users send requests.
2. Load Balancer distributes traffic.
3. EC2 instances process requests.
4. Database stores application data.

---

# Conclusion
Amazon EC2 is one of the most important services in AWS cloud computing. It provides flexible, scalable, and secure virtual servers for hosting applications, websites, machine learning systems, and enterprise workloads. Because of its scalability and pay-as-you-go pricing model, EC2 is widely used by startups, enterprises, and developers worldwide.