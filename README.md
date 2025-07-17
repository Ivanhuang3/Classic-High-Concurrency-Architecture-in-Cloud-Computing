

<img width="1122" height="635" alt="架構圖" src="https://github.com/user-attachments/assets/3c8b5775-c541-4958-8dfb-4bc44c2a4b2d" />


# ☁️ Classic Cloud High-Concurrency Architecture

This project demonstrates a **highly scalable, decoupled, and resilient cloud architecture** built with AWS native services. It supports high concurrency workloads, auto-scaling, fault tolerance, and observability across multiple availability zones.

---

## 📌 Architecture Diagram

> This architecture features:
> - Frontend acceleration using **CloudFront**, **WAF**, **Route 53**, and **ACM**
> - Public subnet EC2 instances behind **Elastic Load Balancer (ALB/NLB)**
> - Backend EC2 services running in **private subnets**, accessing databases and caches
> - **NAT Gateway** for secure outbound internet access
> - Highly available **RDS** and **ElastiCache** with cross-AZ redundancy
> - Monitoring and logging via **CloudWatch**, **Grafana**, and **CloudTrail**


---

## 🔧 Key Components

| Category           | AWS Services Used                                                               |
|--------------------|----------------------------------------------------------------------------------|
| Frontend & Routing | CloudFront, WAF, Route 53, ACM                                                  |
| Networking         | Internet Gateway, NAT Gateway, VPC, Subnets                                     |
| Compute Layer      | Amazon EC2, Auto Scaling Group, AMI                                             |
| Load Balancing     | Application Load Balancer (ALB), Network Load Balancer (NLB)                    |
| Database Layer     | Amazon RDS (Multi-AZ), Amazon ElastiCache                                       |
| Object Storage     | Amazon S3                                                                        |
| Monitoring         | Amazon CloudWatch, Grafana, AWS CloudTrail                                      |

---

## 🌟 Architecture Highlights

- ⚙️ Auto-scaling EC2 backend to support high traffic and failover  
- 🔄 Multi-AZ RDS deployment for data redundancy and disaster recovery  
- 🌐 Frontend decoupling with global content delivery (S3 + CloudFront)  
- 🔒 Security with WAF and HTTPS using ACM  
- 📊 Real-time observability with CloudWatch, Grafana, and CloudTrail

---

