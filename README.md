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