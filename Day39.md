# AWS Shield & Shield Advanced

## What is AWS Shield?
AWS Shield is a managed Distributed Denial of Service (DDoS) protection service provided by AWS.

It helps protect applications and websites from malicious traffic and cyber attacks.

---

# Types of AWS Shield

## 1. AWS Shield Standard

### Description
AWS Shield Standard is automatically enabled for all AWS customers at no additional cost.

It provides protection against common network and transport layer DDoS attacks.

### Features
- Free for all AWS users
- Automatic protection
- Real-time attack detection
- Protects:
  - Amazon EC2
  - Elastic Load Balancer (ELB)
  - Amazon CloudFront
  - Amazon Route 53

### Example
A blog website hosted on EC2 receives fake traffic from attackers.  
AWS Shield Standard automatically helps reduce the attack traffic.

---

## 2. AWS Shield Advanced

### Description
AWS Shield Advanced provides enhanced DDoS protection for critical applications.

It includes advanced monitoring, detailed reports, and support from the AWS DDoS Response Team (DRT).

### Features
- Advanced DDoS mitigation
- 24/7 AWS DRT support
- Detailed attack visibility
- Cost protection during attacks
- Integration with AWS WAF

### Example
An online banking system uses Shield Advanced to protect customer services during massive DDoS attacks.

---

# Difference Between Shield Standard and Shield Advanced

| Feature | Shield Standard | Shield Advanced |
|---|---|---|
| Pricing | Free | Paid |
| Basic Protection | Yes | Yes |
| Advanced Detection | No | Yes |
| DRT Support | No | Yes |
| Cost Protection | No | Yes |
| Best For | Small apps | Enterprise apps |

---

# Services Used with AWS Shield

## AWS WAF
AWS WAF filters malicious HTTP requests.

### Example
Block suspicious IP addresses trying to access a website.

---

## Amazon CloudFront
CloudFront distributes content globally and helps absorb attack traffic.

### Example
A video streaming platform uses CloudFront for faster and safer content delivery.

---

## Amazon Route 53
Route 53 is a DNS web service with built-in DDoS protection.

### Example
Users can still access a website during traffic spikes.

---

# Important Exam Points

- Shield Standard is free and automatically enabled.
- Shield Advanced is a paid service.
- Shield Advanced provides AWS DRT support.
- AWS WAF works together with Shield.
- CloudFront and Route 53 commonly use Shield protection.

---

# Quick MCQ Notes

- Standard = Basic + Free
- Advanced = Extra Security + Paid

---

# Real-World Scenario

An e-commerce company hosts its website using:
- Amazon EC2
- CloudFront
- Route 53
- AWS WAF

To protect against large DDoS attacks and get expert AWS support, the company uses AWS Shield Advanced.