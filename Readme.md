
---

🚀 Cloud Resume Challenge Lite

Project Overview

This project is a streamlined version of the popular Cloud Resume Challenge, demonstrating the deployment of a personal static website (resume) hosted on AWS S3 with CloudFront, backed by automated infrastructure provisioning using AWS CLI and Bash scripting.


---

Why This Matters

Showcases core cloud skills employers crave: infrastructure as code, AWS services (S3, CloudFront), automation, and web hosting — all essential for junior cloud and infra roles.


---

Architecture Diagram

+------------+       +-----------+       +--------------+
|   User     | ----> | CloudFront| ----> |     S3       |
+------------+       +-----------+       +--------------+

CloudFront distributes the static site globally with low latency

S3 stores the website content securely



---

How It Works

AWS CLI and Bash scripts automate the setup of the S3 bucket and CloudFront distribution

The static site files (HTML, CSS, JS) are uploaded to the S3 bucket

CloudFront CDN caches and serves the site worldwide



---

Project Structure

Cloud-Resume-Challenge-lite/
├── deploy.sh           # Bash script to provision infra and deploy site  
├── website/            # Static website files (HTML, CSS, images)  
├── README.md           # This documentation  
└── docs/
    ├── architecture.png # Diagram  
    └── screenshots/     # AWS Console & site screenshots


---

Prerequisites

AWS CLI installed and configured

Basic Bash scripting knowledge

AWS account with permissions to create S3 buckets and CloudFront distributions



---

Setup & Deployment

1. Configure AWS CLI with your credentials


2. Run the deployment script:

./deploy.sh


3. Access the website URL provided by CloudFront after deployment




---

Example Output

Creating S3 bucket: your-bucket-name
Uploading website files
Creating CloudFront distribution
Deployment complete! Access your site at: https://xxxxxxxx.cloudfront.net


---

Screenshots

AWS S3 bucket contents

CloudFront distribution settings

Live site screenshot


(See /docs/screenshots/)


---

Real-World Use Cases

Hosting personal portfolios or resumes

Deploying static websites with global reach

Demonstrating cloud infrastructure skills to employers



---

Next Steps

Add custom domain with Route 53

Implement HTTPS using AWS Certificate Manager

Automate with Terraform or CloudFormation for Infrastructure as Code



---

Author

Charles Bucher
Junior Cloud Engineer | GitHub: Tommy813-lab


---

License

MIT License


---
