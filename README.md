# Microsoft-AZ900
> These are my personal notes from studying for the Microsoft Fundamentals AZ-900 exam.>

## Table of Contents

- [Cloud-Concepts](#Cloud-Concepts)
- [Core-Azure-Services](#Core-Azure-Services)

---

## Cloud-Concepts

#### Identify the benefits and considerations of using cloud services 

1. Cost effective – PAY GO model or consumption-based model 
2. Allows better cost prediction 
3. It's scalable – vertical and horizontal scaling 
4. It's elastic – automatically allocate resources upon peak periods, or removes resources during non-peak periods 
5. It's current – cloud provider manages patches, updates, etc. 
6. It's reliable – data and resources will always be available 
7. It's global – multiple datacenters in multiple regions; replication + redundancy 
8. It's secure – physical and digital security 

#### Describe terms such as high availability, scalability, elasticity, agility, Fault Tolerance, and disaster recovery 
- High availability - run as designed in a healthy state with no significant downtime (up and running for long periods of time) 
  - the goal is to minimize the effects of a single failing component 
- Scalability is the ability of a system to handle increased load; scaling allows applications to react to variable load by increasing and decreasing the number of instances of roles, queues, and other services; application services must be stateless; know upper and scaling limits, and use sharding or decomposition to go beyond those limits; ensure the application doesn't require affinity; use built-in autoscaling features when possible; ability to increase or decrease resources for any given workload 
  - Scale out = add more systems; scale up = add more resources (e.g. CPU, RAM) to the same resource 
  - Does not have to be done automatically 
- Elasticity - automatically add/remove resources based on demand; Azure Advisor and Azure Cost Management are two services that help you optimize cloud spend and elasticity; is the ability to use as much capacity as you need, scaling out as load increases, and scaling in when the extra capacity is not needed; ability to automatically or dynamically increase or decrease resources as needed; elasticity is done automatically/dynamically whereas scalability does not have to be done automatically 
- Agility – ability to rapidly change IT infrastructure (react quickly) in order to adapt to evolving needs of the business (e.g. online website that peaks during holiday hours); ability to react quickly; cloud services can allocate and deallocate as needed; on-demand services via self-service; no manual intervention when provisioning / deprovisioning services 
- Fault Tolerance – ability to remain up and running even in event of a component or service failure; redundancy is built into cloud services architecture; the type of service is said to be "tolerant of faults" 
- Disaster Recovery – the ability to recover from major incidents; non transient; wide scale features such as service disruption that affects entire region; DR includes data backup and archiving which may include manual intervention (e.g. restore DB from backup) 

#### Describe the principles of economies of scale 
- Is the ability to do things more efficiently or at a lower cost per unit when operating at a large scale 
- Cloud savings are passed to end users 
  - Ability to acquire hardware at lower cost 
  - Cloud service providers can make deals with government and utilities providers to get tax savings on lower price for power/cooling, etc. 
  - CSP's then pass these savings on to end users thereby making public cloud services cheaper 
- Concept is about the ability to do things more cheaply and more efficiently when operating at larger scale 

#### Describe the differences between Capital Expenditure (CapEx) and Operational Expenditure (OpEx) 
- CAPEX = when an organization decides to own infrastructure, it buys equipment that goes onto the balance sheet as assets (upfront cost). Because a capital investment was made, accountants categorize this transaction as CAPEX 
  - Spending money on physical infrastructure upfront 
  - Value reduces over time – servers, storage, networking, backup, technical personnel, etc. 
  - Assets are depreciated or amortized 
 
- OPEX = Cloud services are categorized as operating expenses, because of their consumption model. There is no asset to amortize. Instead, OPEX has direct impact on net profit, taxable income, and associated expenses on balance sheet 
  - Leasing software, scaling charges, billing at the user or organizational level
  - No upfront costs 
  - Pay per month / per year 
  - Spending money on services and products NOW and being charged for them NOW 

#### Describe the consumption-based model 
- Most (if not all) CSP's operate on this model 
- No upfront costs; no need to purchase and manage infrastructure; PAY GO model (pay for what you use) 
- Ability to pay for additional resources when you need them 
- Ability to stop paying for resources when you don't need them 
- CSP's provide computing as a utility – to be consumed on-demand 
- No minimums or commitments 
- Competitive pricing 
- Cancel anytime 

#### Describe Infrastructure-as-a-Service (IaaS)  
- most basic category of cloud computing services. With IaaS, you rent IT infrastructure—servers and virtual machines (VMs), storage, networks, operating systems—from a cloud provider on a pay-as-you-go basis 
- is an instant computing infrastructure, provisioned and managed over the internet 
- quickly scales up and down with demand, letting you pay only for what you use 
- Each resource is offered as a separate service component, and you only need to rent a particular one for as long as you need it 
- A cloud computing service provider, such as Azure, manages the infrastructure, while you purchase, install, configure, and manage your own software—operating systems, middleware, and applications. 

Common scenario's: 
- Test / dev 
- Migrating workloads 
- Website hosting 
- Storage, backup and recovery 
- Web apps 
- High performance applications (HPC) 
- Big data analysis 

Advantages 
- Eliminate CAPEX and reduce ongoing cost (no upfront costs) 
- Improve BC/DR 
- Innovate rapidly 
- Respond quicker to shifting business conditions 
- Focus on your core business 
- Increase stability, reliability, supportability 
- Better security 
- Get new apps faster to end users 

#### Describe Platform-as-a-Service (PaaS)  
- refers to cloud computing services that supply an on-demand environment for developing, testing, delivering, and managing software applications.  
- PaaS is designed to make it easier for developers to quickly create web or mobile apps, without worrying about setting up or managing the underlying infrastructure of servers, storage, network, and databases needed for development. 
- is a complete development and deployment environment in the cloud, with resources that enable you to deliver everything from simple cloud-based apps to sophisticated, cloud-enabled enterprise applications. You purchase the resources you need from a cloud service provider on a pay-as-you-go basis and access them over a secure Internet connection. 
- PaaS includes infrastructure—servers, storage, and networking—but also middleware, development tools, business intelligence (BI) services, database management systems, and more. PaaS is designed to support the complete web application lifecycle: building, testing, deploying, managing, and updating. 
- You manage the applications and services you develop, and the cloud service provider typically manages everything else 
- PAY GO model 
- End user responsible for application development; no upfront costs 
- Avoids expense and complexity of buying and managing software licenses 

Common scenario's: 
- Development framework 
- Analytics or Business Intelligence (BI) 
- Additional services like workflows, directory, security, and scheduling 

Advantages 
- Cut coding time 
- Add DEV capabilities without adding staff 
- Multiple platform development - mobile 
- Use of sophisticated tools 
- Support geographically distributed development teams 
- Manage application lifecycles 

#### Describe Software-as-a-Service (SaaS)  
- Software as a service is a method for delivering software applications over the Internet, on demand and typically on a subscription basis (can also be monthly/annual). With SaaS, cloud providers host and manage the software application and underlying infrastructure, and handle any maintenance, like software upgrades and security patching. Users connect to the application over the Internet, usually with a web browser on their phone, tablet, or PC. 
- allows users to connect to and use cloud-based apps over the Internet. Common examples are email, calendaring, and office tools (such as Microsoft Office 365). 
- purchase on a pay-as-you-go basis / PAY GO model 
- You rent the use of an app for your organization, and your users connect to it over the Internet, usually with a web browser. All of the underlying infrastructure, middleware, app software, and app data are located in the service provider’s data center. The service provider manages the hardware and software, and with the appropriate service agreement, will ensure the availability and the security of the app and your data as well. 
  
Common scenario's: 
- web-based email service such as Outlook, Hotmail, or Yahoo! Mail 
- sophisticated business applications such as customer relationship management (CRM), enterprise resource planning (ERP), and document management. You pay for the use of these apps by subscription or according to the level of use. 
  
Advantages: 
- Access to sophisticated applications – no upfront costs 
- Predictive cost model
- Use free client software 
- Mobilize your workforce 
- Access data application anywhere 

#### Compare and contrast the 3 difference service delivery models  
1. IaaS – requires most user management; user responsible for managing OS, data, applications, security patches, etc. 
2. PaaS – requires less user management; CSP manages the OS and the user manages the applications and data 
3. SaaS – requires least amount of management; CSP manages everything and the user manages the software 

![cloud models](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fguides%2Foperations%2Fmedia%2Fcloud-computing-comparison.png&f=1&nofb=1)

Define cloud computing 
- you only pay for what you need / pay for what you use 
- Cloud computing is when you access computing services—like servers, storage, networking, software—over the internet (“the cloud”) from a provider like Azure 
- you don't worry about how or when to upgrade to the latest technology 
- You don't have to manage scaling resources 
- Cloud computing is renting resources, like storage space or CPU cycles, on another company's computers 
- cloud provider is responsible for the physical hardware required to execute your work, and for keeping it up-to-date 
- CSP provides compute, network, storage, and analytics solutions 
- Is the delivery of computing services over the internet 

#### Describe public cloud 
- Most common type of deployment 
- are owned and operated by a third-party cloud service providers, which deliver their computing resources, like servers and storage, over the Internet. Microsoft Azure is an example of a public cloud. With a public cloud, all hardware, software, and other supporting infrastructure is owned and managed by the cloud provider.  
- You access these services and manage your account using a web browser. 
- PAY GO model – cheapest cloud model 
- Multitenant model 
- Does not require deep technical knowledge to set up and use its resources 
 
Advantages 
- High scalability / agility 
- No CAPEX 
- PAY GO (consumption-based model) 
- User not responsible for managing underlying hardware, updates, maintenance, etc 
- Minimal technical knowledge 
- Public access over the internet/browser 

#### Describe private cloud 
- cloud computing resources used exclusively by a single business or organization (self-service access) 
- A private cloud can be physically located on the company’s on-site datacenter. Some companies also pay third-party service providers to host their private cloud.  
- A private cloud is one in which the services and infrastructure are maintained on a private network. 
- User is responsible for maintenance, updates, hardware, etc. 
- Costs to maintain a private cloud are high 
- Requires more technical skills/resources/knowledge 
- Some initial CAPEX may be required 
- Limits agility 
 
Advantages 
- Ensures configurations are met for specific business cases 
- You have complete control over security – compliance, regulations, legal requirements 
- Medical data is secure 
- Government data / sites 

#### Describe hybrid cloud 
- Hybrid clouds combine public and private clouds, bound together by technology that allows data and applications to be shared between them. By allowing data and applications to move between private and public clouds, a hybrid cloud gives your business greater flexibility, more deployment options, and helps optimize your existing infrastructure, security, and compliance. 
- Example – put web app in public cloud, while DB is in private cloud 
- Specific resources run in public cloud while others used in private cloud 
- May be more expensive than selecting a single cloud model – complicated to set up, configure, etc. 
- Moderate technical knowledge required 
- Some resources cannot be put in a public cloud for legal/compliance reasons 
- can still run legacy applications/infrastructure in private cloud, while taking newer applications to the public cloud 
 
Advantages 
- Keep systems running even with out-of-date/legacy hardware or OS 
- Flexibility 
- Take advantages of economies of scale from public cloud providers while supplementing with your own hardware/software when needed 

#### Compare and contrast the 3 different cloud models 

Type | Advantages | Disadvantages
------------ | ------------ | -------------
Public | High Scalability and Agility, PAYG (No CapEx, OpEx model), Not responsible for hardware maintenance, Minimal technical knowledge required | May not be able to meet specific security requirements, May not be able to meet specific compliance requirements, You don't own the hardware and may not be able to manage them as you wish
Private | You have complete control, Can meet strict security and compliance requirements | Upfront CapEx costs, Owning equipment limits agility to scale, Requires high technical knowledge
Hybrid | advantages of both private and public, flexibility | Can be more expensive than selecting one deployment model, Can be more complicated to set up and manage, CAPEX

## Core-Azure-Services

#### Describe the benefit and usage of Regions 
- A region is a set/collection of datacenters deployed within a latency-defined perimeter and connected through a dedicated regional low-latency network 
- Is a geographical area (physical location) containing at least 1 or more datacenters that are in close proximity and networked together via low latency network 
- Pick a region that closest to users; pick a region due to cost; pick a region due to compliance reasons; some regions may not have all available features

![AZ and region](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fsecurity%2Ffundamentals%2Fmedia%2Fphysical-security%2Fdata-residency-boundary.png&f=1&nofb=1)

Azure has some special regions that you may wish to use when building out your applications for compliance or legal purposes. These special regions include: 
- US Gov Virginia and US Gov Iowa 
  - A physical and logical network-isolated instance of Azure for US government agencies and partners, operated by screened US persons. Includes additional compliance certifications such as FedRAMP and DISA. Read more about Azure Government. 
- China East and China North 
  - These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft does not directly maintain the datacenters. See more about Azure China 21Vianet. 
- Germany Central and Germany Northeast 
  - These regions are available via a data trustee model whereby customer data remains in Germany under control of T-Systems, a Deutsche Telekom company, acting as the German data trustee. 

Each Azure region is paired with another region within same geography 
- Allows for replication of resources 
- 300 miles of separation between regions
- Region pairs must be in same geography
- One region out of every pair is prioritized to help reduce time it takes to restore applications, etc. 
  - Planned updates are rolled out to paired regions, one region at a time 
  - Data resides in same geography as its pair for tax/law jurisdiction purposes 

![geo](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fmedia%2Fbest-practices-availability-paired-regions%2Fpairedregionsoverview2.png&f=1&nofb=1)

Azure is generally available in 52+ regions worldwide with plans to announce 6+ in future 
- Minimum 3 zones in each region 
- some services or VM features are only available in certain regions; some products are only available in certain regions 
 
Geography – is a discrete market typically containing 2 or more regions that preserve data residency and compliance boundaries 
- Allows customers with specific data residency and compliance needs to keep their data and applications close 
- Americas, Europe, Asia Pacific, Middle East, Africa 
 
Hierarchy: Geography -> Region -> Availability Zone -> Availability Set -> Fault Domain -> Update Domain 

#### Describe the benefit and usage of Availability Zones 
- Availability Zones are physically separate locations within an Azure region.  
- Each Availability Zone is made up of one or more datacenters equipped with independent power, cooling, and networking. 
- Availability Zones allow customers to run mission-critical applications with high availability and low-latency replication. 
- is a high-availability offering that protects your applications and data from datacenter failures.  
- Availability Zones are unique physical locations within an Azure region 
  - minimum of 3 separate zones in all enabled regions 
- is a combination of a fault domain and an update domain 
  - For example, if you create three or more VMs across three zones in an Azure region, your VMs are effectively distributed across three fault domains and three update domains.   - The Azure platform recognizes this distribution across update domains to make sure that VMs in different zones are not updated at the same time. 
- A fault domain is a logical group of underlying hardware that share a common power source and network switch, similar to a rack within an on-premises datacenter. 
  - Physical separate
  - Up to 5 fault domains inside an availability set
- An update domain is a logical group of underlying hardware that can undergo maintenance or be rebooted at the same time. 
  - Up to 20 UD in an availability set
- This approach ensures that at least one instance of your application always remains running as the Azure platform undergoes periodic maintenance. The order of update domains being rebooted may not proceed sequentially during maintenance, but only one update domain is rebooted at a time. 

![AZ](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fcloud-adoption-framework%2Fmigrate%2Fazure-best-practices%2Fmedia%2Fmigrate-best-practices-networking%2Favailability-zone.png&f=1&nofb=1)

- Azure services that support Availability Zones fall into two categories: 
  - Zonal services – you pin the resource to a specific zone (for example, virtual machines, managed disks, Standard IP addresses), or 
  - Zone-redundant services – platform replicates automatically across zones (for example, zone-redundant storage, SQL Database). 
- 99.99% VM uptime SLA is offered when two or more VMs are deployed across two or more Availability Zones within an Azure region 
- No cost for deploying resources in AZ's 

![storage](lrs-grs.png)

#### Describe the benefit and usage of Resource Groups 
A resource group is a container that holds related resources for an Azure solution 
- Is a unit of management for Azure resources 
- MUST create this first
- Includes those resources you want to manage as a group 
- Is a collection of azure resources — azure resources must existing in 1 and only 1 resource group
- RBAC is included 
 
You can manage: 
- Metering and billing 
- Policies 
- Monitoring and alerts 
- Quotas 
- Access control 
- NOTE: if you delete a resource group, all resources are also deleted 
 
Resource group stores metadata about those resources 
- Metadata follows where you put the resource group location; therefore, when you specify a location for the resource group, you are specifying where that metadata is stored 
- Locking prevents users in your organization from accidentally deleting or modifying critical resources 

![resourcelocks](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-au%2Fazure%2Fazure-resource-manager%2Fmanagement%2Fmedia%2Fmanage-resources-portal%2Fmanage-azure-resources-portal-lock-resource.png&f=1&nofb=1)

All the resources in your resource group should share the same / similar life cycle 
- You deploy, update, and delete them together 
- Each resource can only exist in one resource group 
- You can add or remove a resource at any time 
- You can move a resource from one group to another 
- A resource group can contain resources that are located in different regions 
- A resource group can be used to scope access control for administrative actions 
- A resource group can interact with resources in other resource groups 
- You can export Azure Resource Manager (ARM) templates to 1) automate future deployments, and 2) learn JSON syntax that represents a solution 
 
