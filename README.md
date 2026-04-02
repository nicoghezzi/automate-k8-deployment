# 🚀 Kubernetes Deployment Automation: Ansible → EKS

![Orchestration: Kubernetes](https://img.shields.io/badge/Kubernetes-%23326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Automation: Ansible](https://img.shields.io/badge/Ansible-%23EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![Infrastructure: Terraform](https://img.shields.io/badge/Terraform-%235835CC?style=for-the-badge&logo=terraform&logoColor=white)
![Cloud: AWS](https://img.shields.io/badge/AWS-%23FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![CLI: kubectl](https://img.shields.io/badge/kubectl-%23326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

Automated Kubernetes deployments on Amazon EKS using Ansible, demonstrating infrastructure-as-code and cloud-native automation workflows.

---

## 📌 Overview

This project showcases an end-to-end Kubernetes automation setup:

- Provisioned an EKS cluster using Terraform  
- Configured Ansible for local and remote execution  
- Deployed a Kubernetes namespace (`my-app`) via playbooks  
- Verified cluster connectivity and deployment using `kubectl`  
- Deployed an NGINX application to the cluster  

---

## ⚙️ Workflow

### 1. Infrastructure Provisioning
- Created EKS cluster using Terraform  
- Configured networking and cluster access  

### 2. Ansible Configuration
- Set up inventory for local and remote hosts  
- Enabled Ansible to interact with Kubernetes cluster  

### 3. Kubernetes Deployment
- Executed Ansible playbook to create namespace (`my-app`)  
- Applied Kubernetes resources to cluster  

### 4. Validation
- Verified namespace creation using `kubectl`  
- Confirmed application deployment (NGINX)  

---

## 🧰 Tech Stack

- AWS EKS (Managed Kubernetes)  
- Terraform (Infrastructure as Code)  
- Ansible (Automation & Orchestration)  
- kubectl (Kubernetes CLI)  
- DigitalOcean (Optional test hosts)  

---

## 💡 Key Skills Demonstrated

- Writing Ansible playbooks for Kubernetes resources  
- Managing kubeconfig and EKS cluster access  
- Automating Kubernetes deployments  
- Understanding cloud networking and API access patterns  
- Integrating Terraform and Ansible workflows  

---

## ⚠️ Challenges & Fixes

- **EKS connectivity issues** → Resolved private vs public API endpoint access  
- **SSH host key verification** → Managed known_hosts for remote connections  
- **YAML parsing errors** → Fixed formatting issues in Ansible playbooks  

---

## ✅ Outcome

- ✔ Automated creation of Kubernetes namespace (`my-app`)  
- ✔ Verified deployment directly in EKS cluster  
- ✔ Successfully deployed NGINX application  
- ✔ Established repeatable Kubernetes deployment workflow  

---

## 🧪 Takeaway

This project demonstrates how to automate Kubernetes deployments using Ansible on top of Terraform-provisioned infrastructure. It highlights real-world challenges in cluster connectivity, configuration management, and YAML-based automation—while reinforcing best practices for reliable cloud-native deployments.

## Steps

Step 1: Create Kubernetes Cluster using Terraform
![Lighthouse Report](/images/1_terraformapply.png)

Step 2: Review EC2 instance
![Lighthouse Report](/images/2_creationofEC2instance.png)

Step 3: Verification of Cluster in AWS Console
![Lighthouse Report](/images/3_verificationofcluster.png)

Step 4: Create a K8 Namespace
![Lighthouse Report](/images/4_createnamespace.png)

Step 5: Check Cluster over Terminal
![Lighthouse Report](/images/5_checkcluster.png)

Step 6: Check K8 Namespace over Terminal
![Lighthouse Report](/images/6_kubectlgetnamespaces.png)

Step 7: Execute Playbook to deploy nginx application
![Lighthouse Report](/images/7_playbookfornginx.png)

Step 8: Check K8 pod
![Lighthouse Report](/images/8_checkdeploymenttoK8.png)

Step 9: Check Service
![Lighthouse Report](/images/9_checkK8-service.png)

Step 10: Access Nginx App via browser.
![Lighthouse Report](/images/10_accessnginxappviabrowser.png)