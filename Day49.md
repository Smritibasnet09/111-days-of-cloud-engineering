# AWS Emerging & Advanced Services (New Topics)

## 1. AWS App Runner

### What is AWS App Runner?

AWS App Runner is a fully managed service that allows developers to deploy web applications and APIs directly from source code or container images without managing servers.

### Key Features

* Automatic deployment
* Built-in load balancing
* Auto scaling
* HTTPS support
* Minimal infrastructure management

### Example

A startup creates a Flask API for an AI chatbot.

Workflow:

1. Developer pushes code to GitHub
2. App Runner automatically deploys the application
3. Traffic increases
4. App Runner scales automatically
5. Users access the API without downtime

### Real-World Use Case

* Startup applications
* REST APIs
* AI-powered web services

---

## 2. Amazon Bedrock

### What is Amazon Bedrock?

Amazon Bedrock allows developers to build Generative AI applications using foundation models without managing infrastructure.

### Key Features

* Access to multiple AI models
* Serverless AI platform
* API-based integration
* Security and governance controls
* Fine-tuning capabilities

### Example

A company builds an AI document assistant.

Workflow:

1. Employee uploads a PDF
2. Application sends content to Bedrock
3. AI summarizes the document
4. User receives key insights instantly

### Real-World Use Case

* AI chatbots
* Content generation
* Document analysis

---

## 3. Amazon OpenSearch Service

### What is Amazon OpenSearch Service?

Amazon OpenSearch Service helps organizations search, analyze, and visualize large volumes of data in real time.

### Key Features

* Full-text search
* Log analytics
* Dashboards and visualizations
* Real-time monitoring
* Scalable clusters

### Example

An e-commerce platform tracks customer searches.

Workflow:

1. User searches for "gaming laptop"
2. OpenSearch indexes product data
3. Results are returned within milliseconds
4. Analytics show trending searches

### Real-World Use Case

* Website search engines
* Log monitoring
* Security analytics

---

## 4. AWS Proton

### What is AWS Proton?

AWS Proton helps platform teams automatically deploy and manage infrastructure for container and serverless applications.

### Key Features

* Infrastructure templates
* Standardized deployments
* CI/CD integration
* Centralized governance
* Environment management

### Example

A company has 50 developers creating microservices.

Workflow:

1. Platform team creates approved templates
2. Developers select a template
3. Proton automatically provisions infrastructure
4. Service is deployed consistently

### Real-World Use Case

* Enterprise DevOps
* Large engineering teams
* Standardized cloud deployments

---

## 5. Amazon Managed Grafana

### What is Amazon Managed Grafana?

Amazon Managed Grafana is a fully managed visualization service used to monitor applications and infrastructure.

### Key Features

* Interactive dashboards
* AWS integration
* Real-time monitoring
* Alerting support
* Team collaboration

### Example

A company monitors its cloud infrastructure.

Workflow:

1. CloudWatch collects metrics
2. Grafana reads the metrics
3. Dashboards display CPU, memory, and network usage
4. Alerts are triggered if thresholds are exceeded

### Real-World Use Case

* Cloud monitoring
* DevOps observability
* Performance tracking

---

# Summary Table

| Service                | Purpose                     | Example                                |
| ---------------------- | --------------------------- | -------------------------------------- |
| AWS App Runner         | Deploy apps without servers | Deploy Flask API from GitHub           |
| Amazon Bedrock         | Build Generative AI apps    | AI document summarizer                 |
| Amazon OpenSearch      | Search and analytics        | E-commerce search engine               |
| AWS Proton             | Standardized deployments    | Microservice infrastructure automation |
| Amazon Managed Grafana | Monitoring dashboards       | Cloud infrastructure monitoring        |

---


