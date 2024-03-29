<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://cctechconsulting.com/">
    <img src="images/CC_Logo.png" alt="CC Tech Consulting" width="180" height="80">
  </a>
  <a href="https://bitnami.com/stack/odoo/cloud/aws/amis">
    <img src="images/Bitnami.png" alt="Bitnami by VMWare" width="180" height="80">
  </a>
  <h3 align="center">Odoo-17 Deployment:</h3>

  <p align="center">
    Comprehensive guide for deploying Odoo 17 on AWS EC2 using the Bitnami AMI!
    <br />
    <a href="https://docs.bitnami.com/aws/"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://bitnami.com/stack/odoo/cloud/aws">DEPLOYMENT OFFERING</a>
    ·
    <a href="https://github.com/bitnami/vms">Report Bug</a>
    ·
    <a href="https://docs.bitnami.com/aws/faq/">AWS FAQ</a>
  </p>
  </div>
  
# Product Overview

Odoo is an open source Enterprise Resource Planning (ERP) and Customer Relationship Management (CRM) platform that can consolidate a variety of business operations, from supply chain and project management to accounting and HR, into one system. It is supported by a community of over 20,000 contributors.

If you’re new to the cloud, the easiest way to get started with Amazon Web Services is with Bitnami. Bitnami provides pre-packaged application images for AWS Cloud servers, so that you can get productive with your new server immediately. You can access and launch these images in three ways:

Through the [AWS Marketplace](https://aws.amazon.com/marketplace), Amazon’s online application library;

Through the [AWS Console](https://console.aws.amazon.com/), Amazon’s online dashboard for AWS users;

Through [Amazon Lightsail](https://amazonlightsail.com/), Amazon’s virtual private servers.

In this tutorial, I’ll walk you, step by step, through the process of using the AWS Console to create and provision a new AWS cloud server. And since AWS offers a Free Tier valid for 12 months, you’ll have plenty of time to experiment with your server and Bitnami images without worrying about being billed for usage.

## Getting Started

1. Sign in to your [AWS account](https://console.aws.amazon.com/console/home)

2. Go to your AWS Management Console

3. Search for EC2 landing page

4. Click on Launch instance

5. Name your Virtual Server (something like "Odoo Server")

6. On Application and OS Images (Amazon Machine Image) section search for Odoo 17

<img src="images/Searching_AMI.png" alt="Search for Odoo 17" width="600" height="500">

7. Look for and Click on the Community AMIs result

8. You can choose from the list and click Select. (I used the up [Bitnami package for Odoo 17.0.20240305-1](https://bitnami.com/stack/odoo/cloud/aws))

9. Choose Instance Type "t3a.small"

10. Create a Key pair or use your existing one if you prefer. 

11. By default the AMI creates a new security group called 'Bitnami package for Odoo-15.0.20240310-0 on Debian 12-AutogenByAWSMP--1' with the following rules:
<img src="images/SG.png" alt="Security Group" width="600" height="100">

12. Confirm your selection by hitting the “Launch Instances” button.

### Prerequisites

Requirements for the software and other tools to build, test and push 
- [Example 1](https://www.example.com)
- [Example 2](https://www.example.com)

### Installing

Open your terminal or command prompt and use the following SSH command to connect to your Odoo instance:

Say what the step will be

    ssh -i /path/to/your/private-key.pem ec2-user@your-instance-public-ip

Replace /path/to/your/private-key.pem with the path to your private key file (.pem) associated with the instance. Replace ec2-user with the appropriate username based on the AMI (Amazon Machine Image) used for your instance (e.g., bitnami, ubuntu, admin, etc.). Replace your-instance-public-ip with the public IP address or hostname of your AWS instance.

//////////////////////////////////////////////////////////////////////////////

<img src="images/SSH.png" alt="Connecting using SSH" width="600" height="400">

//////////////////////////////////////////////////////////////////////////////

List directories 

    ls

Open editor to copy bitnami_credentials 

    nano bitnami_credentials
    
<img src="images/Odoo_Login.png" alt="Logging page" width="200" height="300">