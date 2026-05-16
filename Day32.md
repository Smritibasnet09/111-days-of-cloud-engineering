# AWS CloudTrail
- Records AWS API calls and user activities.
- Used for auditing, security, and compliance.
- Tracks:
  - Who did the action
  - What action was done
  - When it happened
- Logs are commonly stored in S3.

## Exam Trick
CloudTrail = "Who did what"

---

# AWS CloudWatch
- Monitors AWS resources and applications.
- Tracks:
  - CPU usage
  - Memory
  - Errors
  - Logs
- Can trigger alarms and notifications.

## Exam Trick
CloudWatch = "Watch system health"

---

# Kinesis Data Analytics
- Processes streaming data in real time.
- Used for:
  - Live analytics
  - Fraud detection
  - Real-time monitoring

## Examples
- Website clicks
- IoT sensor data
- Banking transactions

## Exam Trick
Kinesis = "Flowing live data"

---

# AWS Data Lake
- Centralized storage for huge amounts of raw data.
- Stores:
  - Structured data
  - Semi-structured data
  - Unstructured data
- Usually built using S3.

## Exam Trick
Data Lake = "Big storage lake for raw data"

---

# AWS Glue
- Serverless ETL service.
- ETL = Extract, Transform, Load
- Used to:
  - Clean data
  - Transform data
  - Prepare data for analytics

## Important Components
- Glue Crawler → Automatically finds schema
- Data Catalog → Stores metadata

## Exam Trick
Glue = "Glue data together"

---

# Quick Difference Table

| Service | Purpose |
|---|---|
| CloudTrail | Audit user/API activity |
| CloudWatch | Monitor performance |
| Kinesis | Real-time streaming analytics |
| Data Lake | Store raw data |
| Glue | Clean and prepare data |