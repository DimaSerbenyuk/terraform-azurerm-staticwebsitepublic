# terraform-azurerm-staticwebsitepublic
Terraform Modules to be shared in Terraform Public Registry
version 3.0.0

```h
module "staticwebsitepublic" {
  source  = "DimaSerbenyuk/staticwebsitepublic/azurerm"
  version = "1.0.0"
  # insert the 8 required variables here
  # Resource Group
  location            = "eastus"
  resource_group_name = "myrg1"

  # Storage Account
  storage_account_name              = "staticwebsite"
  storage_account_tier              = "Standard"
  storage_account_replication_type  = "LRS"
  storage_account_kind              = "StorageV2"
  static_website_index_document     = "index.html"
  static_website_error_404_document = "error.html"
}
```