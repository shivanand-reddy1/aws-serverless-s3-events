# AWS Serverless S3 Events

## Description

A comprehensive case study project exploring Amazon Web Services (AWS) serverless architecture with S3 event-driven processing for course CS3532.

## Problem Statement

Traditional file processing systems require dedicated servers running 24/7, leading to high costs and maintenance overhead. This project demonstrates how to build a cost-effective, scalable, and event-driven file processing system using AWS serverless services.

## Features

- Event-driven architecture triggered by S3 bucket events
- Serverless compute with AWS Lambda
- Automatic scaling based on workload
- Pay-per-use pricing model
- Real-time file processing capabilities

## Tech Stack

| Technology     | Purpose                         |
| -------------- | ------------------------------- |
| AWS S3         | Object storage and event source |
| AWS Lambda     | Serverless compute              |
| AWS IAM        | Access management               |
| Python/Node.js | Lambda function runtime         |

## Installation

1. Clone this repository

   ```bash
   git clone https://github.com/yourusername/aws-serverless-s3-events.git
   cd aws-serverless-s3-events
   ```

2. Configure AWS CLI with your credentials

   ```bash
   aws configure
   ```

3. Deploy the infrastructure using AWS Console or CloudFormation (refer to case study report)

## Usage

1. Upload a file to the configured S3 bucket
2. The S3 event triggers the Lambda function automatically
3. View the processing results in CloudWatch logs

## Architecture

```
┌─────────┐     ┌─────────────┐     ┌─────────────┐
│  User   │────▶│   S3 Bucket │────▶│   Lambda    │
└─────────┘     └─────────────┘     └─────────────┘
                   (Event)            (Process)
```

Refer to `images/` folder and `AWS_Presentation.pdf` for detailed architecture diagrams.

## 📁 Project Contents

| File                                   | Description                         |
| -------------------------------------- | ----------------------------------- |
| `CS3532 Project Case Study Report.pdf` | Detailed case study report on AWS   |
| `AWS_Presentation.pdf`                 | Presentation slides for the project |
| `images/`                              | Supporting images and diagrams      |

## Limitations

- Cold start latency for Lambda functions
- Maximum execution time limit (15 minutes) for Lambda
- S3 event delivery is eventually consistent
- Limited to AWS ecosystem

## Future Scope

- Add support for multiple file formats
- Implement Step Functions for complex workflows
- Add SNS notifications for processing status
- Integrate with DynamoDB for metadata storage
- Implement error handling with Dead Letter Queues

## Learnings

- Understanding of serverless architecture patterns
- Event-driven programming concepts
- AWS service integration and IAM policies
- Cost optimization strategies in cloud computing
- Infrastructure as Code principles

## Author

**Shiva**

- College: CS3532 Course Project
- Purpose: Educational case study on AWS serverless architecture

## Pro Tip (For Placements / Interviews)

> A good README answers three questions clearly:
>
> 1. **What is this project?** - An AWS serverless application demonstrating S3 event-driven processing
> 2. **Why is it useful?** - Eliminates server management, scales automatically, and reduces costs
> 3. **How do I run it?** - Configure AWS CLI, deploy infrastructure, upload files to S3

### Key Interview Talking Points:

- Explain the difference between monolithic and serverless architectures
- Discuss event-driven vs polling-based approaches
- Highlight cost benefits of pay-per-invocation model
- Be ready to discuss trade-offs (cold starts, vendor lock-in)

---

## 📄 License

This project is for educational purposes.

---

_CS3532 - College Project_
