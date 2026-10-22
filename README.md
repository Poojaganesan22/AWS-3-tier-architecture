# AWS 3-Tier Architecture Project

## Project Overview

This project demonstrates the design and implementation of a three-tier web application architecture using Amazon Web Services (AWS).

The architecture separates the application into three layers: the Web Tier, Application Tier, and Database Tier.

## AWS Services Used

* Amazon VPC
* Amazon EC2
* Application Load Balancer (ALB)
* Amazon RDS (MySQL)
* Security Groups
* Public and Private Subnets
* Internet Gateway
* NAT Gateway

## Architecture

### 1. Web Tier

The web tier uses an EC2 instance to host the frontend and Nginx reverse proxy.

### 2. Application Tier

The application tier uses a private EC2 instance to run the Python Flask application and process feedback requests.

### 3. Database Tier

Amazon RDS for MySQL stores feedback submitted through the application.

## Application Request Flow

User → Public Load Balancer → Web Tier → Internal Load Balancer → Application Tier → Amazon RDS

## Project Deliverables

* Working application link
* AWS architecture diagram
* Project documentation with screenshots
* SQL query output showing stored feedback records

## Security

The architecture uses private subnets and security groups to control communication between tiers.

Database credentials and other sensitive information must be stored securely and must not be committed to this repository.

## Project Status

AWS infrastructure has been configured. Application verification, project documentation, and submission deliverables are being prepared.

