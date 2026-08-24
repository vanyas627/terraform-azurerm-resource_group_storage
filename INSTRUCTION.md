# Azure Resource Group & Storage Account Terraform Module

This Terraform module creates an Azure Resource Group along with a Storage Account following best practices.

## Usage

Add the following snippet to your `main.tf` file to use this module from the Terraform Registry:

```hcl
module "resource_group_storage" {
  source  = "vanyas627/resource_group_storage/azurerm"
  version = "1.0.0"

  
  resource_group_name  = var.resource_group_name
  storage_account_name = var.storage_account_name
  location             = var.location
}