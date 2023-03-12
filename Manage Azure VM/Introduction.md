# Manage Azure VM

Microsoft Azure is a powerful cloud computing platform that provides a variety of services to help organizations build, deploy, and manage applications and services. One of the most important skills for anyone working with Azure is the ability to use PowerShell and CLI commands to manage Azure resources.

In this article, we will provide an overview of PowerShell and CLI in Azure Cloud Services and discuss how to use these tools to manage Azure resources effectively. This article is aimed at individuals studying for the AZ-104 exam and looking to improve their understanding of PowerShell and CLI in Azure Cloud Services.

## What is PowerShell?

PowerShell is a powerful command-line tool developed by Microsoft that allows users to automate tasks and manage configurations in Windows and Azure environments. PowerShell provides a rich set of cmdlets that can be used to perform a wide variety of tasks in Azure, including managing Azure resources, configuring virtual machines, and deploying applications.

PowerShell cmdlets are grouped into modules, and each module provides a set of related cmdlets. For example, the Azure PowerShell module includes cmdlets for managing Azure resources such as virtual machines, storage accounts, and network interfaces.

## Using PowerShell in Azure:

To use PowerShell in Azure, you need to install the Azure PowerShell module on your local machine. You can do this by running the following command in PowerShell:

```
Install-Module -Name Az -AllowClobber
```
Once the Azure PowerShell module is installed, you can connect to your Azure account using the following command:

```
Connect-AzAccount
```
This command will prompt you to enter your Azure credentials, after which you will be connected to your Azure account.

Once you are connected, you can use PowerShell cmdlets to manage your Azure resources. For example, the following command lists all the virtual machines in your Azure subscription:

```
Get-AzVM
```
You can also use PowerShell to create and configure Azure resources. For example, the following command creates a new virtual machine:

```
New-AzVM -ResourceGroupName myResourceGroup -Name myVM -ImageName Win2016Datacenter -Credential (Get-Credential) -Location "East US"
```
In this example, the command creates a new virtual machine named "myVM" in the "myResourceGroup" resource group, using the Windows Server 2016 Datacenter image.

## What is CLI?

Azure CLI is another powerful command-line tool developed by Microsoft that allows users to manage Azure resources from the command line. CLI provides a set of commands that can be used to manage Azure resources, including creating and deleting resources, updating configurations, and managing access control.

## Using CLI in Azure:

To use CLI in Azure, you need to install the Azure CLI on your local machine. You can do this by downloading and installing the CLI package for your operating system from the Azure CLI website.

Once the CLI is installed, you can connect to your Azure account using the following command:

```
az login
```
This command will prompt you to enter your Azure credentials, after which you will be connected to your Azure account.

Once you are connected, you can use CLI commands to manage your Azure resources. For example, the following command lists all the virtual machines in your Azure subscription:

```
az vm list
```

You can also use CLI to create and configure Azure resources. For example, the following command creates a new virtual machine:

```
az vm create --resource-group myResourceGroup --name myVM --image Win2016Datacenter --admin-username azureuser --admin-password <yourpassword>
```

In this example, the command creates a new virtual machine named "myVM" in the "myResourceGroup" resource group, using the Windows Server 2016 Datacenter image. It also specifies an administrator username and password for the virtual machine.

## PowerShell vs CLI:

Both PowerShell and CLI can be used to manage Azure resources effectively. However, there are some differences between these tools that may make one more suitable than the other depending on the task at hand.

PowerShell is a more powerful and versatile tool than CLI, with a larger set of cmdlets and more advanced scripting capabilities. PowerShell is well-suited for complex tasks that require detailed configuration and customization, such as deploying complex applications or configuring complex network topologies.

CLI, on the other hand, is a simpler tool that provides a more streamlined and intuitive command-line interface. CLI is well-suited for simple tasks that require quick and easy configuration, such as creating and deleting resources or updating simple configurations.

# Conclusion:

PowerShell and CLI are powerful command-line tools that can be used to manage Azure resources effectively. These tools provide a rich set of commands and capabilities that can be used to automate tasks, manage configurations, and deploy applications in Azure.

For individuals studying for the AZ-104 exam, it is important to have a good understanding of PowerShell and CLI in Azure Cloud Services. By mastering these tools, you can become a more effective and efficient Azure administrator, and achieve success in your career in the cloud computing industry.





