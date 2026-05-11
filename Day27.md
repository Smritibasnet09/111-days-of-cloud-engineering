# AWS Advanced Concepts Notes

# 1. AWS Route Tables and Routing

## What is Routing in AWS?
Routing controls how network traffic moves between:
- VPCs
- Subnets
- Internet
- VPNs
- Other AWS services

AWS uses Route Tables to decide where traffic should go.

---

## Route Table

A Route Table contains rules called routes.

Each route has:
- Destination
- Target

### Example

| Destination | Target |
|---|---|
| 0.0.0.0/0 | Internet Gateway |
| 10.0.1.0/24 | Local |

---

## Important Targets in Routing

### Internet Gateway (IGW)
Allows public internet access.

### NAT Gateway
Allows private subnet instances to access internet outbound only.

### Virtual Private Gateway
Used for VPN connections.

### Transit Gateway
Connects multiple VPCs centrally.

### VPC Peering
Direct connection between two VPCs.

---

## Public vs Private Routing

### Public Subnet
- Route to Internet Gateway
- Public IP possible

### Private Subnet
- No direct internet access
- Uses NAT Gateway for outbound traffic

---

## Key Concept
AWS routing works using:
- CIDR ranges
- Longest prefix match

More specific routes get priority.

---

# 2. AWS Elastic Beanstalk

## What is Elastic Beanstalk?
Elastic Beanstalk is a Platform as a Service (PaaS).

It helps developers deploy applications easily without managing infrastructure manually.

---

## Supported Languages
- Java
- Python
- Node.js
- PHP
- Go
- Docker
- .NET

---

## What Elastic Beanstalk Automatically Handles
- EC2 provisioning
- Load balancing
- Auto Scaling
- Monitoring
- Deployment
- Health checks

---

## Architecture Flow

User → Load Balancer → EC2 Instances → Application

---

## Deployment Process
1. Upload application code
2. Elastic Beanstalk creates infrastructure
3. Application becomes available automatically

---

## Deployment Policies

### All at Once
Deploys to all instances together.

Fast but risky.

### Rolling
Updates instances gradually.

### Rolling with Additional Batch
Creates extra temporary instances during deployment.

### Immutable Deployment
Creates completely new environment first.

Safest deployment method.

---

## Benefits
- Easy deployment
- Automatic scaling
- Reduced operational work
- Integrated monitoring

---

## Difference Between EC2 and Elastic Beanstalk

| EC2 | Elastic Beanstalk |
|---|---|
| Manual infrastructure setup | Automated infrastructure |
| Full control | Managed environment |
| More operational work | Easier deployment |

---

# 3. Amazon Neptune Streams

## What is Amazon Neptune?
Amazon Neptune is a graph database service.

It is designed for:
- Highly connected data
- Relationship-based applications

---

## Common Use Cases
- Social networks
- Fraud detection
- Recommendation engines
- Knowledge graphs

---

## What are Neptune Streams?
Neptune Streams capture changes made to graph data.

It records:
- Inserts
- Updates
- Deletes

---

## Why Important?
Applications can react to graph changes in real time.

---

## Stream Flow

Graph Change → Neptune Stream → Lambda/Event Processing

---

## Example Use Case

In a recommendation system:
- User likes a product
- Graph updates immediately
- Stream captures update
- Recommendation engine refreshes suggestions

---

## Benefits
- Real-time processing
- Event-driven graph applications
- Change tracking
- Better integration with analytics systems

---

# 4. AWS Direct Connect Routing

## What is AWS Direct Connect?
AWS Direct Connect creates a dedicated private connection between:
- On-premises network
- AWS cloud

---

## Why Use It?
- Lower latency
- Stable connection
- Higher bandwidth
- More secure than internet

---

## Routing in Direct Connect

Direct Connect uses:
- BGP (Border Gateway Protocol)

BGP dynamically exchanges routing information.

---

## Types of Virtual Interfaces

### Private VIF
Access private AWS resources.

### Public VIF
Access public AWS services.

### Transit VIF
Used with Transit Gateway.

---

## Important Concept
Direct Connect does not automatically encrypt traffic.

VPN can be added for encryption.

---

# 5. AWS Global Routing with Route 53

## What is Route 53?
Amazon Route 53 is AWS DNS service.

It routes users to applications.

---

## Routing Policies

### Simple Routing
Single resource routing.

### Weighted Routing
Distributes traffic based on percentage.

### Latency Routing
Sends users to lowest latency region.

### Failover Routing
Switches to backup resource if primary fails.

### Geolocation Routing
Routes based on user location.

### Multi-Value Routing
Returns multiple healthy IPs.

---

## Example

Users from:
- Asia → Singapore server
- Europe → Frankfurt server

---

# 6. AWS App Mesh

## What is App Mesh?
AWS App Mesh manages communication between microservices.

---

## Main Features
- Traffic control
- Service discovery
- Monitoring
- Secure communication

---

## Why Important?
In microservices architecture:
- Many services communicate together
- Monitoring becomes difficult

App Mesh helps manage this communication.

---

## Commonly Used With
- ECS
- EKS
- Kubernetes

---

# 7. AWS Gateway Load Balancer

## What is it?
Gateway Load Balancer combines:
- Load balancing
- Network security appliance deployment

---

## Main Purpose
Helps deploy:
- Firewalls
- Intrusion detection systems
- Packet inspection tools

---

## Benefits
- Scalable security
- Centralized inspection
- Transparent traffic routing

---

# 8. AWS Cloud WAN

## What is AWS Cloud WAN?
Cloud WAN helps build and manage global wide area networks.

---

## Why Important?
Large organizations have:
- Multiple branches
- Multiple regions
- Hybrid networks

Cloud WAN centralizes management.

---

## Features
- Centralized networking
- Automated connectivity
- Global network management

---

# 9. AWS Network Firewall

## What is it?
AWS Network Firewall protects VPC networks.

---

## Features
- Stateful inspection
- Stateless filtering
- Domain filtering
- Intrusion prevention

---

## Main Benefit
Improves VPC-level network security.

---

# 10. AWS Verified Access

## What is it?
AWS Verified Access provides secure application access without VPN.

---

## Important Concept
Uses Zero Trust security model.

Meaning:
- Every request must be verified
- No automatic trust

---

## Benefits
- Secure remote access
- Identity-aware access control
- Better security posture

---

# Quick Revision Table

| Service | Main Purpose |
|---|---|
| Route Tables | Control traffic routing |
| Elastic Beanstalk | Easy app deployment |
| Neptune Streams | Real-time graph updates |
| Direct Connect | Dedicated AWS connection |
| Route 53 | DNS and traffic routing |
| App Mesh | Microservices communication |
| Gateway Load Balancer | Security appliance scaling |
| Cloud WAN | Global network management |
| Network Firewall | VPC network protection |
| Verified Access | Zero Trust application access |
