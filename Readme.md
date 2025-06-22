☁️ Cloud Resume Challenge – Lite Edition
This project is my personal execution of the Cloud Resume Challenge — adapted and streamlined to prove my real-world cloud, Git, and infrastructure skills using Terraform, AWS S3, CloudFront, and GitHub Pages.

It’s a public-facing resume powered by the cloud, built with Infrastructure as Code, and served through a global CDN.

🧠 What I Proved
✅ Skill	💬 Description
AWS Cloud Infrastructure	Provisioned S3 bucket, static website hosting, and optionally CloudFront CDN.
Infrastructure as Code	Used Terraform to define and automate every piece of infrastructure.
Git + GitHub	Code versioned and deployed via GitHub.
Linux CLI + Bash	Deployed and managed infrastructure via CLI and shell scripting.
Cloud Fundamentals	Understood IAM, S3 policy, bucket configs, and public access safely.

🚀 Live Demo (optional)
📄 View Resume

(Replace this with your deployed website link — S3/CloudFront/GitHub Pages)

🧱 Project Architecture
text
Copy
Edit
Browser → CloudFront CDN → S3 Bucket (Static Website)
                    ↑
          Terraform deploys & manages all
📁 File Structure
bash
Copy
Edit
Cloud-Resume-Challenge-lite/
│
├── website/           # HTML/CSS/JS files for resume
├── terraform/         # Terraform IaC configs
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── provider.tf
├── scripts/           # Bash deployment scripts (optional)
│   └── deploy.sh
└── README.md          # This file
🔧 Tech Stack
Terraform – Infrastructure as Code

AWS S3 – Static website hosting

CloudFront – CDN for performance (optional)

GitHub – Source control and version history

Bash – CLI automation

💻 How to Deploy
🧰 Prerequisites
AWS CLI (aws configure)

Terraform (terraform -v)

Git

⚙️ Deployment Steps
bash
Copy
Edit
cd terraform
terraform init
terraform plan
terraform apply
bash
Copy
Edit
# Optional: sync your site files to S3 if not done via Terraform
aws s3 sync ../website/ s3://your-bucket-name --delete
🔐 Security Considerations
S3 bucket is set for public read access, but only to static files (no write/delete).

IAM permissions follow least privilege.

🧼 Teardown
bash
Copy
Edit
terraform destroy
👔 About Me
Charles Bucher (Tommy813)
💼 Career-changer | Future Cloud Engineer
📫 GitHub

This project was built to prove I can break into cloud — no excuses, no shortcuts.

