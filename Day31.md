# AWS Network Firewall
- A managed firewall service that protects AWS Virtual Private Clouds (VPCs).
- Helps filter and monitor inbound and outbound network traffic.
- Supports:
  - Stateful inspection
  - Stateless filtering
  - Intrusion prevention
  - Domain and IP blocking
- Can be integrated with AWS Firewall Manager for centralized management.
- Useful for:
  - Securing applications
  - Blocking malicious traffic
  - Enforcing network security rules

---

# Amazon Elastic Compute Cloud (EC2)
- AWS service that provides resizable virtual servers in the cloud.
- Allows users to launch and manage instances quickly.
- Common uses:
  - Hosting websites
  - Running applications
  - Databases
  - Development and testing
- Key Features:
  - Auto Scaling
  - Elastic Load Balancing
  - Multiple instance types
  - Security Groups
  - EBS storage integration

---

# EC2 Hibernate
EC2 Hibernate allows an instance to save its in-memory (RAM) state to the EBS root volume and resume later from the same state.

## When Hibernated
- Instance moves to the **stopping** state.
- Operating system saves RAM contents to disk.
- Instance stops without deleting storage.
- On restart:
  - OS restores saved memory state.
  - Applications resume exactly where they stopped.
- Provides much faster startup compared to normal reboot.

## EC2 Hibernate - Good to Know
- Supported Instance Families:
  - C3, C4, C5
  - I3
  - M3, M4
  - R3, R4
  - T2, T3
- RAM size must be less than **150 GB**.
- Not supported for **bare metal instances**.
- Supported AMIs:
  - Amazon Linux 2
  - Ubuntu
  - RHEL
  - CentOS
  - Windows
- Root volume requirements:
  - Must be EBS-backed
  - Must be encrypted
  - Must be large enough
  - Cannot use instance store
- Available for:
  - On-Demand Instances
  - Reserved Instances
  - Spot Instances
- An instance cannot remain hibernated for more than **60 days**.

---

# EBS (Elastic Block Store)
- Block storage service used with EC2 instances.
- Provides persistent storage even after instance stop/start.
- Commonly used as:
  - Root volume
  - Data storage
  - Database storage
- Features:
  - High availability
  - Snapshots and backups
  - Encryption support
  - SSD and HDD volume types
- EBS volumes can be attached, detached, and resized easily.