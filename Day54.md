# AWS Advanced Topics - Part 1

## 1. AWS Step Functions

### What is AWS Step Functions?

AWS Step Functions is a serverless workflow service that helps you coordinate multiple AWS services into automated workflows.

### Why Use It?

* Automates business processes
* Reduces application complexity
* Visual workflow monitoring
* Error handling and retries

### Example

Imagine an online shopping system:

1. Customer places an order
2. Verify payment
3. Check inventory
4. Ship product
5. Send confirmation email

Step Functions can automate the entire process from start to finish.

---

## 2. Amazon EventBridge

### What is Amazon EventBridge?

Amazon EventBridge is an event bus service that connects applications using events.

### Why Use It?

* Event-driven architecture
* Connect AWS services easily
* Real-time automation
* Supports SaaS integrations

### Example

When a file is uploaded to S3:

* EventBridge detects the upload
* Triggers a Lambda function
* Lambda processes the file automatically

No manual action required.

---

## 3. AWS App Runner

### What is AWS App Runner?

AWS App Runner is a fully managed service that deploys web applications and APIs directly from source code or containers.

### Why Use It?

* No server management
* Automatic scaling
* Simple deployment
* Built-in HTTPS support

### Example

You build a Node.js website.

Instead of:

* Creating EC2 instances
* Configuring load balancers
* Managing scaling

Simply connect your GitHub repository to App Runner and deploy.

---

## 4. Amazon OpenSearch Service

### What is Amazon OpenSearch Service?

OpenSearch helps you search, analyze, and visualize large amounts of data in real time.

### Why Use It?

* Fast searching
* Log analysis
* Monitoring applications
* Data visualization

### Example

A company stores millions of application logs.

With OpenSearch:

* Search errors instantly
* Monitor system health
* Create dashboards for analytics

---

## 5. AWS Global Accelerator

### What is AWS Global Accelerator?

AWS Global Accelerator improves application performance by routing user traffic through AWS's global network.

### Why Use It?

* Lower latency
* Better availability
* Faster global access
* Automatic failover

### Example

Users from:

* Nepal
* Japan
* USA
* Germany

access the same application.

Global Accelerator routes each user through the nearest AWS edge location, reducing delays and improving speed.

---

# Quick Summary

| Service                | Main Purpose                |
| ---------------------- | --------------------------- |
| AWS Step Functions     | Automate workflows          |
| Amazon EventBridge     | Event-driven automation     |
| AWS App Runner         | Easy application deployment |
| Amazon OpenSearch      | Search and analytics        |
| AWS Global Accelerator | Improve global performance  |

## Real-World Architecture Example

User Uploads File → Amazon S3 → EventBridge → Lambda → OpenSearch

OR

User → Global Accelerator → App Runner → Database

These services help create scalable, automated, and highly available cloud applications.
