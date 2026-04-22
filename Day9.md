# AWS Load Balancing & Auto Scaling 

---

# 🌐 1. Load Balancing

## 🔹 What is Load Balancing?

Load Balancing is a technique used to **distribute incoming traffic across multiple servers (EC2 instances)** so that no single server becomes overloaded.

In simple terms: 
If many users access an application at the same time, instead of sending all requests to one server, AWS distributes them across multiple servers.

### Why we use Load Balancing:
- Improves performance  
- Ensures high availability  
- Prevents server overload  
- Provides fault tolerance  

---

## 🔹 Types of Load Balancers in AWS

---

### 🟢 1. Application Load Balancer (ALB)

- Works at **Layer 7 (Application Layer)**
- Supports **HTTP and HTTPS**
- Makes routing decisions based on:
  - URL path
  - Hostname
  - Headers

👉 Example: