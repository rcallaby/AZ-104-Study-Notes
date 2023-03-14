# Monitor and Troubleshoot Virtual Networks

As more and more organizations are moving their workloads to the cloud, the need for virtual networks has increased significantly. A virtual network is a logical representation of a network that is built on top of a physical network infrastructure, enabling virtual machines (VMs) to communicate with each other as well as with external networks such as the internet. In this article, we will discuss managing and troubleshooting virtual networks on the Azure cloud as it pertains to the AZ-104 exam.

## Azure Virtual Networks

Azure Virtual Networks are an essential part of the Azure networking stack, providing a secure and isolated environment for VMs to communicate. A virtual network can contain one or more subnets, and each subnet can be associated with a network security group (NSG) that controls inbound and outbound traffic. Azure Virtual Networks also allow you to connect your on-premises network to the cloud using a VPN gateway, enabling you to extend your on-premises network to the cloud.

## Managing Virtual Networks

### Creating a Virtual Network

To create a virtual network in Azure, follow these steps:

Sign in to the Azure portal.
In the left-hand menu, click on "Create a resource."
Search for "Virtual network" and click on "Virtual network" from the search results.
Fill in the required fields such as the name, address space, and subnet details.
Click on "Create" to create the virtual network.
Connecting Virtual Networks

Azure Virtual Networks can be connected to each other using virtual network peering. Virtual network peering allows you to connect virtual networks in the same region or in different regions. To set up virtual network peering, follow these steps:

Sign in to the Azure portal.
Select the virtual network that you want to connect to another virtual network.
Click on "Peerings" in the left-hand menu.
Click on "Add."
Fill in the required fields such as the name, remote virtual network, and remote subnet details.
Click on "Create" to create the virtual network peering.
Managing Subnets

Subnets are logical divisions of a virtual network, and they allow you to segment your network into smaller parts. Each subnet can be associated with a network security group (NSG) that controls inbound and outbound traffic. To manage subnets in Azure, follow these steps:

Sign in to the Azure portal.
Select the virtual network that contains the subnet you want to manage.
Click on "Subnets" in the left-hand menu.
Select the subnet that you want to manage.
You can then edit the subnet details, associate an NSG, or create a service endpoint.
Managing Network Security Groups (NSGs)

Network Security Groups (NSGs) are used to control inbound and outbound traffic to subnets within a virtual network. NSGs contain security rules that define which traffic is allowed or denied. To manage NSGs in Azure, follow these steps:

Sign in to the Azure portal.
Select the virtual network that contains the NSG you want to manage.
Click on "Network security groups" in the left-hand menu.
Select the NSG that you want to manage.
You can then add or remove security rules or associate the NSG with a subnet.
Troubleshooting Virtual Networks

Azure provides various tools and features to troubleshoot virtual networks. Some of the common troubleshooting techniques are:

Azure Network Watcher: Azure Network Watcher is a monitoring and diagnostic service that provides a suite of tools for troubleshooting virtual networks. It allows you to monitor and diagnose network issues such as latency, packet loss, and connectivity problems.

Network Performance Monitor: Network Performance Monitor is a feature in Azure Network Watcher that provides network monitoring capabilities for hybrid and cloud environments. It uses network monitoring probes to assess network performance and diagnose connectivity issues.

Azure Diagnostics: Azure Diagnostics is a feature that collects diagnostic data from Azure resources, including virtual networks. It allows you to collect and analyze logs, metrics, and other diagnostic data to troubleshoot issues.

Azure Resource Health: Azure Resource Health is a feature that provides visibility into the health and availability of Azure resources, including virtual networks. It allows you to monitor the status of virtual networks and troubleshoot issues related to resource availability and health.

Azure Network Watcher Troubleshooting Tools: Azure Network Watcher includes various troubleshooting tools such as IP flow verify, packet capture, and next hop. These tools help you to identify and diagnose network issues, including connectivity problems and routing errors.

In addition to these tools, you can also use various Azure services and features to troubleshoot virtual network issues. These include:

Azure Traffic Manager: Azure Traffic Manager is a global DNS load balancer that helps you to distribute incoming traffic across multiple virtual networks or regions. It can be used to redirect traffic away from a problematic virtual network.

Azure Load Balancer: Azure Load Balancer is a Layer 4 load balancer that distributes incoming traffic across multiple VMs within a virtual network. It can be used to balance traffic across multiple VMs to improve performance and availability.

Azure VPN Gateway: Azure VPN Gateway allows you to connect your on-premises network to a virtual network using a secure VPN connection. It can be used to troubleshoot connectivity issues between your on-premises network and virtual network.

# Conclusion

Virtual networks are a critical component of Azure infrastructure and enable organizations to build scalable and secure cloud environments. Managing and troubleshooting virtual networks in Azure requires a combination of tools, features, and best practices. By leveraging the tools and features available in Azure, you can effectively manage and troubleshoot virtual networks to ensure optimal performance and availability. For those preparing for the AZ-104 exam, a strong understanding of virtual network management and troubleshooting is essential.