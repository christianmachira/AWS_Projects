# Host a Website on Amazon S3
> A guide to hosting static websites using Amazon S3 bucket

## Project Overview
This project demonstrates how to host a static website using Amazon S3 (Simple Storage Service). The implementation takes advantage of S3's high availability, auto-scaling capabilities, and cost-effective pay-as-you-go model.

## Time Investment
- Project completion time: Approximately 1 hour
- Setup time for S3 bucket: Less than 5 minutes

## Implementation Steps

### 1. Setting Up the S3 Bucket
- Created a bucket in the `us-west-2` region
  - Chosen for lower pricing compared to us-east-1
  - Benefits from newer infrastructure
- Enabled required features:
  - Access Control Lists (ACLs)
  - Public Access
  - Versioning
- Note: S3 bucket names must be globally unique across all AWS accounts

### 2. File Upload
Uploaded necessary website files to the S3 bucket:
- `index.html` file (main website structure)
- Images folder (website content)

### 3. Configuring Static Website Hosting
1. Enabled Static Website Hosting in bucket properties
2. Configured the bucket to point to the HTML file
3. Set up Access Control Lists (ACL) to manage resource access

### 4. Managing Bucket Endpoints
- Upon enabling static website hosting, S3 generates a region-specific bucket endpoint URL
- This URL serves as the hosting location for the website
- Region: us-west-2

### 5. Troubleshooting
Common Issues:
- **403 Forbidden Error**: Occurs when bucket objects are set to private
- **Resolution**: Enable public access permissions via ACLs for bucket objects

## Key Learnings
- S3 provides a versatile platform for website hosting
- Quick setup process with comprehensive learning opportunities
- Importance of proper access configuration
- Understanding of S3's public access and ACL mechanisms

## Features Utilized
- Static Website Hosting
- Access Control Lists (ACLs)
- Public Access Management
- Versioning
- Region-specific endpoints

## About
This project was created as part of NextWork.org's educational program. NextWork.org believes everyone should be in a job they love.

## Additional Resources
For more projects and learning opportunities, visit [NextWork.org](https://nextwork.org)
