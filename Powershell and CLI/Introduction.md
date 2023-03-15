# Powershell and CLI

Microsoft Azure is one of the most widely used cloud computing platforms in the world, with a huge number of users and organizations leveraging its powerful capabilities to host their infrastructure and applications. The Azure platform provides a wide range of tools and technologies that enable users to easily manage and automate their Azure resources. One such tool is PowerShell, a command-line interface (CLI) that allows you to automate and manage Azure resources.

## What is PowerShell and CLI?
PowerShell is a command-line interface (CLI) that is used to automate and manage Azure resources. It is a cross-platform tool that is used to automate administrative tasks in Windows and Azure. PowerShell is built on top of the .NET Framework, and it provides access to a wide range of .NET classes and APIs. PowerShell is a powerful tool for managing Azure resources, and it is widely used by Azure administrators and developers.

CLI is a cross-platform command-line interface that can be used to manage Azure resources from any operating system. It is built on top of the Azure REST API, and it provides a simplified way to manage Azure resources. CLI is written in Python, and it is available for Windows, Linux, and macOS. CLI is a lightweight tool that is perfect for managing Azure resources from the command line.

## Why use PowerShell and CLI for Azure?
PowerShell and CLI are powerful tools for managing and automating Azure resources. They provide a way to easily automate repetitive tasks, and they can be used to create scripts that can be run across multiple Azure resources. PowerShell and CLI provide a way to manage Azure resources from the command line, which is often faster and more efficient than using the Azure Portal. PowerShell and CLI can also be used to manage Azure resources programmatically, which is useful for developers who want to integrate Azure with their applications.

## How to use PowerShell and CLI for Azure
To use PowerShell and CLI for Azure, you will need to have an Azure subscription and a basic understanding of the Azure platform. You can download PowerShell and CLI from the Azure Portal or from the official Microsoft website. Once you have installed PowerShell and CLI, you can connect to your Azure subscription and start managing your Azure resources.

## AZ-104 Certification Exam and PowerShell/CLI
The AZ-104 certification exam tests your knowledge of Azure administration, and it covers a wide range of topics related to Azure. PowerShell and CLI are two of the most important tools that you will need to know for the AZ-104 exam. You will need to know how to use PowerShell and CLI to manage Azure resources, and you will need to know how to write scripts that automate tasks.

The AZ-104 exam covers a wide range of topics related to Azure administration, including:

### Virtual Machines
PowerShell:

To manage Virtual Machines in Azure through PowerShell, you need to first install the Azure PowerShell module. You can do this by running the following command:
```
Install-Module -Name Az
```
Once you have installed the module, you can log in to your Azure account by running the following command:
```
Connect-AzAccount
```
To create a new Virtual Machine, you can run the following command:
```
New-AzVM -ResourceGroupName "MyResourceGroup" -Name "MyVM" -Location "EastUS" -Image "Win2016Datacenter" -Size "Standard_DS1_v2" -Credential (Get-Credential)
```
This command creates a new Virtual Machine named "MyVM" in the "MyResourceGroup" resource group, located in the "EastUS" region, using the "Win2016Datacenter" image and the "Standard_DS1_v2" size. The -Credential parameter prompts you to enter your Azure credentials.

To start a Virtual Machine, you can run the following command:
```
Start-AzVM -Name "MyVM" -ResourceGroupName "MyResourceGroup"
```
To stop a Virtual Machine, you can run the following command:
```
Stop-AzVM -Name "MyVM" -ResourceGroupName "MyResourceGroup"
```
To delete a Virtual Machine, you can run the following command:
```
Remove-AzVM -Name "MyVM" -ResourceGroupName "MyResourceGroup"
```
Azure CLI:

To manage Virtual Machines in Azure through Azure CLI, you need to first install the CLI. You can do this by following the instructions on the Azure CLI documentation.

