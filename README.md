# Google Cloud Platform (GCP) VM Deployment & SSH Configuration

This repository contains a comprehensive guide and technical documentation for setting up a virtual infrastructure on Google Cloud Platform.

## 🚀 Project Overview
In this project, I have successfully deployed a Virtual Machine (VM) on GCP and configured secure remote access using SSH Key Pairs. This laboratory work demonstrates cloud infrastructure management, security best practices, and terminal-based server operations.

## 🛠 Tech Stack & Tools
* **Provider:** Google Cloud Platform (GCP)
* **Service:** Compute Engine (VM Instances)
* **OS:** Debian/Linux
* **Security:** SSH Key Pair (RSA 2048-bit)
* **Terminal:** Git Bash for Windows

## 📋 Step-by-Step Implementation

### 1. Account & Billing Setup
* Activated GCP Free Tier with $300 credit.
* Configured Billing Account and linked to the project.

### 2. Compute Engine API Activation
* Enabled the Google Compute Engine API to manage virtual machine resources.

### 3. SSH Key Generation
* Generated a secure SSH key pair using Git Bash:
  `ssh-keygen -t rsa -f ~/.ssh/google_cloud_key -C "user.name" -b 2048`

### 4. VM Configuration
* **Region:** europe-west3 (Frankfurt)
* **Machine Type:** e2-medium
* **Security:** Injected Public Key into VM Metadata.

### 5. Remote Connection
* Established a secure connection via terminal:
  `ssh -i [PATH_TO_KEY] [USER]@[EXTERNAL_IP]`
  
---
**Medium Article:** [(https://medium.com/@kumrueylem2/google-cloud-gcp-rehberi-%C3%BCcretsiz-hesap-olu%C5%9Fturma-vm-kurulumu-ve-ssh-key-yap%C4%B1land%C4%B1rmas%C4%B1-0a4f09dce3fe)]