You can apply tags to resource groups and resources to logically organize your assets. For information, see Using tags to organize your Azure resources. 

#### Describe the benefit and usage of Azure Resource Manager 
- Is the deployment and management service for Azure – provides a management layer that enables you to create, update, and delete resources in your Azure subscription 
- Allows you to automate the deployment and configuration of resources using different tools like PowerShell, Azure CLI, Portal, REST API, and SDK 
- A resource is a manageable item through Azure (VM, storage accounts, web apps, database's, etc) 
 
You use management features like access control, locks, and tags to secure and organize resources after deployment 
- When a user sends a request from any of the Azure tools, ARM receives this request. It then authenticates and authorizes the request. ARM sends the request to the Azure service which takes the requested action. All requests are handled through the same API and therefore has consistent results 

![arm](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fazure-resource-manager%2Fmedia%2Fresource-group-overview%2Fconsistent-management-layer.png&f=1&nofb=1)

ARM Template - A JavaScript Object Notation (JSON) file that defines one or more resources to deploy to a resource group or subscription. The template can be used to deploy the resources consistently and repeatedly. See Template deployment overview. 
  
Azure provides four levels of scope: management groups, subscriptions, resource groups, and resources. The following image shows an example of these layers. 

![scopelevels](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-in%2Fazure%2Fazure-resource-manager%2Fmedia%2Fresource-group-overview%2Fscope-levels.png&f=1&nofb=1)

You apply management settings at any of these levels of scope. The level you select determines how widely the setting is applied. Lower levels inherit settings from higher levels. For example, when you apply a policy to the subscription, the policy is applied to all resource groups and resources in your subscription. When you apply a policy on the resource group, that policy is applied the resource group and all its resources. However, another resource group doesn't have that policy assignment. 
- You can deploy templates to management groups, subscriptions, or resource groups. 

Resource Manager and control plane operations (requests sent to management.azure.com) in the REST API are: 
- Distributed across regions. Some services are regional. 
- Distributed across Availability Zones (as well regions) in locations that have multiple Availability Zones. 
- Not dependent on a single logical data center. 
- Never taken down for maintenance activities. 
 
Benefits: 
- Use of declarative templates (JSON file) rather than scripts 
- Deploy, manage, and monitor all resources for your solution as a group 
- Capable of redeploying solution throughout development cycle 
- Defines dependencies between resources 
- RBAC 
- Ability to apply tags 
- Clarity of organizational billing via costs for groups of resources and sharing the same tag(s) 

#### Describe products available for compute products such as Virtual Machines, VM Scale Sets, App Services, Azure Container Instances (ACI), Azure Kubernetes Service (AKS)  
Virtual Machines 
- Is one of several types of on-demand scalable computing resources that Azure offers 
- VM's are software emulations of physical computers 
- Are offered as IaaS 
- single instance virtual machine SLA of 99.9% provided you deploy the VM with premium and managed storage for all disks
- VM SLA of 99.95% when deployed with 2 VMs in an availability set
- Virtual Machines that have two or more instances deployed across two or more Availability Zones in the same Azure region, we guarantee you will have Virtual Machine Connectivity to at least one instance at least 99.99% of the time

VM Scale Sets 
- Are Azure compute resources you can use to deploy and manage a set of identical VM's (load balanced VM's) 
- The number of VM instances can automatically increase or decrease in response to demand or a defined schedule. Scale sets provide high availability to your applications, and allow you to centrally manage, configure, and update many VMs. We recommended that two or more VMs are created within a scale set to provide for a highly available application and to meet the 99.95% Azure SLA. 
- There is no cost for the scale set itself, you only pay for each VM instance that you create. 
- When a single VM is using Azure premium SSDs, the Azure SLA applies for unplanned maintenance events. Virtual machines in a scale set can be deployed across multiple update domains and fault domains to maximize availability and resilience to outages due to data center outages, and planned or unplanned maintenance events. Virtual machines in a scale set can also be deployed into a single Availability zone, or regionally. Availability zone deployment options may differ based on the orchestration mode. 
- All VM's are the same so Scale Sets supports true autoscale (no pre-provisioning of VMs) 
- Targets big data compute jobs and containerized workloads 
- Manual or automated tasks 
 
Typically choose a VM when you need more control over the computing environment (like the OS) 
- Still need to maintain the VM like configuring, patching, and installing software 
- VM use cases = Dev/Test, applications in the cloud, extend your datacenter 
- The location specifies where the virtual hard disks (VHD) are stored 
- HOURLY price based on VM size + operating system 
- A VM subscription has default quota limits – current default is 20 VM's per region but can be increased via support ticket 

Availability Set
An Availability Set is a logical grouping of VMs within a datacenter that allows Azure to understand how your application is built to provide for redundancy and availability. We recommended that 2 or more VMs are created within an availability set to provide for a highly available application and to meet the 99.95% Azure SLA.  
There is no cost for the Availability Set itself, you only pay for each VM instance that you create. When a single VM is using Azure premium SSDs, the Azure SLA applies for unplanned maintenance events. 
- It ensures your application remains online if a high-impact maintenance event is required or hardware failure occurs 
- In an availability set, VMs are automatically distributed across these fault domains. This approach limits the impact of potential physical hardware failures, network outages, or power interruptions. 
- For VMs using Azure Managed Disks, VMs are aligned with managed disk fault domains when using a managed availability set. This alignment ensures that all the managed disks attached to a VM are within the same managed disk fault domain. 
- Only VMs with managed disks can be created in a managed availability set. The number of managed disk fault domains varies by region - either two or three managed disk fault domains per region. You can read more about these managed disk fault domains for Linux VMs or Windows VMs. 

![avset](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fincludes%2Fmedia%2Fvirtual-machines-common-manage-availability%2Fmd-fd-updated.png&f=1&nofb=1)

Fault Domain and Update Domain

![fdud](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fincludes%2Fmedia%2Fvirtual-machines-common-manage-availability%2Fud-fd-configuration.png&f=1&nofb=1)

Azure App Service = PaaS
- is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. 
- fully managed compute platform that is optimized for hosting websites and web applications
- can also take advantage of its DevOps capabilities, such as continuous deployment from Azure DevOps, GitHub, Docker Hub, and other sources, package management, staging environments, custom domain, and SSL certificates. 
- With App Service, you pay for the Azure compute resources you use. The compute resources you use is determined by the App Service plan that you run your apps on 
App Service Environment is an Azure App Service feature that provides a fully isolated and dedicated environment for securely running App Service apps at high scale. 
- Besides App Service, Azure offers other services that can be used for hosting websites and web applications. For most scenarios, App Service is the best choice. For microservice architecture, consider Service Fabric

Whatever apps you put into this App Service plan run on these compute resources as defined by your App Service plan. Each App Service plan defines: 
1. Region (West US, East US, etc.) 
2. Number of VM instances 
3. Size of VM instances (Small, Medium, Large) 
4. Pricing tier (Free, Shared, Basic, Standard, Premium, PremiumV2, Isolated) 

Benefits 
- Multiple languages supported 
- DevOps optimization 
- Global scale with HA 
- SaaS and on-premise connectivity 
- Application templates 
- Serverless 
- API+Mobile features 
- Visual Studio integration 
- Is ISO, SOC, and PCI compliant 

Azure Container Instances (ACI) = PaaS
- Is the fastest and simplest way to run a container in Azure without having to manage any virtual instances (basically containers as a service) 
- is a great solution for any scenario that can operate in isolated containers, including simple applications, task automation, and build jobs. 
- Is a PaaS offering 
- Pay based on what you need and get billed by the second – PAY GO model 
- ACI uses Azure Files shares backed by Azure Storage for persistent storage 
- For compute-intensive jobs such as machine learning, Azure Container Instances can schedule Linux containers to use NVIDIA Tesla GPU resources (preview). 
 
YAML is recommended for container deployments 
Can use ARM templates to deploy ACI and containers 

Azure Kubernetes Service (AKS) = PaaS
- Azure Kubernetes Service (AKS) makes it simple to deploy a managed Kubernetes cluster in Azure. AKS reduces the complexity and operational overhead of managing Kubernetes by offloading much of that responsibility to Azure. As a hosted Kubernetes service, Azure handles critical tasks like health monitoring and maintenance for you. The Kubernetes masters are managed by Azure. You only manage and maintain the agent nodes. As a managed Kubernetes service, AKS is free - you only pay for the agent nodes within your clusters, not for the masters. 
- You can create an AKS cluster in the Azure portal, with the Azure CLI, or template driven deployment options such as Resource Manager templates and Terraform. When you deploy an AKS cluster, the Kubernetes master and all nodes are deployed and configured for you. Additional features such as advanced networking, Azure Active Directory integration, and monitoring can also be configured during the deployment process. Windows Server containers support is currently in preview in AKS. 
- AKS lets you integrate with Azure Active Directory and use Kubernetes role-based access controls. You can also monitor the health of your cluster and resources. 

![aks](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fda-dk%2Fazure%2Farchitecture%2Freference-architectures%2Fmicroservices%2F_images%2Faks.png&f=1&nofb=1)

AKS supports Kubernetes role-based access control (RBAC). RBAC lets you control access to Kubernetes resources and namespaces, and permissions to those resources. You can also configure an AKS cluster to integrate with Azure Active Directory (AD).

Azure Monitor for container health collects memory and processor metrics from containers, nodes, and controllers. Container logs are available, and you can also review the Kubernetes master logs. This monitoring data is stored in an Azure Log Analytics workspace, and is available through the Azure portal, Azure CLI, or a REST endpoint.

AKS nodes run on Azure virtual machines. You can connect storage to nodes and pods, upgrade cluster components, and use GPUs. AKS supports Kubernetes clusters that run multiple node pools to support mixed operating systems and Windows Server containers (currently in preview). Linux nodes run a customized Ubuntu OS image, and Windows Server nodes run a customized Windows Server 2019 OS image.

An AKS cluster can be deployed into an existing virtual network. In this configuration, every pod in the cluster is assigned an IP address in the virtual network, and can directly communicate with other pods in the cluster, and other nodes in the virtual network. Pods can connect also to other services in a peered virtual network, and to on-premises networks over ExpressRoute or site-to-site (S2S) VPN connections.

AKS supports the Docker image format. For private storage of your Docker images, you can integrate AKS with Azure Container Registry (ACR).

Azure Kubernetes Service (AKS) is compliant with SOC, ISO, PCI DSS, and HIPAA 

Nodes and node pools 
To run your applications and supporting services, you need a Kubernetes node. An AKS cluster has one or more nodes, which is an Azure virtual machine (VM) that runs the Kubernetes node components and container runtime: 
- The kubelet is the Kubernetes agent that processes the orchestration requests from the control plane and scheduling of running the requested containers. 
- Virtual networking is handled by the kube-proxy on each node. The proxy routes network traffic and manages IP addressing for services and pods. 
- The container runtime is the component that allows containerized applications to run and interact with additional resources such as the virtual network and storage. In AKS, Moby is used as the container runtime. (other public options are Docker, CRI-O, containerd)

#### Describe products available for networking such as Virtual Networks, Load Balancer, VPN Gateway, Application Gateway, and CDN 
Virtual Networks 
- is a logical representation of your network in the cloud. It allows you to define your own private IP address space and segment the network into subnets.
- VNets serves as a trust boundary to host your compute resources such as Azure Virtual Machines and Cloud Services (web/worker roles). A VNet allows direct private IP communication between the resources hosted in it. You can link a virtual network to an on-premises network through a VPN Gateway, or ExpressRoute. 
- Public IP addresses may have a nominal charge. To learn more about IP address pricing in Azure, review the IP address pricing page.
- $0.0036/hour

VNet concepts 
- Address space: When creating a VNet, you must specify a custom private IP address space using public and private (RFC 1918) addresses. Azure assigns resources in a virtual network a private IP address from the address space that you assign. For example, if you deploy a VM in a VNet with address space, 10.0.0.0/16, the VM will be assigned a private IP like 10.0.0.4. 
- Subnets: Subnets enable you to segment the virtual network into one or more sub-networks and allocate a portion of the virtual network's address space to each subnet. You can then deploy Azure resources in a specific subnet. Just like in a traditional network, subnets allow you to segment your VNet address space into segments that are appropriate for the organization's internal network. This also improves address allocation efficiency. You can secure resources within subnets using Network Security Groups. For more information, see Security groups. 
- Regions: VNet is scoped to a single region/location; however, multiple virtual networks from different regions can be connected together using Virtual Network Peering. 
Subscription: VNet is scoped to a subscription. You can implement multiple virtual networks within each Azure subscription and Azure region. 

All resources in a VNet can communicate outbound to the internet, by default. You can communicate inbound to a resource by assigning a public IP address or a public Load Balancer. You can also use public IP or public Load Balancer to manage your outbound connections

Outbound communication is enabled by default; inbound communication requires public IP address or load balancer IP address

You can filter network traffic between subnets using either or both of the following options: 
- Security groups: Network security groups and application security groups can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by source and destination IP address, port, and protocol. To learn more, see Network security groups or Application security groups. 
- Network virtual appliances: A network virtual appliance is a VM that performs a network function, such as a firewall, WAN optimization, or other network function. To view a list of available network virtual appliances that you can deploy in a virtual network, see Azure Marketplace.
- There is no charge for using Azure VNet, it is free of cost. Standard charges are applicable for resources, such as Virtual Machines (VMs) and other products 
- On-premise communication: P2P, Site-to-site VPN, or via ExpressRoute 

Load Balancer 
- Refers to evenly distributing load (incoming network traffic) across a group of backend resources or servers.
- Azure Load Balancer operates at layer 4 of the Open Systems Interconnection (OSI) model. It's the single point of contact for clients. Load Balancer distributes inbound flows that arrive at the load balancer's front end to backend pool instances. These flows are according to configured load balancing rules and health probes. The backend pool instances can be Azure Virtual Machines or instances in a virtual machine scale set.
- operate at the transport layer (OSI layer 4 - TCP and UDP) and route traffic based on source IP address and port, to a destination IP address and port.

VPN Gateway 
- is used to send encrypted traffic between an Azure virtual network and an on-premises location over the public Internet
- Each virtual network can only have one VPN gateway

A virtual network gateway is composed of two or more VMs that are deployed to a specific subnet you create called the gateway subnet. Virtual network gateway VMs contain routing tables and run specific gateway services. These VMs are created when you create the virtual network gateway. You can't directly configure the VMs that are part of the virtual network gateway.
- One setting that you configure for a virtual network gateway is the gateway type. Gateway type specifies how the virtual network gateway will be used and the actions that the gateway takes. The gateway type 'Vpn' specifies that the type of virtual network gateway created is a 'VPN gateway', rather than an ExpressRoute gateway. A virtual network can have two virtual network gateways; one VPN gateway and one ExpressRoute gateway
- The gateway subnet contains the IP addresses that the virtual network gateway services use. You need to create a gateway subnet for your VNet in order to configure a virtual network gateway. All gateway subnets must be named 'GatewaySubnet' to work properly

Application Gateway = WAF
- is a web traffic load balancer that enables you to manage traffic to your web applications
- Application Gateway can make routing decisions based on additional attributes of an HTTP request, for example URI path or host headers. For example, you can route traffic based on the incoming URL. So if /images is in the incoming URL, you can route traffic to a specific set of servers (known as a pool) configured for images. If /video is in the URL, that traffic is routed to another pool that's optimized for videos.
- This type of routing is known as application layer (OSI layer 7) load balancing. Azure Application Gateway can do URL-based routing and more.

CDN 
- Is a distributed network of servers that can efficiently deliver web content to users. 
- CDNs store cached content on edge servers in point-of-presence (POP) locations that are close to end users, to minimize latency

#### Describe products available for storage such as Blob, Disk Storage, File Storage, and Archive Storage

![storage](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Faspnet%2Faspnet%2Foverview%2Fdeveloping-apps-with-windows-azure%2Fbuilding-real-world-cloud-apps-with-windows-azure%2Fdata-storage-options%2F_static%2Fimage5.png&f=1&nofb=1)

Blob Storage - Azure Blob storage is Microsoft's object storage solution for the cloud. Blob storage is optimized for storing massive amounts of unstructured data. Unstructured data is data that doesn't adhere to a particular data model or definition, such as text or binary data. 
- Highly scalable 
- Can manage thousands of simultaneous uploads 
- No file format per se 
- Tiered storage 
 
Blob storage is designed for: 
- Serving images or documents directly to a browser. 
- Storing files for distributed access. 
- Streaming video and audio. 
- Writing to log files. 
- Storing data for backup and restore, disaster recovery, and archiving. 
- Storing data for analysis by an on-premises or Azure-hosted service. 
- Supports Azure Data Lake storage (Gen 2) 
- Users or client applications can access objects in Blob storage via HTTP/HTTPS

Blob storage offers three types of resources: 
- The storage account 
- A container in the storage account 
- A blob in a container 

![blob](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fstorage%2Fblobs%2Fmedia%2Fstorage-blob-introduction%2Fblob1.png&f=1&nofb=1)

Containers use a "scratch" space by default; Windows containers by default use ephemeral storage 
- Ideal for stateless applications. 
- They can be used with both Marketplace and custom images. 
- Ability to fast reset or reimage VMs and scale set instances to the original boot state. 
- Lower latency, similar to a temporary disk. 
- Ephemeral OS disks are free, you incur no storage cost for OS disk. 
- They are available in all Azure regions. 
- Ephemeral OS Disk is supported by Shared Image Gallery

All container I/O happens in "scratch" space and each container gets their own scratch space
File creation and file writes are captured in the scratch space and do not escape to the host
When a container instance is stopped, all changes that occurred in the "scratch" space are thrown away; when a new container instance is started, a new "scratch" space is provided for the instance

Data Lake storage: 
- Is a set of capabilities dedicated to big data analytics, built on Azure Blob storage
- Data Lake Storage Gen2 is the result of converging the capabilities of our two existing storage services, Azure Blob storage and Azure Data Lake Storage Gen1
- A fundamental part of Data Lake Storage Gen2 is the addition of a hierarchical namespace to Blob storage.
- A superset of POSIX permissions - The security model for Data Lake Gen2 supports ACL and POSIX permissions
- Big data analytics 
- Hadoop compatible - allows you to manage and access data just as you would with a Hadoop Distributed File System (HDFS)

Disk Storage – Managed Disks 
Azure managed disks are block-level storage volumes that are managed by Azure and used with Azure Virtual Machines. The available types of disks are ultra disks, premium solid-state drives (SSD), standard SSDs, and standard hard disk drives (HDD). 

Benefits: 
- Highly durable and scalable 
- Integration with availability sets 
- Integration with availability zones 
- Azure Backup support 
- RBAC 
- VHD upload 

There are 3 main disk roles in Azure: the data disk, the OS disk, and the temporary disk. These roles map to disks that are attached to your virtual machine.

![diskroles](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fhe-il%2Fazure%2Fincludes%2Fmedia%2Fvirtual-machines-managed-disks-overview%2Fdisk-types.png&f=1&nofb=1)

Data disk 
A data disk is a managed disk that's attached to a virtual machine to store application data, or other data you need to keep. Data disks are registered as SCSI drives and are labeled with a letter that you choose. Each data disk has a maximum capacity of 32,767 gibibytes (GiB). The size of the virtual machine determines how many data disks you can attach to it and the type of storage you can use to host the disks. 

OS disk 
Every virtual machine has one attached operating system disk. That OS disk has a pre-installed OS, which was selected when the VM was created. This disk contains the boot volume. 
- This disk has a maximum capacity of 2,048 GiB. 

Temporary disk 
Every VM contains a temporary disk, which is not a managed disk. The temporary disk provides short-term storage for applications and processes and is intended to only store data such as page or swap files. Data on the temporary disk may be lost during a maintenance event event or when you redeploy a VM. On Azure Linux VMs, the temporary disk is /dev/sdb by default and on Windows VMs the temporary disk is D: by default. During a successful standard reboot of the VM, the data on the temporary disk will persist.

Managed disk snapshots 
- A managed disk snapshot is a read-only crash-consistent full copy of a managed disk that is stored as a standard managed disk by default. With snapshots, you can back up your managed disks at any point in time. These snapshots exist independent of the source disk and can be used to create new managed disks. 
Snapshots are billed based on the used size 

Images 
- Managed disks also support creating a managed custom image. You can create an image from your custom VHD in a storage account or directly from a generalized (sysprepped) VM. This process captures a single image. This image contains all managed disks associated with a VM, including both the OS and data disks. This managed custom image enables creating hundreds of VMs using your custom image without the need to copy or manage any storage accounts.

File Storage 
- Azure Files offers fully managed file shares in the cloud that are accessible via the industry standard Server Message Block (SMB) protocol. Azure file shares can be mounted concurrently by cloud or on-premises deployments of Windows, Linux, and macOS. Additionally, Azure file shares can be cached on Windows Servers with Azure File Sync for fast access near where the data is being used. 
- Secures data at rest and in transit using SMB 3.0 and HTTPS 
- Create high-performance file shares using Premium Files storage tier 
- Compatible with Azure Files AD authentication on-premise infrastructure

Benefits: 
- Replace or supplement on-premises file servers 
- "Lift and shift" applications 
- Simplify cloud development 
  - Shared application settings - A common pattern for distributed applications is to have configuration files in a centralized location where they can be accessed from many application instances. Application instances can load their configuration through the File REST API, and humans can access them as needed by mounting the SMB share locally. 
  - Diagnostic share - An Azure file share is a convenient place for cloud applications to write their logs, metrics, and crash dumps. Logs can be written by the application instances via the File REST API, and developers can access them by mounting the file share on their local machine. This enables great flexibility, as developers can embrace cloud development without having to abandon any existing tooling they know and love. 
  - Dev/Test/Debug - When developers or administrators are working on VMs in the cloud, they often need a set of tools or utilities. Copying such utilities and tools to each VM can be a time consuming exercise. By mounting an Azure file share locally on the VMs, a developer and administrator can quickly access their tools and utilities, no copying required

