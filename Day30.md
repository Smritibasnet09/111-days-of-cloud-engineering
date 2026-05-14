# AWS Security & Services Notes

---

## AWS Systems Manager (SSM) Parameter Store
AWS service used to securely store configuration data, passwords, API keys, and secrets.

### Example:
- Store database password securely.
- EC2 instance retrieves the password during application startup.

---

## AWS Certificate Manager (ACM) – Requesting Public Certificate
AWS service used to create and manage SSL/TLS certificates for websites.

### Example:
- Use ACM certificate for HTTPS on:
  - Elastic Load Balancer (ELB)
  - CloudFront
  - API Gateway

---

# Layer 7 = Application Layer
Layer 7 refers to the Application Layer in the OSI model.

It handles:
- HTTP
- HTTPS
- APIs
- Web traffic

### Example:
- AWS WAF filters HTTP requests at Layer 7.

---

## AWS Shield
AWS service that protects applications from DDoS (Distributed Denial of Service) attacks.

### Features:
- 24/7 protection
- Automatic detection and mitigation

### Example:
- Protects a website hosted on CloudFront or ELB from traffic flooding attacks.

---

## AWS WAF (Web Application Firewall)
Protects web applications from common web attacks.

### Blocks:
- SQL Injection
- Cross-site scripting (XSS)
- Bad bots

### Example:
- Block requests from suspicious IP addresses.

---

## AWS Firewall Manager
Centralized security management service.

Used to manage:
- AWS WAF rules
- AWS Shield protections
- Security policies across multiple AWS accounts

### Example:
- Apply the same WAF rules to all company accounts automatically.

---

## AWS Inspector – Network Reachability
AWS Inspector checks security vulnerabilities and network exposure.

### Network Reachability:
Checks whether EC2 instances are reachable from the internet unexpectedly.

### Example:
- Detects if a private EC2 instance accidentally became publicly accessible.

---

## Amazon Elastic Container Registry (ECR)
A fully managed Docker container registry service.

Used to:
- Store Docker container images
- Manage container versions
- Deploy containers easily

### Example:
- Store Docker image for an application before deploying to ECS or EKS.

---

## AWS Macie
Security service that helps discover and protect sensitive data in Amazon S3.

Detects:
- PII (Personally Identifiable Information)
- Financial data
- Sensitive documents

### Example:
- Finds passport numbers or phone numbers inside S3 files.

---

## How does Macie detect PII if files are encrypted?
Macie can scan encrypted S3 objects if:
- AWS has permission to decrypt them.
- Encryption uses:
  - SSE-S3
  - SSE-KMS

Macie temporarily decrypts the file securely during scanning.

### Example:
- An encrypted PDF in S3 still gets scanned for credit card numbers.

---

## Automatic Rotation = AWS Secrets Manager
AWS Secrets Manager can automatically rotate secrets and passwords.

### Example:
- Automatically change RDS database password every 30 days.

---

# Disaster Recovery Concepts

## RPO (Recovery Point Objective)
Maximum acceptable amount of data loss measured in time.

### Example:
- RPO = 1 hour
- Means maximum 1 hour of data loss is acceptable.

---

## RTO (Recovery Time Objective)
Maximum acceptable downtime before systems recover.

### Example:
- RTO = 30 minutes
- System must be restored within 30 minutes after failure.

---