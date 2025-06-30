🚀 AWS Capstone Project – Scalable Web Application Architecture

This project was completed as part of an **18-week AWS Cloud Solutions Architect training program**. It involved designing and deploying a secure, scalable, and highly available web application infrastructure using core AWS services.

---

🧩 Architecture Overview

The infrastructure was built using the following AWS services:

- Amazon **VPC** (Virtual Private Cloud) with public and private subnets
- **EC2** instances for hosting NGINX/Apache web servers
- **Elastic Load Balancer (ALB)** for traffic distribution
- **Auto Scaling Group** for high availability
- **IAM Roles** for secure access to AWS services
- **Amazon DynamoDB** for NoSQL database needs
- **CloudWatch** and **SNS** for monitoring and alerts

---

💼 Key Design Decisions

- **CIDR Block: `10.0.0.0/16`** – Offers over 65,000 IPs, supporting future scaling and segmentation into multiple subnets.
- **Why DynamoDB?** – Chosen for its **serverless**, **fully managed**, and **highly scalable** nature compared to relational databases like MySQL. It also simplifies integration with EC2 via IAM.
- **IAM Roles over Access Keys** – IAM roles were used for secure, temporary access to DynamoDB, reducing security risks.
- **Application Load Balancer** – Enables smart routing and built-in health checks for better reliability than classic ELBs.
- **Stress Testing** – Used to simulate CPU usage and trigger auto-scaling for testing CloudWatch alerts.

---

📊 Monitoring and Optimization

- Configured **CloudWatch Alarms** for EC2 CPUUtilization.
- Integrated **SNS** to send real-time email notifications.
- Performed **stress testing** to simulate production load.

---

🛡️ Security

- **Security Groups** defined per service to restrict access.
- **NACLs** configured at subnet level for layered security.
- Adopted **principle of least privilege** throughout.

---

⚙️ Areas for Improvement

- Deploying **multiple NAT Gateways** for better fault tolerance.
- Refining **NACL rules** to avoid unnecessary traffic blocks.
- Using **CloudFormation** or **Terraform** for infrastructure as code (IaC).
- Expanding monitoring beyond CPU (e.g., memory, I/O, logs).

---

📁 Files in This Repo

- `Project_Report.pdf` – Detailed walkthrough of the project
- `Presentation.pdf` – Visual summary with screenshots
- `README.md` – Project summary and key design highlights

---

🔗 Let’s Connect!
- [LinkedIn](https://www.linkedin.com/in/gkmensah)
- [X (Formerly Twitter)](https://twitter.com/gkmensah_)


This is just Phase One of the journey. More to come!  
#AWS #CloudComputing #DevOps #WomenInTech #CloudArchitect 
