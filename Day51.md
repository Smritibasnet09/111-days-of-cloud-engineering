# AWS Important Topics with Examples

## 1. Amazon Athena

Topic
Amazon Athena is a serverless service that helps users run SQL queries directly on data stored in S3.

Example
A company stores log files in S3 and wants to analyze the data using SQL without creating servers or databases. In this case, Athena is the best solution.

---

## 2. CloudFront

Topic
CloudFront is a content delivery network that helps deliver content faster to users around the world.

Example
A website has users from different countries and the images are loading slowly. CloudFront stores cached copies in nearby locations to improve speed and reduce latency.

---

## 3. Multi-AZ

Topic
Multi-AZ is used in RDS to provide high availability and automatic failover.

Example
A banking application needs the database to continue working even if one Availability Zone fails. Multi-AZ creates a standby database in another zone for backup and failover.

---

## 4. Read Replica

Topic
Read Replica is used to improve database read performance.

Example
A social media application receives millions of read requests every day and the main database becomes overloaded. Read Replica creates additional read-only copies to reduce the load.

---

## 5. DynamoDB

Topic
DynamoDB is a serverless NoSQL database designed for high speed and massive scalability.

Example
A gaming application needs very fast response time for millions of users worldwide. DynamoDB is suitable because it provides low latency and automatic scaling.
