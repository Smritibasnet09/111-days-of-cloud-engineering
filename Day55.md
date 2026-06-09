# AWS Learning Notes

## 1. AWS Step Functions

### What is it?
AWS Step Functions helps connect multiple AWS services into a workflow and executes them in the correct order.

### Example
A food delivery app:
1. Customer places an order.
2. Payment is processed.
3. Restaurant receives the order.
4. Delivery partner is assigned.

---

## 2. Amazon EventBridge

### What is it?
Amazon EventBridge allows AWS services and applications to communicate using events.

### Example
When a user uploads a file to S3:
- EventBridge detects the upload.
- A Lambda function starts automatically.
- The file is processed.

---

## 3. AWS Global Accelerator

### What is it?
AWS Global Accelerator improves application speed and availability for users around the world.

### Example
A gaming company has players in different countries.
Global Accelerator routes players through the fastest AWS network path, reducing lag.

---

## 4. Amazon FSx

### What is it?
Amazon FSx provides fully managed file storage systems for different workloads.

### Example
A company needs a shared Windows file server.
Instead of managing servers manually, it uses Amazon FSx for Windows File Server.

---

## 5. AWS AppConfig

### What is it?
AWS AppConfig helps safely deploy configuration changes without changing application code.

### Example
A company enables a new feature for only 10% of users first.
If no issues occur, the feature is rolled out to everyone.

---

# Quick Revision

| Service | Purpose |
|----------|----------|
| AWS Step Functions | Workflow automation |
| Amazon EventBridge | Event-driven communication |
| AWS Global Accelerator | Faster global application access |
| Amazon FSx | Managed file systems |
| AWS AppConfig | Safe configuration management |