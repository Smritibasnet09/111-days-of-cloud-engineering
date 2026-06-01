# AWS Learning

## 1. AWS App Runner

**What it is:**  
A fully managed service that lets you deploy web apps and APIs directly from source code or container images without managing servers.

**Key Idea:**  
You don’t manage EC2, load balancers, or scaling — AWS handles everything.

**Example:**  
A startup deploys a Node.js API directly from GitHub. App Runner automatically builds, deploys, and scales it when traffic increases.

---

## 2. Amazon EventBridge

**What it is:**  
A serverless event bus that connects AWS services and applications using events.

**Key Idea:**  
It helps different services communicate without direct integration.

**Example:**  
When a file is uploaded to S3, EventBridge triggers a Lambda function to process it and send a notification.

---

## 3. Amazon SQS (Simple Queue Service)

**What it is:**  
A message queue service that decouples application components.

**Key Idea:**  
One service sends messages, another processes them later — improves reliability.

**Example:**  
An e-commerce site sends order details to SQS, and a separate service processes payments asynchronously.

---

## 4. Amazon EKS (Elastic Kubernetes Service)

**What it is:**  
A managed Kubernetes service used to run containerized applications.

**Key Idea:**  
AWS manages Kubernetes control plane, you manage worker nodes or use Fargate.

**Example:**  
A media company runs microservices (video upload, encoding, streaming) inside Kubernetes clusters using EKS.

---

## 5. AWS Step Functions

**What it is:**  
A workflow orchestration service used to coordinate multiple AWS services in a sequence.

**Key Idea:**  
You build state machines to automate complex workflows.

**Example:**  
A user uploads a photo → Step Function triggers Lambda → processes image → stores in S3 → sends notification.

---

# Quick Memory Trick

- App Runner → “Deploy app instantly”
- EventBridge → “Event routing system”
- SQS → “Message queue (decouple systems)”
- EKS → “Kubernetes in AWS”
- Step Functions → “Workflow automation”