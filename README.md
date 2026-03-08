# Kubernetes Deployment Automation with Ansible

Automated deployment of a Kubernetes namespace to an **AWS EKS cluster** using **Ansible**, showcasing DevOps and infrastructure-as-code skills.

---

## Project Overview

This project demonstrates how to automate Kubernetes deployments using Ansible on an AWS EKS cluster:

- Provisioned the cluster using **Terraform**  
- Configured Ansible to communicate with local and remote hosts  
- Deployed a Kubernetes namespace (`my-app`) via an Ansible playbook  
- Verified cluster connectivity and namespace creation using `kubectl`  

---

## Technology Stack

- **AWS EKS** – managed Kubernetes cluster  
- **Terraform** – infrastructure as code for cluster provisioning  
- **Ansible** – automation and orchestration  
- **kubectl** – Kubernetes CLI  
- **DigitalOcean** – optional test hosts for Ansible connectivity  

---

## Skills Gained

- Writing and running **Ansible playbooks** for Kubernetes resources  
- Managing **kubeconfig** and connecting to EKS clusters  
- Troubleshooting **private vs public API access** in EKS  
- Understanding **infrastructure as code** with Terraform and cloud networking  

---

## Challenges

- Initial connectivity issues due to **private-only EKS endpoint**  
- SSH host key verification for droplets in DigitalOcean  
- Parsing errors and YAML formatting in Ansible playbooks  

---

## Outcome

- Successfully automated the creation of a Kubernetes namespace (`my-app`)  
- Verified namespace creation in the cluster.
- Deployment of nginx app to K8. 