Azure Files can be deployed in two main ways: by directly mounting the serverless Azure file shares or by caching Azure file shares on-premises using Azure File Sync 
- Azure File Sync – a method to ingest data into an Azure file share 
- Maintains ACL's and timestamps 
- Azure file shares are deployed into storage accounts, which are top-level objects that represent a shared pool of storage. This pool of storage can be used to deploy multiple file shares, as well as other storage resources such as blob containers, queues, or tables. All storage resources that are deployed into a storage account share the limits that apply to that storage account

To access an Azure file share, the user of the file share must be authenticated and have authorization to access the share. This is done based on the identity of the user accessing the file share. Azure Files integrates with three main identity providers: 
1. Customer-owned Active Directory 
2. Azure Active Directory Domain Services (Azure AD DS) 
3. Azure storage account key

Azure Files supports two different types of encryption: encryption in transit, which relates to the encryption used when mounting/accessing the Azure file share, and encryption at rest, which relates to how the data is encrypted when it is stored on disk.

Encryption in transit 
- By default, all Azure storage accounts have encryption in transit enabled. This means that when you mount a file share over SMB or access it via the FileREST protocol (such as through the Azure portal, PowerShell/CLI, or Azure SDKs), Azure Files will only allow the connection if it is made with SMB 3.0+ with encryption or HTTPS

Encryption at rest 
- All data stored in Azure Files is encrypted at rest using Azure storage service encryption (SSE). Storage service encryption works similarly to BitLocker on Windows: data is encrypted beneath the file system level. Because data is encrypted beneath the Azure file share's file system, as it's encoded to disk, you don't have to have access to the underlying key on the client to read or write to the Azure file share. 
- By default, data stored in Azure Files is encrypted with Microsoft-managed keys. With Microsoft-managed keys, Microsoft holds the keys to encrypt/decrypt the data, and is responsible for rotating them on a regular basis

Archive Storage 
Azure storage offers different access tiers, which allow you to store blob object data in the most cost-effective manner. The available access tiers include:
1. Hot - Optimized for storing data that is accessed frequently.
2. Cool - Optimized for storing data that is infrequently accessed and stored for at least 30 days.
3. Archive - Optimized for storing data that is rarely accessed and stored for at least 180 days with flexible latency requirements (on the order of hours).
2 hour latency (time to first byte)

- Archive storage stores data offline and offers the lowest storage costs but also the highest data rehydrate and access costs
- The archive access tier has the lowest storage cost. But it has higher data retrieval costs compared to the hot and cool tiers. Data in the archive tier can take several hours to retrieve. Data must remain in the archive tier for at least 180 days or be subject to an early deletion charge.
- While a blob is in archive storage, the blob data is offline and can't be read, overwritten, or modified. To read or download a blob in archive, you must first rehydrate it to an online tier

Usage scenarios for the archive access tier include:
- Long-term backup, secondary backup, and archival datasets
- Original (raw) data that must be preserved, even after it has been processed into final usable form.
- Compliance and archival data that needs to be stored for a long time and is hardly ever accessed

Storage Tiers 
Azure Files offers 2 different tiers of storage, premium and standard, to allow you to tailor your shares to the performance and price requirements of your scenario: 
1. Premium file shares: Premium file shares are backed by solid-state drives (SSDs) and are deployed in the FileStorage storage account type. Premium file shares provide consistent high performance and low latency, within single-digit milliseconds for most IO operations, for IO-intensive workloads. This makes them suitable for a wide variety of workloads like databases, web site hosting, and development environments. Premium file shares are only available in a provisioned billing model. For more information on the provisioned billing model for premium file shares, see Understanding provisioning for premium file shares. 
- Premium file shares are provisioned based on a fixed GiB/IOPS/throughput ratio 
- Premium file shares can burst their IOPS up to a factor of three 

2. Standard file shares: Standard file shares are backed by hard disk drives (HDDs) and are deployed in the general purpose version 2 (GPv2) storage account type. Standard file shares provide reliable performance for IO workloads that are less sensitive to performance variability such as general-purpose file shares and dev/test environments. Standard file shares are only available in a pay-as-you-go billing model. 
- By default, standard file shares can span only up to 5 TiB, although the share limit can be increased to 100 TiB

#### Describe products available for databases such as Cosmos DB, Azure SQL Database, Azure Database for MySQL, Azure Database for PostgreSQL, and Azure Database Migration service 
Cosmos DB – is Microsoft's globally distributed, multi-model database service (key-value, column-family, documents, graph) 
- Supports schema-less data with Always On applications 
- Can add data concurrently from multiple regions 
- Can store JSON documents 
- 99.999% SLA for HA 
- Is a No-SQL database / non-relational DB
- Supports wire protocols 
- All APIs are exposed by Cosmos DB – SQL, MongoDB, Cassandra, Gremlin, and Table can be used

Benefits 
- Turnkey global distribution – replicates data wherever you are 
- Always On – with multi-master replication capabilities 
- Scalability and throughput of storage – writes and reads across global servers; increase scale easily 
- Optimized latency – less than 10ms reads/writes 
- Multiple consistency options – strong, bound staleness, session, consistent prefix, and eventual 
- No schema or index management – database engine is schema-agnostic 
- Battle tested – works for MSFT office, XBox, O365, Skype, etc

![consistency](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-gb%2Fazure%2Fcosmos-db%2Fmedia%2Fconsistency-levels%2Ffive-consistency-levels.png&f=1&nofb=1)

Cosmos DB is great for: 
- Any web, mobile, gaming, and IoT application that needs to handle massive amounts of data, reads, and writes at a global scale with near-real response times for a variety of data 
- Near real-time response times 
- Low latency, high throughput 
- Cosmos DB can run Apache Spark 
 
Partitioning 
- Uses partitioning to scale individual containers in a DB to meet the performance needs of the application 
- Divided into distinct subsets called logical partitions 
 
