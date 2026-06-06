# AWS New Topics 

---

# 1. AWS Cloud WAN

## What is AWS Cloud WAN?

AWS Cloud WAN (Wide Area Network) is a managed networking service that helps organizations connect multiple AWS Regions, VPCs, branch offices, and on-premises data centers through a centralized network.

Instead of creating many VPC peering connections or managing multiple Transit Gateways, Cloud WAN provides a single place to manage global connectivity.

## Why Use It?

- Centralized network management
- Connects multiple AWS Regions
- Simplifies global networking
- Reduces operational complexity
- Improves network visibility

## How It Works

1. Create a Cloud WAN core network.
2. Connect VPCs, branch offices, and data centers.
3. AWS automatically manages routing.
4. Traffic flows securely across the global network.

## Real-World Example

A multinational company has offices in:

- Nepal
- India
- Australia
- USA

Instead of managing separate VPN connections and Transit Gateways, they use Cloud WAN to manage all locations from one dashboard.

## Exam Tip

Cloud WAN = Global Network Management

### Keyword

"Centralized networking across multiple AWS Regions"

---

# 2. AWS Verified Access

## What is AWS Verified Access?

AWS Verified Access provides secure access to applications without requiring traditional VPNs.

It continuously verifies both the user's identity and the device's security posture before granting access.

This follows the Zero Trust security model.

## Why Use It?

- Eliminates traditional VPNs
- Improves security
- Supports remote workers
- Continuously validates access requests
- Implements Zero Trust Architecture

## How It Works

1. User requests application access.
2. Verified Access checks identity.
3. Device security status is verified.
4. Access is granted only if all requirements are met.

## Real-World Example

An employee working from home wants to access a company dashboard.

AWS checks:

- Is the employee authenticated?
- Is the laptop secure and compliant?

If both checks pass, access is allowed.

## Exam Tip

Verified Access = Secure Access Without VPN

### Keyword

"Zero Trust Security"

---

# 3. Amazon CodeWhisperer

## What is Amazon CodeWhisperer?

Amazon CodeWhisperer is an AI-powered coding assistant that helps developers write code faster by generating real-time code suggestions.

It integrates directly into development environments.

## Why Use It?

- Increases productivity
- Reduces coding time
- Generates code automatically
- Supports multiple programming languages
- Helps learn AWS SDK usage

## How It Works

1. Developer writes a comment or code.
2. CodeWhisperer analyzes context.
3. AI suggests complete code snippets.
4. Developer accepts or modifies suggestions.

## Real-World Example

A developer writes:

"Upload a file to Amazon S3"

CodeWhisperer automatically suggests the required SDK code.

## Exam Tip

CodeWhisperer = AI Coding Assistant

### Keyword

"Generative AI for Developers"

---

# 4. Amazon Bedrock

## What is Amazon Bedrock?

Amazon Bedrock is a fully managed service that provides access to Foundation Models (FMs) from multiple AI providers.

Developers can build Generative AI applications without managing infrastructure or training models.

## Why Use It?

- Build chatbots
- Generate text
- Generate images
- Summarize content
- Create AI-powered applications

## How It Works

1. Select a Foundation Model.
2. Send prompts through API calls.
3. Receive AI-generated responses.
4. Integrate into applications.

## Real-World Example

A company wants an AI chatbot for customer support.

Using Bedrock:

- No GPU management needed
- No model training required
- AWS handles infrastructure

## Exam Tip

Bedrock = Managed Generative AI Platform

### Keyword

"Foundation Models as a Service"

---

# 5. AWS App Runner

## What is AWS App Runner?

AWS App Runner is a fully managed service for deploying web applications and APIs directly from source code repositories or container images.

AWS automatically handles infrastructure management and scaling.

## Why Use It?

- No server management
- Automatic scaling
- Easy deployment
- Built-in load balancing
- Faster development lifecycle

## How It Works

1. Connect source code repository.
2. AWS builds the application.
3. AWS deploys the application.
4. App Runner automatically scales based on traffic.

## Real-World Example

A startup creates a Node.js web application.

After pushing code to GitHub:

- App Runner builds the application
- Deploys automatically
- Scales when traffic increases

No EC2 management is required.

## Exam Tip

App Runner = Deploy Applications Without Managing Servers

### Keyword

"Serverless Application Deployment"

---

# Quick Revision Table

| Service | Purpose | Keyword |
|----------|----------|----------|
| AWS Cloud WAN | Global network management | Centralized Networking |
| AWS Verified Access | Secure application access | Zero Trust |
| Amazon CodeWhisperer | AI coding assistant | Code Generation |
| Amazon Bedrock | Generative AI platform | Foundation Models |
| AWS App Runner | Web application deployment | Serverless Deployment |

---

# One-Line Memory Tricks

## AWS Cloud WAN

One network to connect all AWS Regions and offices.

## AWS Verified Access

Secure application access without VPN.

## Amazon CodeWhisperer

AI assistant that writes code for developers.

## Amazon Bedrock

Build Generative AI applications without managing models.

## AWS App Runner

Deploy web applications without managing servers.

---

# Exam Cheat Sheet

Cloud WAN
→ Global networking

Verified Access
→ Zero Trust security

CodeWhisperer
→ AI code generation

Bedrock
→ Generative AI service

App Runner
→ Serverless web application deployment