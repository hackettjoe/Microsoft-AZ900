# Microsoft-AZ900
> These are my personal notes from studying for the Microsoft Fundamentals AZ-900 exam>.

## Table of Contents

- [Cloud-Concepts](#Cloud-Concepts)

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
------------ | -------------
Public | High Scalability/Agility, PAYG (No CapEx, OpEx model), Not responsible for hardware maintenance, Minimal technical knowledge required | May not be able to meet specific security requirements, May not be able to meet specific compliance requirements, You don't own the hardware and may not be able to manage them as you wish
Private | You have complete control, Can meet strict security and compliance requirements | Upfront CapEx costs, Owning equipment limits agility to scale, Requires high technical knowledge
Hybrid | advantages of both private and public, flexibility | Can be more expensive than selecting one deployment model, Can be more complicated to set up and manage, CAPEX

















