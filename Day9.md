# AWS Load Balancing & Auto Scaling 

---

# 1. Load Balancing

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

### 1. DNS Name (Hostname)

Each load balancer has a DNS like: xxx.region.elb.amazonaws.com

Users access the application through this.

---

### 2. Target Group

- A group of EC2 instances  
- Load balancer sends traffic to this group  

Ex: Target Group → [EC2-1, EC2-2, EC2-3]


---

### 3. Private Traffic Handling

- EC2 instances can be in a **private subnet**
- Load balancer receives public traffic and forwards it internally  

This improves security.

---

## Sticky Sessions 

- Keeps a user connected to the same EC2 instance  

### Disadvantages:
- Uneven load distribution  
- If instance fails → user session is lost  


---

## Cross-Zone Load Balancing

### 🔹 Enabled:
- Traffic is evenly distributed across all availability zones  

### 🔹 Disabled:
- Traffic stays within the same availability zone  


---

# 2. Auto Scaling Group (ASG)

---

## 🔹 What is Auto Scaling?

Auto Scaling automatically:
- Adds EC2 instances (**Scale Out**)  
- Removes EC2 instances (**Scale In**)  

---

## 🔹 Why Auto Scaling is Important?

- Handles traffic spikes automatically  
- Reduces manual effort  
- Saves cost  
- Maintains availability  

---

## 🔹 Desired Capacity

- The number of EC2 instances you want running  

Ex: Desired Capacity = 4



AWS always tries to maintain this number.

---

## 🔹 How AWS Decides to Scale?

Based on monitoring metrics such as:
- CPU utilization  
- Memory (RAM) usage  
- Network traffic  

Ex rule:

CPU > 70% → Add 2 instances

CPU < 30% → Remove 1 instance


---

## 🔹 Types of Scaling

---

### 1. Dynamic Scaling

- Based on real-time metrics  
Ex:
High CPU → Add instances
Low CPU → Remove instances


---

### 2. Scheduled Scaling

- Based on time  

Ex: Increase instances at 9 AM daily


---

### 3. Predictive Scaling

- Uses machine learning to predict future demand  

Ex:
- Automatically increases instances before expected traffic surge  

---

## 🔹 Scaling Actions

- **Scale Out** → Add instances  
- **Scale In** → Remove instances  

---

# 3. Load Balancer + Auto Scaling 

These services work together:

| Component      | Function                     |
|----------------|-----------------------------|
| Load Balancer  | Distributes traffic         |
| Auto Scaling   | Adjusts number of instances |

### Workflow:
1. User sends request  
2. Load balancer distributes traffic  
3. Auto scaling adjusts instances based on load  

Result in:
- High performance  
- High availability  
- Cost efficiency  

---

# 4. Templates

The statement:
> "By using templates, we can navigate from one box to another box during loading"

### ✔ Meaning:

This refers to tools like **AWS CloudFormation**.

- Load balancer  
- EC2 instances  
- Auto scaling group  

AWS automatically:
- Creates resources  
- Connects everything  

---

# Summary of today's class

- ALB → HTTP/HTTPS (Layer 7)  
- NLB → TCP/UDP (Layer 4, static IP)  
- GWLB → Security (GENEVE protocol)  
- Target Group → EC2 instances  
- Sticky sessions → Not recommended  
- Cross-zone → Better when enabled  

---

- Auto Scaling → Automatic EC2 scaling  
- Desired capacity → Target instance count  
- CPU > 70% → Scale out  
- CPU < 30% → Scale in  
- Types → Dynamic, Scheduled, Predictive  

---
