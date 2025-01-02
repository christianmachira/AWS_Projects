# Implementing a Serverless Architecture on AWS
> A comprehensive guide to building a serverless inventory tracking system using AWS services

## Project Overview
This project implements a serverless inventory tracking system that allows stores worldwide to upload inventory files to Amazon S3. The system processes these files, stores the data, monitors inventory levels, and sends automated notifications for low stock situations.

## Architecture Components
- AWS Lambda for serverless computing
- Amazon S3 for file storage
- Amazon DynamoDB for data storage
- Amazon Cognito for authentication
- Amazon SNS for notifications

## Implementation Steps

### 1. Lambda Function for Data Loading
Created a Lambda function that:
- Triggers automatically when files are uploaded to S3
- Downloads and processes inventory files
- Inserts data into DynamoDB
- Maximum runtime: 15 minutes

### 2. S3 Bucket Configuration
- Created bucket named "inventory-69"
- Configured S3 event triggers to invoke Lambda function
- Set up appropriate permissions and access controls

### 3. Web Dashboard Setup
- Implemented serverless web-based dashboard
- Integrated Amazon Cognito for authentication
- Connected dashboard to DynamoDB for data display
- Enabled real-time inventory level monitoring

### 4. Notification System
Components:
1. Second Lambda function for monitoring inventory levels
2. SNS topic configuration for notifications
3. Email notification setup for zero-stock alerts

Key Features:
- Separate Lambda functions for loading and notifications (following single responsibility principle)
- Automated email alerts for out-of-stock items
- Real-time inventory monitoring

## System Testing
Testing procedures include:
1. Uploading CSV files to S3 bucket
2. Verifying data appears in dashboard
3. Confirming email notifications for zero-stock items
4. Validating end-to-end system functionality

## Advantages of Serverless Architecture
1. Infrastructure Management
   - Cloud provider handles all infrastructure
   - Focus solely on application code
   
2. Cost Efficiency
   - Pay only for actual compute time
   - No costs for idle servers
   
3. Scalability
   - Automatic resource scaling based on demand
   - No manual intervention required

## System Flow
1. Stores upload inventory files to S3
2. Lambda function processes uploads
3. Data stored in DynamoDB
4. Dashboard displays current inventory
5. Monitoring Lambda checks stock levels
6. SNS sends notifications for low stock

## Technical Considerations
- Lambda function runtime limit: 15 minutes
- Separate Lambda functions for different responsibilities
- Event-driven architecture
- Fully managed services

## Best Practices Implemented
- Separation of concerns in Lambda functions
- Event-driven architecture
- Automated monitoring and alerting
- Secure authentication with Cognito
- Scalable data storage with DynamoDB

## Future Enhancements
Potential improvements could include:
- Additional notification channels
- Advanced analytics
- Historical data tracking
- Predictive inventory management

## Author
Christian Machira

