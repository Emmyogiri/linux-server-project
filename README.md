# AWS EC2 Nginx Server Setup

## Overview
This project documents the process of setting up an Nginx web server on an AWS EC2 instance. Nginx is a popular web server known for its performance, scalability, and ease of configuration.

## Steps to Set Up the Server
1. **Launch an EC2 Instance**:
   - Sign up for an AWS account if you haven't already.
   - Access the AWS Management Console and navigate to the EC2 dashboard.
   - Launch a new EC2 instance, choosing the desired Amazon Machine Image (AMI) and instance type.

2. **Install Nginx**:
   - Connect to the EC2 instance via SSH.
   - Update the package repository: `sudo apt update`.
   - Install Nginx: `sudo apt install nginx`.

3. **Configure Nginx**:
   - Start the Nginx service: `sudo systemctl start nginx`.
   - Enable Nginx to start on boot: `sudo systemctl enable nginx`.

4. **Configure Security**:
   - Ensure that port 80 (HTTP) is open inbound in the security group associated with your EC2 instance.

5. **Test Nginx**:
   - Open a web browser and enter your EC2 instance's public IP address to verify that Nginx is serving content.

6. **Document Progress on GitHub**:
   - Create a new repository on GitHub for your server project.
   - Write a detailed README.md file documenting the setup process and any configurations made.

7. **Test and Monitor**:
   - Test your Nginx server by accessing it through the browser.
   - Set up monitoring tools (e.g., AWS CloudWatch) to track server performance and uptime.

## Resources
- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
- [Nginx Documentation](https://nginx.org/en/docs/)

## Author
- Emmanuel Ogiri (https://github.com/Emmyogiri)