Once you have installed the CLI, you can log in to your Azure account by running the following command:
```
az login
```
To create a new Virtual Machine, you can run the following command:
```
az vm create --resource-group MyResourceGroup --name MyVM --image Win2016Datacenter --size Standard_DS1_v2 --admin-username azureuser --admin-password MyPa$$word123
```
This command creates a new Virtual Machine named "MyVM" in the "MyResourceGroup" resource group, using the "Win2016Datacenter" image and the "Standard_DS1_v2" size. The --admin-username and --admin-password parameters specify the credentials for the administrator account.

To start a Virtual Machine, you can run the following command:
```
az vm start --name MyVM --resource-group MyResourceGroup
```
To stop a Virtual Machine, you can run the following command:
```
az vm stop --name MyVM --resource-group MyResourceGroup
```
To delete a Virtual Machine, you can run the following command:
```
az vm delete --name MyVM --resource-group MyResourceGroup
```
### Storage Accounts
Managing Azure Storage accounts through Powershell
Creating a new Storage account
```
# Set variables for the new Storage account
$resourceGroupName = "myResourceGroup"
$location = "eastus"
$accountName = "mystorageaccount"
$skuName = "Standard_RAGRS"
$kind = "StorageV2"
$accessTier = "Hot"

# Create the new Storage account
New-AzStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName -Location $location -SkuName $skuName -Kind $kind -AccessTier $accessTier
```
Retrieving information about a Storage account

```
# Set variables for the Storage account
$resourceGroupName = "myResourceGroup"
$accountName = "mystorageaccount"

# Get information about the Storage account
Get-AzStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName
```
Updating a Storage account

```
# Set variables for the Storage account
$resourceGroupName = "myResourceGroup"
$accountName = "mystorageaccount"

# Update the Storage account to enable logging
Set-AzStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName -EnableLogging $true
```
Deleting a Storage account

```
# Set variables for the Storage account
$resourceGroupName = "myResourceGroup"
$accountName = "mystorageaccount"

# Delete the Storage account
Remove-AzStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName -Force
```
Managing Azure Storage accounts through Azure CLI
Creating a new Storage account

```
# Set variables for the new Storage account
resourceGroupName="myResourceGroup"
location="eastus"
accountName="mystorageaccount"
skuName="Standard_RAGRS"
kind="StorageV2"
accessTier="Hot"

# Create the new Storage account
az storage account create --resource-group $resourceGroupName --name $accountName --location $location --sku $skuName --kind $kind --access-tier $accessTier
```
Retrieving information about a Storage account

```
# Set variables for the Storage account
resourceGroupName="myResourceGroup"
accountName="mystorageaccount"

# Get information about the Storage account
az storage account show --resource-group $resourceGroupName --name $accountName
```
Updating a Storage account

```
# Set variables for the Storage account
resourceGroupName="myResourceGroup"
accountName="mystorageaccount"

# Update the Storage account to enable logging
az storage account update --resource-group $resourceGroupName --name $accountName --set "properties.logging.delete.retentionPolicy.enabled=true"
```
Deleting a Storage account

```
# Set variables for the Storage account
resourceGroupName="myResourceGroup"
accountName="mystorageaccount"

# Delete the Storage account
az storage account delete --resource-group $resourceGroupName --name $accountName --yes
```

### Virtual Networks
Creating a virtual network using Powershell:
```
New-AzVirtualNetwork -ResourceGroupName "myResourceGroup" -Name "myVnet" -AddressPrefix "10.0.0.0/16"
```
Creating a virtual network using the Azure CLI:

```
az network vnet create --name myVnet --resource-group myResourceGroup --address-prefixes 10.0.0.0/16
```
Adding a subnet to a virtual network using Powershell:

```
Add-AzVirtualNetworkSubnetConfig -Name "mySubnet" -VirtualNetwork (Get-AzVirtualNetwork -Name "myVnet" -ResourceGroupName "myResourceGroup") -AddressPrefix "10.0.1.0/24"
```
Adding a subnet to a virtual network using the Azure CLI:

