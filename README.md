---
page_type: sample
languages:
- terraform
- hcl
name: Introduction to using Azure Verified Modules for Terraform
description: A walk through lab demonstrating how to use the Azure Verified Modules for Terraform.
products:
- azure
urlFragment: avm-terraform-labs
---

# Introduction to using Azure Verified Modules for Terraform

This is a lab based sample that demonstrates how to use the Azure Verified Modules for Terraform. The repository contains the full working solution, but you should follow the steps in the lab to understand how it fits together.

## Content

| File/folder | Description |
|-------------|-------------|
| `labs` | The files for the lab. |
| `.gitignore` | Define what to ignore at commit time. |
| `CHANGELOG.md` | List of changes to the sample. |
| `CONTRIBUTING.md` | Guidelines for contributing to the sample. |
| `README.md` | This README file. |
| `LICENSE.md` | The license for the sample. |

## Features

This lab walks through the following steps in AVM cration
* Module proposal
* GitHub setup
* Coding steps
* AVM submission

## Getting Started

### Prerequisites

* HashiCorp Terraform CLI Version 1.7 or higher: [Download](https://www.terraform.io/downloads)
* Git: [Download](https://git-scm.com/downloads)
* Visual Studio Code: [Download](https://code.visualstudio.com/)
  * Azure Terraform Extension for Visual Studio Code: [Install](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azureterraform)
  * HashiCorp Terraform Extension for Visual Studio Code: [Install](https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform)
* Azure CLI: [Download](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-windows?tabs=azure-cli#install-or-update)
* An Azure Subscription: [Free Account](https://azure.microsoft.com/en-gb/free/search/)

### Quickstart

The instructions for this sample are in the form of a Lab. Follow along with them to get up and running.

## Demo / Lab

### Part 0 - Propose module

#### Reference
* [ID: SNFR11 - Category: Contribution/Support - Issues Response Times](https://azure.github.io/Azure-Verified-Modules/specs/shared/#id-snfr11---category-contributionsupport---issues-response-times)

Use the following fields to fill in the form

| Field | Value |
|--|--|
| Name: | [Module Proposal]: Resource Group Resource Module|
| I have checked for previous/existing GitHub issues/module proposals. | Check |
| I have checked for that this module doesn't already exist in the module indexes; or I'm proposing the module to be migrated from CARML/TFVM. | Check |
| Bicep or Terraform | Terraform |
| Module Classification | Resource Module |
| Repository Name | terraform-azurerm-avm-res-resources-resourcegroups |
| Module Details | A Terraform resource module for managing Resource Groups. |
| Do you want to be the owner of this module?   | Yes <br> See: [SNFR11 - Issues Response Times](https://azure.github.io/Azure-Verified-Modules/specs/shared/#id-snfr11---category-contributionsupport---issues-response-times) |
| Module Owner's GitHub Username (handle) | Github username |
| (Optional) Secondary Module Owner's GitHub Username (handle) | Github username <br> NOTE: By choosing to be an owner you are agreeing to AVM SLAs.  For this reason, it is recommended that you have at least secondary owner. |
| Submit new issue | DO NOT CLICK |

### Part 1 - Wait for approval

* Expect some back and forth with the AVM Team
* Don't start before you get approval

### Part 2 - Create a Repository from AVM Template

#### Reference
* [Terraform Contribution Guide | Azure Verified Modules](https://azure.github.io/Azure-Verified-Modules/contributing/terraform/#template-repository)
* [ID: SNFR11 - Category: Contribution/Support - Issues Response Times](https://azure.github.io/Azure-Verified-Modules/specs/shared/#id-snfr11---category-contributionsupport---issues-response-times)

Steps:

* Go to: [Azure/terraform-azurerm-avm-template: Template repo for Azure Verified Modules using Terraform (github.com)](https://github.com/Azure/terraform-azurerm-avm-template)
* Click “Use this template”:

![terraform-azurerm-avm-template](images/azurerm-avm-template.png)

* Fill in the following

| Field | Value |
|--|--|
| Include all branches | Uncheck |
| Owner | For the lab choose your personal org. When creating a real AVM choose “Azure” |
| Repository name | terraform-azurerm-avm-res-resources-resourcegroups <br> See: [Module Publishing](https://azure.github.io/Azure-Verified-Modules/contributing/terraform/#module-publishing) |
| Description | A Terraform resource module for managing Resource Groups. |

![Alt text](images/create-new-repository.png)

* This lab creates a repository in your organization.  When you create an AVM in the Azure repository you will need to follow the [1es](https://dev.azure.com/CSUSolEng/Azure%20Verified%20Modules/_wiki/wikis/AVM%20Internal%20Wiki/274/1es) process.  You will receive an email and will need to enter information related to our organization.


### Create Labels

#### Reference
* [ID: SNFR23 - Category: Contribution/Support - GitHub Repo Labels](https://azure.github.io/Azure-Verified-Modules/specs/shared/#id-snfr23---category-contributionsupport---github-repo-labels)


#### Steps:

* Run ```pwsh``` from a command line and enter the following
* Download [Set-AvmGitHubLabels.ps1](https://azure.github.io/Azure-Verified-Modules/scripts/Set-AvmGitHubLabels.ps1)
```

```
