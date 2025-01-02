# Connecting a Web Application to Amazon Aurora
> A guide to setting up a PHP web application on EC2 connected to Amazon Aurora database

## Project Overview
This project demonstrates how to create and deploy a PHP web application on Amazon EC2 that connects to an Amazon Aurora database. The implementation includes setting up the web server, configuring database connections, and testing the complete system.

## Time Investment
- Total project completion time: 2 hours and 25 minutes
- Includes setup, configuration, and troubleshooting time

## Prerequisites
Required dependencies:
- Apache HTTP Server (httpd)
- PHP
- php-mysqli (MySQL extension for PHP)
- MariaDB
- MySQL repository

## Implementation Steps

### 1. EC2 Instance Setup
- SSH access using PEM key
- Installation of required dependencies
- Configuration of web server environment

### 2. Database Connection Setup
Created database connection configuration:
- Created `dbinfo.inc` file using nano
- Defined PHP connection details
- Configured secure access parameters

### 3. Web Application Development
- Created PHP-based sample page
- Stored in dedicated HTML directory
- Implemented database interactions

### 4. Testing and Verification
Testing procedure:
1. Download MySQL repository to EC2
2. Connect to Aurora DB using MySQL
3. Query database to verify:
   - Database structure
   - Database contents
   - Connection stability

## Technical Components

### Web Server
- Apache HTTP Server
- PHP runtime environment
- MySQL extensions

### Database
- Amazon Aurora RDS
- MariaDB compatibility
- MySQL repository integration

## Configuration Details

### Required Files
- PEM key for EC2 access
- dbinfo.inc for database configuration
- PHP sample pages
- HTML directory structure

## Troubleshooting
The project required significant troubleshooting, including:
- Database connection issues
- Configuration verification
- Access permission settings
- Dependency compatibility

## Best Practices
1. Secure key management
2. Proper configuration file organization
3. Systematic testing approach
4. Comprehensive dependency management

## Security Considerations
- Secure SSH access using PEM keys
- Protected database credentials
- Configured access permissions
- Secure file storage

## Future Enhancements
Potential improvements:
- Add more interactive features
- Implement caching
- Enhance security measures
- Optimize database queries

## About
This project was created as part of NextWork.org's educational program. NextWork.org believes everyone should be in a job they love.

## Additional Resources
For more projects and learning opportunities, visit [NextWork.org](https://nextwork.org)

