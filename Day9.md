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

### 1. Application Load Balancer (ALB)

- Works at **Layer 7 (Application Layer)**
- Supports **HTTP and HTTPS**
- Makes routing decisions based on:
  - URL path
  - Hostname
  - Headers

Ex: 
login → EC2 Instance 1
, cart → EC2 Instance 2



### Use case:
- Web applications  
- Microservices  

---

### 2. Network Load Balancer (NLB)

- Works at **Layer 4 (Transport Layer)**
- Supports:
  - TCP
  - TLS
  - UDP
- Provides **static IP address**
- High performance and low latency  

### Use case:
- Real-time systems  
- Gaming servers  
- Financial applications  

---

### 3. Gateway Load Balancer (GWLB)

- Used for **security purposes**
- Uses **GENEVE protocol**
- Integrates with:
  - Firewalls  
  - Intrusion Detection Systems  

### Use case:
- Traffic inspection  
- Security appliances  

---

## 🔹 Important Components

---

### 📌 1. DNS Name (Hostname)

Each load balancer has a DNS like: xxx.region.elb.amazonaws.com

