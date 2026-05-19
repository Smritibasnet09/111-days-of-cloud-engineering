# AWS Notes

## 1. Amazon CloudFront

### What is CloudFront?
Amazon CloudFront is a Content Delivery Network (CDN) service used to deliver content faster to users worldwide.

### Why is it Important?
- Reduces latency
- Improves website speed
- Caches content near users
- Provides security with HTTPS

### Example
A company in Nepal hosts its website in the AWS Singapore Region.

Users from:
- Nepal
- India
- Japan
- USA

access the website.

Without CloudFront:
- All users request data directly from Singapore server
- Website becomes slower for distant users

With CloudFront:
- Content is cached at nearby Edge Locations
- Users receive content faster

### Important Terms
- Edge Location → Caching servers worldwide
- Origin → Original server (S3, EC2, ALB)
- Cache Hit → Content served from edge cache
- Cache Miss → Content fetched from origin

### Key Points
- Improves global performance
- Reduces server load
- Supports DDoS protection with AWS Shield

---

## 2. AWS Lambda

### What is AWS Lambda?
AWS Lambda is a serverless compute service that runs code without managing servers.

### Why is it Important?
- No server management
- Pay only when code runs
- Automatically scales
- Event-driven execution

### Example
A user uploads an image into S3 bucket.

Lambda automatically:
1. Detects upload event
2. Resizes image
3. Stores resized image in another bucket

### Common Triggers
- S3 uploads
- API Gateway requests
- CloudWatch events
- DynamoDB streams

### Key Points
- Supports Python, Node.js, Java, etc.
- Ideal for small automated tasks
- Reduces infrastructure management

---

## 3. Amazon VPC (Virtual Private Cloud)

### What is VPC?
Amazon VPC allows users to create a private network inside AWS.

### Why is it Important?
- Provides network isolation
- Improves security
- Controls traffic flow
- Enables custom networking

### Example
A company creates:
- Public subnet → Web servers
- Private subnet → Database servers

Internet users can access web servers only.
Database remains private and secure.

### Important Components
1. Subnets
   - Public Subnet
   - Private Subnet

2. Internet Gateway
   - Allows internet access

3. Route Table
   - Controls network routing

4. Security Groups
   - Virtual firewall for instances

### Key Points
- Highly secure networking
- Essential for AWS architecture
- Used in almost every production environment

---

## 4. Amazon DynamoDB

### What is DynamoDB?
Amazon DynamoDB is a fully managed NoSQL database service.

### Why is it Important?
- Very fast performance
- Automatic scaling
- Serverless database
- High availability

### Example
A gaming application stores:
- Player scores
- Rankings
- Live session data

inside DynamoDB because it requires very fast response time.

### Important Features
1. Partition Key
   - Used to distribute data

2. Global Secondary Index (GSI)
   - Allows additional query patterns

3. DynamoDB Streams
   - Tracks data changes

### Key Points
- Millisecond response time
- Suitable for real-time applications
- Handles massive traffic automatically

---

# Quick Summary Table

| Service | Main Purpose | Example |
|---|---|---|
| CloudFront | Faster content delivery | Cache website globally |
| Lambda | Serverless computing | Auto image resize |
| VPC | Private cloud network | Secure application setup |
| DynamoDB | NoSQL database | Gaming leaderboard system |