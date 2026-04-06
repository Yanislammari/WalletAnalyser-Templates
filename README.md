# WalletAnalyser Templates

This repository contains the HTML email templates used across the WalletAnalyser platform.  
It centralizes all email-related assets and ensures consistent design and formatting for transactional and notification emails.

The templates are deployed via a CI/CD pipeline that automatically pushes updates to the project's Azure Blob Storage container, making them available to the backend services without manual intervention.

---

## 🚀 Project Context

WalletAnalyser is a financial portfolio management platform.  
While the backend handles API routing, data processing, and analytics, this repository focuses solely on the email communication layer.

---

## 🛠️ CI/CD & Deployment

A GitHub Actions pipeline in this repository:

1. Checks out the repository  
2. Builds or validates the email templates (HTML/CSS)  
3. Pushes the finalized templates directly to the configured Azure Blob Storage container  

This ensures that any update to email templates is automatically reflected in the platform without manual deployment.

---

## 📄 Repository Contents

- `templates/` – HTML files for transactional and notification emails  
- `README.md` – this documentation  
- CI/CD workflow files for automated deployment  

---

## 📌 Usage

Backend services can reference the email templates directly from the Azure Blob Storage container.  
No additional processing is required after deployment; the templates are ready to use.
