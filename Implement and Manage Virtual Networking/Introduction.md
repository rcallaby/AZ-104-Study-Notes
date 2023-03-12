# Implement and Manage Virtual Networking

Azure Virtual Networking is a service that enables you to create and manage virtual networks in Azure. In this article, we will discuss how to implement and manage virtual networking in Azure Cloud services as you would find in the AZ-104 exam.

## What is Virtual Networking in Azure?

Virtual networking in Azure is a network service that enables you to create and manage virtual networks in Azure. A virtual network is a logically isolated network that you can create in Azure and use to deploy your resources. You can create multiple virtual networks in Azure and use them to connect your resources, such as virtual machines, web applications, and databases.

## Implementing Virtual Networking in Azure

To implement virtual networking in Azure, you need to perform the following steps:

### Create a virtual network
To create a virtual network, you need to go to the Azure portal and select the "Create a resource" button. Then, search for "Virtual network" and select it. You need to provide the following information to create a virtual network:

Name: A unique name for your virtual network.
Address space: The IP address range for your virtual network.
Subnet: The IP address range for your subnet.
Resource group: The resource group where your virtual network will be created.
Location: The Azure region where your virtual network will be created.
Create a subnet
After creating a virtual network, you need to create a subnet. A subnet is a range of IP addresses in your virtual network. To create a subnet, you need to go to the virtual network that you created and select the "Subnets" option. Then, select the "Add" button and provide the following information:

Name: A unique name for your subnet.
Address range: The IP address range for your subnet.
Create a network security group
A network security group is a firewall that controls the traffic to and from your resources in Azure. To create a network security group, you need to go to the Azure portal and select the "Create a resource" button. Then, search for "Network security group" and select it. You need to provide the following information to create a network security group:

Name: A unique name for your network security group.
Resource group: The resource group where your network security group will be created.
Location: The Azure region where your network security group will be created.
After creating a network security group, you need to associate it with your virtual network.

###  Configure network security rules
To configure network security rules, you need to go to your network security group and select the "Inbound security rules" or "Outbound security rules" option. Then, select the "Add" button and provide the following information:

Name: A unique name for your network security rule.
Priority: The priority of your network security rule.
Source: The source IP address range or network for your network security rule.
Destination: The destination IP address range or network for your network security rule.
Protocol: The protocol for your network security rule, such as TCP or UDP.
Port range: The port range for your network security rule.
Managing Virtual Networking in Azure

### To manage virtual networking in Azure, you need to perform the following steps:

### Monitor your virtual network
To monitor your virtual network, you need to go to the Azure portal and select your virtual network. Then, you can view the following information:

Overview: This section provides an overview of your virtual network, including the IP address range and the number of resources connected to your virtual network.
Subnets: This section shows the subnets that are part of your virtual network.
Network interfaces: This section shows the network interfaces that are connected to your virtual network.
Manage virtual network peering
Virtual network peering is a feature that enables you to connect virtual networks in Azure. With virtual network peering, you can connect virtual networks in the same region or different regions. To manage virtual network peering, you need to perform the following steps:

Go to the Azure portal and select your virtual network.

Select the "Peerings" option and then select the "Add" button.

###  Provide the following information:

Name: A unique name for your virtual network peering.
Virtual network: The virtual network that you want to peer with.
Subscription: The subscription that the virtual network is part of.
Resource group: The resource group that the virtual network is part of.
Peering type: The type of peering that you want to create, such as "Virtual network peering" or "Global virtual network peering."
Traffic forwarding: The type of traffic forwarding that you want to allow, such as "Use remote gateway" or "Allow gateway transit."
Use virtual network gateways
A virtual network gateway is a VPN gateway that you can use to connect your on-premises network to your virtual network in Azure. With a virtual network gateway, you can establish a secure connection between your on-premises network and your virtual network in Azure. To use a virtual network gateway, you need to perform the following steps:

Go to the Azure portal and select your virtual network.

Select the "Virtual network gateways" option and then select the "Add" button.

### Provide the following information:

Name: A unique name for your virtual network gateway.
Gateway type: The type of virtual network gateway that you want to create, such as "VPN" or "ExpressRoute."
VPN type: The type of VPN that you want to use, such as "Route-based" or "Policy-based."
SKU: The SKU of your virtual network gateway, which determines the performance and features of your virtual network gateway.
After creating a virtual network gateway, you need to configure your on-premises VPN device to establish a secure connection between your on-premises network and your virtual network in Azure.

# Conclusion

In this article, we have discussed how to implement and manage virtual networking in Azure Cloud services as you would find in the AZ-104 exam. By following these steps, you can create and manage virtual networks in Azure, configure network security rules, monitor your virtual network, manage virtual network peering, and use virtual network gateways to connect your on-premises network to your virtual network in Azure. With these skills, you can effectively manage your virtual networks in Azure and ensure the security and performance of your resources.