Provisioned Throughput 
- You pay for the throughput you provision per hour 
- Ensures sufficient system resources are available for Azure Cosmos DB; expressed by request units (RU's) 
 
Use Cases 
1. web / retail / marketing 
2. mobile 
3. gaming 
4. IoT / Telematics

Azure SQL Database – general purpose relational database, provided as a managed service 
- Is a fully managed PaaS Database Engine that handles upgrades, patching, backup, and monitoring 
- Predictable performance, dynamic scalability (manual scaling) 
- Available in 38 datacenters 
- Process both relational data and non-relational data (graphs, JSON, spatial, XML) 
- Uses latest Microsoft SQL Server database engine 
 
Use Cases 
1. modern cloud applications 
2. high performance in-memory & intelligent query processing 
3. backup

![azuresql](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fsql-database%2Fmedia%2Fsql-database-paas-vs-sql-server-iaas%2Fsqliaas_sql_server_cloud_continuum.png&f=1&nofb=1)

Azure SQL Deployment Models

![deplymentmodels](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdocs.microsoft.com%2Fen-ca%2Fazure%2Fsql-database%2Fmedia%2Fsql-database-technical-overview%2Fdeployment-options.png&f=1&nofb=1)

- Single Database represents a fully managed, isolated database. You might use this option if you have modern cloud applications and microservices that need a single reliable data source. A single database is similar to a contained database in Microsoft SQL Server Database Engine. 
- Managed instance is a fully managed instance of the Microsoft SQL Server Database Engine. It contains a set of databases that can be used together. Use this option for easy migration of on-premises SQL Server databases to the Azure cloud, and for applications that need to use the database features that SQL Server Database Engine provides. 
- Elastic pool is a collection of single databases with a shared set of resources, such as CPU or memory. Single databases can be moved into and out of an elastic pool

Purchasing Models 
1. vCore-based (recommended) - independently choose compute and storage resources; allows you to use Azure Hybrid Benefit for SQL Server to gain cost savings 
Best for customers who value flexibility, control, and transparency 
2. DTU-based (Database Transaction Unit) - based on a bundled compute and storage packages balanced for common workloads; differentiated by a range of compute sizes with a fixed amount of included storage, retention period for backups, and a fixed price 
  - Best for customers who want preconfigured resource options

SQL Database offers the following purchasing models: 
- The vCore-based purchasing model lets you choose the number of vCores, the amount of memory, and the amount and speed of storage. The vCore-based purchasing model also allows you to use Azure Hybrid Benefit for SQL Server to gain cost savings. For more information about the Azure Hybrid Benefit, see the "Frequently asked questions" section later in this article. 
- The DTU-based purchasing model offers a blend of compute, memory, and I/O resources in three service tiers, to support light to heavy database workloads. Compute sizes within each tier provide a different mix of these resources, to which you can add additional storage resources. 
- The serverless model automatically scales compute based on workload demand, and bills for the amount of compute used per second. The serverless compute tier also automatically pauses databases during inactive periods when only storage is billed, and automatically resumes databases when activity returns

Service tiers 
Azure SQL Database offers three service tiers that are designed for different types of applications: 
- General Purpose/Standard service tier designed for common workloads. It offers budget-oriented balanced compute and storage options. 
- Business Critical/Premium service tier designed for OLTP applications with high transaction rate and lowest-latency I/O. It offers the highest resilience to failures by using several isolated replicas. 
- Hyperscale service tier designed for very large OLTP database and the ability to auto-scale storage and scale compute fluidly

Azure Database for MySQL – is a relational database service in Azure based on the MySQL Community Edition (GPLv2 license); versions 5.6, 5.7, and 8.0 
- Built-in high availability with no additional cost
- Most used database / most popular
- PHP & Python apps

Use Cases
- Developed for SaaS and web applications
- Enterprise content management
- E-comm and payment platforms
- Gaming 
- Predictable performance, using inclusive pay-as-you-go pricing. 
- Scale as needed within seconds. 
- Secured to protect sensitive data at-rest and in-motion. 
- Automatic backups and point-in-time-restore for up to 35 days. 
- Enterprise-grade security and compliance — integrated with Advanced Threat Protection (ATP)
- PAY GO model 
- Fault Tolerance 
- Automatic patching service 
- Automatic backups 

Pricing Model 
Is priced per server based on the configuration of pricing tier, vCores, and storage

An Azure Database for MySQL server: 
- Is created within an Azure subscription. 
- Is the parent resource for databases. 
- Provides a namespace for databases. 
- Is a container with strong lifetime semantics - delete a server and it deletes the contained databases. 
- Collocates resources in a region. 
- Provides a connection endpoint for server and database access. 
- Provides the scope for management policies that apply to its databases: login, firewall, users, roles, configurations, etc. 
- Is available in multiple versions. For more information, see Supported Azure Database for MySQL database versions

Azure Database for PostgreSQL – is a relational database service in Azure for developers 
- Is based on the community version of open source PostgreSQL database engine 
- PAY GO model 
- Vertical scaling / scale up 
- Query parallelization 
- Multi-tenant applications 
- Realtime processing analytics

2 Deployment Models 
1. Azure Database for PostgreSQL - Single Server 
  - Built-in high availability with no additional cost (99.99% SLA) 
  - Predictable performance, using inclusive pay-as-you-go pricing 
  - Vertical scale as needed within seconds 
  - Monitoring and alerting to assess your server 
  - Enterprise-grade security and compliance 
  - Secured to protect sensitive data at-rest and in-motion 
  - Automatic backups and point-in-time-restore for up to 35 days 
  - offers three pricing tiers: Basic, General Purpose, and Memory Optimized 

2. Azure Database for PostgreSQL - Hyperscale (Citus) 
  - Horizontal scaling across multiple machines using sharding 
  - Query parallelization across these servers for faster responses on large datasets 
  - Excellent support for multi-tenant applications, real time operational analytics, and high throughput transactional workloads 
  - The Hyperscale (Citus) hosting type allows Azure Database for PostgreSQL servers (called nodes) to coordinate with one another in a "shared nothing" architecture. The nodes in a server group collectively hold more data and use more CPU cores than would be possible on a single server. The architecture also allows the database to scale by adding more nodes to the server group.
  - Microsoft aims to support n-2 versions of the PostgreSQL engine in Azure Database for PostgreSQL - Single Server. The versions would be the current major version on Azure (n) and the two prior major versions (-2) 
  - PostgreSQL 9.5, 9.6, 10, and 11

Azure Database Migration service – is a fully managed service designed to enable seamless migrations from multiple database sources to Azure data platforms with minimal downtime (online migrations)
- The service uses the Data Migration Assistant to generate assessment reports that provide recommendations to guide you through the changes required prior to performing a migration
- Azure Database Migration Service is designed to support different migration scenarios (source/target pairs) for both offline (one-time) and online (continuous sync) migrations

The Standard pricing tier supports offline (also called “one-time”) migrations. The Standard pricing tier, which offers 1-, 2-, and 4-vCore options, is generally available and free to customers.

The Premium pricing tier supports offline and online migrations (also called "continuous migration") for business critical workloads that require minimal downtime. The Premium pricing tier is generally available.






























