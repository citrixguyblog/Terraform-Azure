# Terraform-Azure
This repository will contain Terraform code for Azure -  snippets, useful bits, samples, labs and more.

## About the code in this Repository

Due to the fact that some of the Terraform Projects in this Repository are unlikely to be used alone, the samples provided may also contain supporting elements. So in some cases, items like Resource Groups, VNETs, Subnets and more are deployed to support whatever is being demonstrated. 
  
To utilise the code you may therefore just deploy as is and see the concept being demonstrated,  *without needing to adapt the code or rework it. * You can then take any elements you require and work them into your code, to move forward from there. 

## How to Deploy
 
For all of the Projects the following files are provided:

- azuredeploy.tf
- variables.tf
- terraform.tfvars
- provider.tf

These should be placed into a directory, and then terraform initialised and applied. 

## Projects in this Repository

### 1. **Automatic NSG based on the Client IP of the Machine running Terraform**
*This creates a data item that gets the external IP of the machine that is running Terraform. The IP is then used to create an    inbound security rule inside a Network Security Group.* **See: [Automatic-ClientIP-NSG](https://github.com/jakewalsh90/Terraform-Azure/tree/main/Automatic-ClientIP-NSG)**

### 2. **Azure KeyVault with Secret for Virtual Machine Password**
*This creates an Azure Key Vault using a random name like "keyvault##########", and then creates a password string, using the random_string resource, which is stored inside the KeyVault. This can then be used during the setup of VMs with Terraform .* **See: [Azure-KeyVault-with-Secret](https://github.com/jakewalsh90/Terraform-Azure/tree/main/Azure-KeyVault-with-Secret)**
