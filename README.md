# Terraform-AzureComplianceFlow
Automated Azure Policy assignment and remediation across multiple resource groups using Terraform.

# PolicyOrchestrator

Automated Azure Policy assignment and remediation across multiple resource groups using Terraform.  
Supports parameterized policies with array inputs for scalable compliance enforcement.

---

## Overview

This project automates the assignment of an Azure Policy definition to multiple resource groups, passing custom parameters for each. It also creates remediation tasks to ensure existing non-compliant resources are fixed automatically.

The solution uses Terraform's `for_each` to dynamically assign policies with parameter arrays and deploy remediations at scale.

---

## Features

- Assign a parameterized Azure Policy to multiple resource groups  
- Supports multiple array parameters per policy  
- Automatically creates remediation tasks for compliance enforcement  
- Uses Terraform’s `for_each` for scalability and maintainability  
- Employs Managed Identities for remediation authorization  

---

## Prerequisites

- Terraform 1.2 or newer  
- Azure CLI or service principal with sufficient permissions  
- Existing Azure Policy Definition ID (custom or built-in)  
- Resource groups created in your Azure subscription  

---

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/PolicyOrchestrator.git
   cd PolicyOrchestrator
