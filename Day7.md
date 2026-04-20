# Day 7 of Cloud Learning

Today I am revising and understanding the following topics:
- Internet Gateway  
- Route Table  
- Bastion Host  

My goal is to clearly understand the concepts and also remember key points for MCQs.

---

# Internet Gateway (IGW)

Internet Gateway is used to connect a VPC to the internet.  
If I want an EC2 instance inside a VPC to communicate with the internet, an IGW is required.

However, one important point is:
IGW alone does not provide internet access.

It acts as a gateway, but proper configuration is required for communication to work.

---

## How it actually works

For internet access, all of the following must be present:

- IGW must be attached to the VPC  
- Route table must contain: 0.0.0.0/0 → IGW

Instance must have:
- Public IP or Elastic IP  
- Security Groups and Network ACLs must allow traffic  

If any of these are missing, internet access will not work.

---

## Concept understanding

I can think of it as:

- IGW → entry/exit point  
- Route Table → path for traffic  
- Public IP → identity on internet  
- Security → permission  

All components must work together.

---

## MCQ tips 

- IGW alone provides internet → Incorrect  
- IGW must be attached to VPC → Correct  
- Only one IGW per VPC → Correct  
- IGW is attached to subnet → Incorrect  

---

# Route Table

A Route Table controls how network traffic flows within a VPC.  
It defines where traffic should go based on defined rules.

---

## Basic structure

Each route follows: Destination → Target


Examples:
- `0.0.0.0/0 → IGW` → traffic goes to internet  
- `VPC CIDR → local` → internal communication  

---

## Key understanding

- Every subnet must be associated with a route table  
- A main (default) route table is automatically created  
- Custom route tables can be created for better control  

---

## Concept understanding

Route table works like a traffic controller that directs packets to the correct destination.

---

## MCQ focus points

- Route table works at subnet level → Correct  
- One subnet can have multiple route tables → Incorrect  
- Route table is optional → Incorrect  
- Without proper route, traffic will fail → Correct  

---

# Bastion Host

A Bastion Host is used to securely access instances in a private subnet.

It is a special EC2 instance placed in a public subnet.

---

## How it works

Instead of directly connecting to private instances: User → Bastion Host → Private EC2


---

## Key understanding

- Acts as a secure entry point  
- Prevents direct exposure of private instances  
- Allows controlled access and monitoring  

---

## Concept understanding

Bastion Host is mainly used for security and controlled access, not for providing internet connectivity.

---

## MCQ focus points

- Bastion Host is placed in public subnet → Correct  
- Used for secure access → Correct  
- Provides internet access → Incorrect  
- Direct access to private instance from internet → Incorrect  

---

# Final Revision

- Internet Gateway enables internet connectivity but requires proper routing and configuration  
- Route Table controls traffic direction inside the VPC  
- Bastion Host provides secure access to private instances  

---

# Final Understanding

Internet communication in a VPC is not dependent on a single component.  
It is a combination of:

- Internet Gateway  
- Route Table  
- Public IP  
- Security configuration  

Bastion Host is an additional security mechanism used for controlled access.

This helped me clearly understand how connectivity and security work together in AWS networking.