```
az network vnet subnet create --name mySubnet --resource-group myResourceGroup --vnet-name myVnet --address-prefixes 10.0.1.0/24
```
Creating a network security group using Powershell:

```
New-AzNetworkSecurityGroup -Name "myNSG" -ResourceGroupName "myResourceGroup"
```
Creating a network security group using the Azure CLI:

```
az network nsg create --name myNSG --resource-group myResourceGroup

```
Assigning a network security group to a subnet using Powershell:

```
Set-AzVirtualNetworkSubnetConfig -VirtualNetwork (Get-AzVirtualNetwork -Name "myVnet" -ResourceGroupName "myResourceGroup") -Name "mySubnet" -AddressPrefix "10.0.1.0/24" -NetworkSecurityGroup (Get-AzNetworkSecurityGroup -Name "myNSG" -ResourceGroupName "myResourceGroup")
```
Assigning a network security group to a subnet using the Azure CLI:

```
az network vnet subnet update --name mySubnet --resource-group myResourceGroup --vnet-name myVnet --network-security-group myNSG

```


### Azure Active Directory
Create a new user in Azure Active Directory through PowerShell:
```
New-AzureADUser -AccountEnabled $true -DisplayName "John Smith" -GivenName "John" -Surname "Smith" -UserPrincipalName "john.smith@contoso.com" -PasswordProfile (New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile -Property @{Password="P@ssw0rd1";ForceChangePasswordNextLogin=$false})
```
List all users in Azure Active Directory through PowerShell:
```
Get-AzureADUser
```
Create a new group in Azure Active Directory through CLI:
```
az ad group create --display-name "Engineering Team" --mail-nickname "engteam" --description "This group contains all members of the Engineering team."
```
Add a user to an Azure Active Directory group through CLI:
```
az ad group member add --group "Engineering Team" --member-id "john.smith@contoso.com"
```



### Azure Security Center
Enable Azure Security Center on a subscription:
```
Connect-AzAccount
Set-AzSubscription -SubscriptionId <subscriptionId>
Set-AzSecurityCenterSubscription -SubscriptionId <subscriptionId> -Tier Standard
```
Get Azure Security Center Recommendations:
```
Connect-AzAccount
$recommendations = Get-AzSecurityRecommendation -ResourceId <resourceId>
foreach ($rec in $recommendations) {
    Write-Host $rec.recommendation.displayname
    Write-Host $rec.recommendation.description
}
```
Get Azure Security Center Alerts:
```
Connect-AzAccount
$alerts = Get-AzSecurityAlert -ResourceId <resourceId>
foreach ($alert in $alerts) {
    Write-Host $alert.Title
    Write-Host $alert.Description
}
```
CLI Examples:
Enable Azure Security Center on a subscription:
```
az account set --subscription <subscriptionId>
az security pricing create --name default --tier 'Standard'
```
Get Azure Security Center Recommendations:
```
az security recommendation list --resource <resourceId>
```
Get Azure Security Center Alerts:
```
az security alert list --resource <resourceId>
```
### Azure Monitor
TODO: Add examples of managing through Powershell and CLI

### Azure Automation
TODO: Add examples of managing through Powershell and CLI

You will need to know how to use PowerShell and CLI to manage all of these Azure resources. You will need to know how to create and manage virtual machines, storage accounts, virtual networks, and Azure Active Directory. You will also need to know how to use PowerShell and CLI to monitor and automate your Azure resources.

# Conclusion
PowerShell and CLI are powerful tools for managing and automating Azure resources. They provide a way to easily automate repetitive tasks, and they can be used to create scripts that can be run across multiple Azure resources. PowerShell and CLI provide a way to manage Azure resources from the command line, which is often faster and more efficient than using the Azure Portal. PowerShell and CLI are also important tools for the AZ-104 certification exam, and you will need to know how to use them to manage Azure resources