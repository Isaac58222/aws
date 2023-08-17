# Project 2: VPC Deployment with Auto Scaling and Load Balancing with Public-Private subnets

## Overview

This project showcases the implementation of a robust Virtual Private Cloud (VPC) environment designed for production servers. The project employs advanced AWS services to ensure high availability, scalability, and security.

## Key Features

- Deployment of Servers in Two Availability Zones for enhanced availability and fault tolerance.
- Utilization of Auto Scaling Group to automatically adjust the number of instances based on traffic load.
- Implementation of Application Load Balancer to distribute incoming traffic across instances.
- Secure Deployment in Private Subnets to shield servers from direct internet exposure.
- Utilization of NAT Gateway for instances in private subnets to access the internet.
- Redundant NAT Gateway deployment across both Availability Zones for increased resilience.

## Services Used

- Amazon VPC: To create a logically isolated network environment.
- NAT Gateway: To allow private instances to access the internet while remaining secure.
- Routing Table: To define traffic routes within the VPC.
- Public and Private Subnets: To segregate and manage network traffic.
- Target Groups: For routing requests from the load balancer to instances.
- Application Load Balancer: To efficiently distribute incoming traffic.
- Launch Template: For specifying configurations when launching instances.
- Auto Scaling Group: To automatically scale the number of instances based on demand.
- Bastion Instance: To securely access private instances using SSH.

## Creating the Project

Follow these steps to create the VPC deployment with Auto Scaling and Load Balancing:

1. **VPC Creation:**
   - Log in to the AWS Console.
   - Navigate to VPC and create a new VPC with public and private subnets across two Availability Zones.
   
2. **Auto Scaling Group:**
   - Create an Auto Scaling group with a launch template to launch instances in private subnets.
   
3. **Bastion Host:**
   - Create a bastion host instance in a public subnet to securely access private instances.
   
4. **Connect Private Instances:**
   - Use the bastion host to connect to private instances for configuration.
   
5. **Application Load Balancer:**
   - Create an Application Load Balancer and associate it with the private instances.
   
6. **Testing:**
   - Access the load balancer's URL to test the project. Traffic will be distributed across instances.

## Acknowledgments

This project is a demonstration of best practices for deploying production-ready server infrastructure using AWS services. It aims to provide a resilient and scalable environment for hosting applications and services.

For more details and the complete source code, visit the [GitHub Repository]([https://github.com/YourUsername/YourRepository](https://github.com/Isaac58222/aws/edit/main/vpc_project)).

---

By Isaac D, created with the assistance of ChatGPT.

