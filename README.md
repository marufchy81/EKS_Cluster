# 🚀 Terraform EKS Two-Tier Application Deployment

Hi, I’m **Maruf Chowdhury** 👋  
This project is a practical implementation of a **two-tier web application** deployed on **AWS EKS**, fully provisioned using **Terraform**. It covers **VPC setup**, **EKS cluster creation**, **load balancing**, and **application deployment** — all done through infrastructure-as-code.

## 🧱 Project Highlights

- **Infrastructure as Code (IaC)** using Terraform
- **Amazon EKS (Elastic Kubernetes Service)** for managing Kubernetes
- **ALB/ELB** for load balancing
- **Private and public subnets** across availability zones
- **Two-tier architecture**: frontend + backend apps running on Kubernetes
- **Auto scaling**, **security groups**, **IAM roles**, and best practices included

## 🛠️ Tools & Tech Stack

- **Terraform** (v1.x)
- **AWS** (VPC, EKS, IAM, ALB)
- **Kubernetes**
- **Docker** (for containerizing app)
- **Helm** *(optional, for future extension)*

## 📂 Folder Structure

```
.
├── modules/
│   ├── vpc/
│   ├── eks/
│   └── alb/
├── environments/
│   └── dev/
│       ├── main.tf
│       ├── variables.tf
│       └── outputs.tf
├── app/
│   ├── frontend/
│   └── backend/
├── terraform.tfvars
├── providers.tf
└── README.md
```

## 🚦 How to Use

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/terraform-eks-two-tier-app.git
   cd terraform-eks-two-tier-app
   ```

2. **Initialize Terraform**
   ```bash
   terraform init
   ```

3. **Preview the infrastructure**
   ```bash
   terraform plan
   ```

4. **Apply and deploy**
   ```bash
   terraform apply
   ```

5. **Deploy apps to EKS**
   - Use `kubectl apply` or Helm to deploy the frontend/backend pods
   - Expose services via LoadBalancer or Ingress

## 📸 Diagram (Optional)

> If you want, you can include a simple architecture diagram here showing:
> - VPC with subnets
> - EKS cluster
> - ALB in front
> - Two-tier application

## 📌 Notes

- Designed to be **production-ready**
- You can extend it to support **RDS**, **Redis**, or other services
- Ideal for **DevOps learning**, **interview prep**, or **personal projects**

## 👨💻 Author

**Maruf Chowdhury**  
DevOps | Cloud | Kubernetes Enthusiast  
📫 [Email or LinkedIn Here]
