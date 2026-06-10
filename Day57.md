# AWS Learning Notes - 5 New Important Topics

## 1. AWS IAM (Identity and Access Management)

### What is it?

IAM is a service that controls **who can access what** in AWS.

### Why Use It?

* Security for AWS resources
* Control user permissions
* Prevent unauthorized access

### Example

You create two users:

* Admin → Full access to AWS
* Student → Only read access to S3

### Real-World Use Case

A company gives developers access only to EC2 but not to billing data.

---

## 2. Amazon VPC (Virtual Private Cloud)

### What is it?

VPC is your **private network inside AWS**.

### Why Use It?

* Secure cloud networking
* Control IP ranges
* Isolate resources

### Example

You create:

* Public subnet → Web server
* Private subnet → Database

### Real-World Use Case

A banking system keeps its database in a private subnet so no one can access it from the internet.

---

## 3. AWS Lambda

### What is it?

Lambda is a **serverless compute service** that runs code only when needed.

### Why Use It?

* No server management
* Pay only when code runs
* Auto-scaling

### Example

When a user uploads an image to S3:

1. Lambda automatically runs
2. Resizes the image
3. Stores it back in S3

### Real-World Use Case

Processing user uploads in social media apps.

---

## 4. Amazon CloudFront

### What is it?

CloudFront is a **Content Delivery Network (CDN)** that delivers data faster globally.

### Why Use It?

* Faster website loading
* Global content delivery
* Low latency

### Example

A user in Nepal opens a website hosted in the US:

* CloudFront serves cached content from the nearest edge location (Asia)

### Real-World Use Case

Streaming platforms like Netflix use CDN for fast video delivery.

---

## 5. Amazon DynamoDB

### What is it?

DynamoDB is a **NoSQL database** that is fast and fully managed.

### Why Use It?

* Very fast performance
* Scales automatically
* No server management

### Example

A mobile app stores:

* User ID
* Username
* Messages

### Real-World Use Case

Real-time gaming leaderboards and chat applications.

---

# Quick Revision Table

| Service    | Main Purpose          | Simple Example                |
| ---------- | --------------------- | ----------------------------- |
| IAM        | Access Control        | Admin vs Student permissions  |
| VPC        | Private Cloud Network | Public + Private subnet setup |
| Lambda     | Serverless Compute    | Image processing on upload    |
| CloudFront | CDN for speed         | Fast website loading globally |
| DynamoDB   | NoSQL Database        | Chat app data storage         |

---

# Exam Keywords

### IAM

Security, Users, Roles, Policies

### VPC

Subnet, Route Table, Internet Gateway

### Lambda

Event-driven, Serverless, Pay-per-use

### CloudFront

CDN, Edge Location, Low Latency

### DynamoDB

NoSQL, Key-value store, Fast scaling

---

# Summary

These AWS services are core building blocks:

* IAM → Controls access
* VPC → Builds secure networks
* Lambda → Runs code without servers
* CloudFront → Speeds up global content
* DynamoDB → Fast NoSQL database

Mastering these will help you understand most real AWS architectures.
