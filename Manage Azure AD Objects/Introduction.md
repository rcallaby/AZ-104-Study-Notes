# Manage Azure AD Objects

Azure Active Directory (Azure AD) is a cloud-based identity and access management (IAM) service that provides users with a single sign-on (SSO) experience across various applications and services. Azure AD is an essential component of the Azure Cloud platform, providing identity management services to Azure resources and other Microsoft cloud services.

In the AZ-104 exam, managing Azure AD objects is an essential skill that candidates must master. In this article, we will explore the basics of managing Azure AD objects and how it pertains to the AZ-104 exam.

## What are Azure AD Objects?

Azure AD objects are the core building blocks of the Azure AD service. They are entities that represent various resources and elements in an Azure AD tenant, including users, groups, devices, and applications.

Users are the individual entities that require authentication and authorization to access Azure resources and services. Azure AD enables administrators to create and manage user accounts, assign roles and permissions, and enforce password policies.

Groups are collections of users that simplify management by allowing administrators to apply policies and permissions to multiple users simultaneously. Azure AD enables administrators to create and manage groups, assign membership, and define group membership rules.

Devices are physical or virtual endpoints that connect to the Azure AD service. Azure AD enables administrators to manage device registration, authentication, and compliance policies, such as conditional access.

Applications are cloud or on-premises services that rely on Azure AD for authentication and authorization. Azure AD enables administrators to manage application registration, configure single sign-on (SSO), and grant access to users and groups.

## Managing Azure AD Objects

To manage Azure AD objects, administrators can use the Azure portal, PowerShell, or the Azure AD Graph API. Here are the steps to manage Azure AD objects in the Azure portal:

+ Sign in to the Azure portal using your Azure AD credentials.
+ Navigate to the Azure AD service by clicking on the 'Azure Active Directory' option on the left-hand menu.
+ Click on the 'Users' or 'Groups' option to create, modify or delete user accounts or groups.
+ Click on the 'Devices' option to manage device registration and compliance policies.
+ Click on the 'Enterprise Applications' option to manage application registration, configure SSO, and grant access to users and groups.
+ Using PowerShell to Manage Azure AD Objects

Azure AD PowerShell module provides administrators with a command-line interface to manage Azure AD objects. Here are the steps to manage Azure AD objects using PowerShell:

+ Install the Azure AD PowerShell module using the following command: Install-Module AzureAD
+ Connect to your Azure AD tenant using the following command: Connect-AzureAD -Credential (Get-Credential)
+ Use PowerShell cmdlets to create, modify or delete Azure AD objects, such as New-AzureADUser, Set-AzureADUser, Remove-AzureADUser.
+ Using Azure AD Graph API to Manage Azure AD Objects

Azure AD Graph API is a RESTful web API that provides programmatic access to Azure AD resources. Here are the steps to manage Azure AD objects using the Azure AD Graph API:

### Register your application in Azure AD and obtain an access token.
+ Use the Azure AD Graph API to create, modify or delete Azure AD objects, such as users, groups, devices, and applications.
+ Use the Graph API Explorer to test the API calls and explore the Azure AD resource hierarchy.

# Conclusion

Managing Azure AD objects is a crucial skill for administrators working with the Azure Cloud platform. The AZ-104 exam tests candidates on their ability to manage Azure AD objects using various tools and techniques, including the Azure portal, PowerShell, and the Azure AD Graph API. By mastering the basics of managing Azure AD objects, candidates can effectively secure and manage access to Azure resources and services.