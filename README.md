# Az 900 exam certification

● Candidates with non-technical backgrounds

## Describe Cloud Concepts

Benefits of Cloud Computing
Benefits
Cost savings - both real and accounting
Agility
Availability
Security
Global reach
Range of ready on-demand services
Range of tools

Cost Savings - Real
Economies of scale
Total cost of ownership (TCO) - electricity, Internet,
cooling, employees
Microsoft can run a server cheaper than anyone else
with few exceptions
4 vCPU server - as low as $187/mo

You can take actions to reduce your cost - i.e. autoscaling

Global reach - ukazat slajd kde maji datacentra

High Availability - Expressed as a percentage, it’s the ability of a system to respond to users, zalezi na sluzbe

Scalability - The ability of a system to handle growth of users or work

Elasticity - The ability of a system to automatically grow and shrink based on application demand

Agility - The ability to change rapidly based on changes to market or environment

Disaster recovery - The ability of a system to recover from failure within a period of time, and how much data is lost

Capital Expenditure (CapEx) and Operational Expenditure (OpEx) - CapEx is money invested in assets (like computers) that return investment over time
OpEx is money spent every day on operating expenses

Consumption-Based Model
Pay per minute
Pay per hour
Pay per execution

### IAAS - ukazat v portalu vytvoreni VM
Virtual machines, networking,load balancers, firewalls

### PAAS - uakazat vytvoreni storage, DB
Upload code packages and have them run, without access to the hardware

### SAAS - office 365
Access to configuration only

Shared Responsibility Model - dat sem obrazek za co je zodpovedny MS a za co my

Serverless - There are still servers… you just don’t ever have to deal with them
Even less access to the server than PaaS

Even with PaaS, you have to choose an App Service Plan

With PaaS, scaling is your responsibility

Serverless means not worrying about choosing the right plan

Serverless means not worrying about scaling

Serverless means you might pay $0 if you don’t use the service

Azure Serverless Offers
Compute - Azure Functions
Compute - Serverless Kubernetes (Virtual Nodes w/ ACI)
Database - Azure SQL Database Serverless
Database - Cosmos DB Serverless (preview)


### Public cloud
Azure owns the hardware, on their network and infrastructure

### private cloud
Looks and acts like a cloud, except customer owns or leases or has exclusive access to the hardware

### Hybrid cloud
Combination of public and private clouds; scale private infrastructure to the cloud



### Describe Core Azure Services (15-20%)

Core Azure architectural components
Regions - 60+, dat sem aktualni obrazek datacenter

Region pairs
Each region has one other region which is treated as it’s “pair” Almost always in the same geography - data storage laws The data connection between region pairs is the highest speed available Software rollouts are deployed to one region of a pair and the other is not touched If multiple regions go down, one region of each pair is treated as a priority

Example Pairs
Canada Canada Central - Canada East
Europe North Europe - West Europe
USA East US - West US
USA East US 2 - Central US
USA North Central US - South Central US
Brazil Brazil South - South Central US

Availability Zones - dat sem obrazek availability zon a vysvetlit!

Resource Groups - dat sem obrazek jak to jde od management group do rg

Azure Subscription - Subscription is a billing unit
Users have access to one or more subscriptions, with different roles

All resources consumed by a subscription will be billed to the owner

Can be used to organize resources into completely distinct accounts

Dat sem obrazek s accounty a subskripcemi

Management groups - dat sem obrazek MM

Azure Resource Manager (ARM) - vysvetlit to je a obrazek kdyztak

Azure resources - instances of services that you create, that are yours to use

### Core resources in Azure

- compute services
- networking services
- storage services
- database services
- azure marketplace

#### Compute services
- VM - full control over it, as if it was your machine
- app services(web apps)
- ACI
- AKS

Web Apps
Give your code and configuration to Azure, and they will run it
Promise of performance but no access to hardware
Platform as a Service (PaaS)

*Containers*
Containers contain everything the app needs to run in a “container image”
Fastest and easiest to deploy
Azure Container Instance (ACI) - single instance, quickest way to deploy a
container
Azure Kubernetes Service (AKS) - runs on a cluster of servers, enterprise-grade

### Networking services
* virtual networks
* VPN gateway
* vnet peering
* express route

Types of Networking Services
● Connectivity Services
● Protection Services
● Delivery Services
● Monitoring Services

Connectivity
Virtual Network - emulating a physical network
Microsoft Global Network already exists, so a virtual network is just software
configuration
Virtual Private Network (VPN) - connecting two networks as if they were on the
same network, uses a Network Gateway
ExpressRoute - high-speed private connection to Azure

Protection - Security Section of the Course
DDos Protection - Distributed Denial of Service attack protection
Azure Firewall
Network Security Groups
Private Link

Delivery - Not on the Exam
Load Balancer - distribute traffic evenly between multiple backend servers
Application Gateway - a higher-level of load balancer with an optional firewall
Content Delivery Network (CDN) - stores common static files on the edge, closer
to the users for (perceived) improved performance
Azure Front Door Service - a load balancer, CDN and firewall all-in-one

Monitoring - Management Tools Section of the
Course
Network Watcher
ExpressRoute Monitor
Azure Monitor

Storage Services Covered
Container (Blob) Storage
Disk Storage
File Storage
Storage Tiers

Container (Blob) and File Storage
The Azure Storage account
General Purpose v2 (gpv2) is the most common type
Blobs, Tables *, Queues *, Files

Many, Many Options
Access tiers - Hot, Cool, Archive
Performance ties - Standard or Premium
Location
Redundancy / Replication
Failover options

Disk Storage
Azure Virtual Machine Disks
Managed Disks
Reserve capacity in advance
Optimized to virtual hard disks

Database Services Covered
Cosmos DB
Azure SQL Database
Azure Database for MySQL
Azure Database for PostgreSQL
SQL Managed Instance

Cosmos DB
Extremely fast storage
Designed for modern applications such as mobile video games, social networks,
and things requiring thousands of global replication
NoSQL Storage
Multi-modal
Supports many open-source APIs and protocols

Azure SQL Database
Runs on the SQL Server engine underneath
Relational DB
Database as a service
Easy to replicate
Easy to scale
Easy to migrate from SQL Server on-prem

Azure Database for MySQL
Managed MySQL database
Common open-source DB
Makes migration to the cloud easier if you rely on this one
Wordpress uses it

Azure Database for PostgreSQL
Managed PostgreSQL database
Open-source DB
Has better support for clusters and more complex server setups
Makes migration to the cloud easier if you rely on this one

SQL Managed Instance
Most compatible with existing SQL Server
Minimal code changes
Fully managed by Azure
Always up-to-date



### Describe Core Solutions and Management Tools (10-15%) - stranka 134
Internet of Things (IoT)
IoT Hub
IoT Central
Azure Sphere - A platform designed to work with connected devices

Big Data and Analytics
Azure Synapse Analytics
(formerly SQL Data Warehouse)
HDInsight
Azure Databricks

Artificial Intelligence (AI)
Azure Machine Learning
Cognitive Services
Azure Bot Service

Serverless
Azure Functions
Logic Apps
Event grid

DevOps Solutions
Azure DevOps
GitHub
GitHub Actions
Azure DevTest Labs

### Azure Tools
Azure CLI
PowerShell
Azure Portal
Azure Cloud Shell
Azure Mobile App

### Azure Advisor

### ARM Templates
The deployment and management service for Azure
Management layer that allows you to create, update, and delete resources called
“deployments”
All actions that you take to manage your Azure resources goes through the ARM
layer

### Azure Monitor

### Azure Service Health


## Describe General and Network Security Features (10-15%)

### Azure Security Center
Azure Security Center
Unified infrastructure security management system that monitors and protects
your systems inside and outside of Azure
● Strengthen security
● Protect against threats
● Get secure faster

### Key Vault
Central, secure repository for
your secrets, certificates and
keys

### Azure Sentinel
Centralizes all the log files from various resources
Analyzes them to detect threats
Allows you to run queries on those logs yourself
Investigate an incident
Orchestration and automation to fix the issues

### Azure Dedicated Hosts

Defense in Depth
Security Layers
● Data - i.e. virtual network endpoint
● Application - i.e. API Management
● Compute - i.e. Limit Remote Desktop access, Windows Update
● Network - i.e. NSG, use of subnets, deny by default
● Perimeter - i.e. DDoS, firewalls
● Identity & access - i.e. Azure AD
● Physical - i.e. Door locks and key cards

NSG

Firewall

Azure DDoS Protection


## Describe Identity, Governance,Privacy, and Compliance Feature (20-25%)

In computing,
“identity” is a
representation of a
person, application
or device

Azure Active Directory
(Azure AD or AAD)

Azure Active Directory
is not the same as
Active Directory

Traditional AD does
not work with
Internet protocols

Azure AD provides
“identity as a
service”

SAML
OpenID
WS Federation

Authentication is a user
proving who they are -
user id and password

Authorization is ensuring
that a user is permitted to
perform an action

RBAC
Microsoft’s
preferred solution
for access control

Create roles that
represent the
common tasks of
the job

Locks
Read Only
Can Not Delete

Using RBAC, you
can restrict who
has access to locks

Resource tags
Helps with billing
and support issues

Azure policy

Azure blueprints
Azure Subscription
templates with
Roles and Policies
already defined


Cloud Adoption Framework for Azure
Set of
documentation,
guidance, tools

Best practices for
succeeding in the
cloud


### Core Tenets of Security, Privacy and Compliance
Azure: Trusted Cloud
● Security
● Privacy
● Compliance
● Resiliency
● Intellectual Property (IP) protection

Security
● Azure is built with security in mind
● Azure delivers tools and technologies to help organizations protect
applications and data
● Azure uses encryption
● Azure offers advanced tools to detect and defend against security threats

Privacy
● You own all your data in Azure
● Microsoft will not mine your data or use it for marketing
● You control where the data is located and who has access
● You can access your own data at any time for any reason
● Microsoft follows a specific policy for government and law enforcement
requests
● Microsoft follows a specific policy to remove data if you
discontinue using their service

Compliance
Microsoft follows international standards and helps customers to follow those
standards too if they wish
Azure has more than 90 compliance certifications
Azure follows more than 50 regional standards
Azure can help with standards in more than 35 industries like health care,
government, finance, etc.

Reliability and Resiliency
● High availability
● Disaster recovery
● Backup

Protecting IP
You can build your solutions on top of Azure’s products and services
Azure offers specific protections against frivolous infringement claims
See: Azure IP Advantage and Shared Innovation Initiative

Microsoft Privacy Statement - privacy.microsoft.com

Trust center - https://www.microsoft.com/en-us/trustcenter/cloudservices/azure


Compliance terms such as GDPR,ISO and NIST
Many different
standards for
technology across
the world

Azure Sovereign Regions
For US government
agencies - federal,
state and local

Different URLs for
connecting to
storage, functions,
etc.

azure china

### Describe Azure cost management and Service Level Agreements (10-15%)

Factors affecting costs - Different services
are billed based on
different factors

Free services
Resource groups
Virtual network (up to 50)
Load balancer (basic)
Azure Active Directory (basic)
Network security groups
Free-tier web apps (up to 10)

Pay per usage
(consumption
model)

Opportunity for cost savings
Azure Functions:
● 1 million executions free per month
● $0.20 per million executions
● Cheapest virtual machine is $20 per month

Pay per usage services
Functions
Logic Apps
Storage (pay per GB)
Outbound bandwidth
Cognitive Services API

Pay for time (per second) - Per second billing
means billing stops
when the VM is
stopped *

Stability in pricing
Pay a fixed price per month for computing power or storage capacity
Whether you use it or not
Discounts for 1-year or 3-year commitment in VM (Reserved Instances)
Multi-tenant or isolated environment

Pay for bandwidth
- First 5 GB is free
- Inbound data is free

Bandwidth costs
Outbound data, $0.05 to $0.087 / GB for Zone 1 (NA and EU w/o Germany)
Outbound data, $0.057 to $0.10 / GB for DE Zone 1 (Germany)
Outbound data, $0.08 to $0.12 / GB for Zone 2 (Asia, Africa and Oceania)
Outbound data, $0.16 to $0.181 / GB for Zone 3 (Brazil)
(Availability zone pricing is different)

Best practices for minimizing Azure costs
- Azure Advisor cost tab
- Auto shutdown on
dev/qa resources
- Utilize cool/archive storage where possible
- - Reserved instances
- Configure alerts
when billing
exceeds an
expected level
- Use Policy to
restrict access to
certain expensive
resources
- Auto scaling
resources
- Downsize when
resources
over-provisioned
- Ensure every
resource has an
owner (tags)
- Spot Pricing

Pricing calculator

Configurable Options
Region
Tier
Subscription Type
Support Options
Dev/Test Pricing

Total Cost of Ownership (TCO)
calculator
Other costs
● Electricity
● Cooling
● Internet connectivity
● Rack space
● Setup labor
● Maintenance labor
● Backup

Azure Cost Management

Service Level Agreement (SLA) - https://azure.microsoft.com/en-ca/support/legal/sla/

Preview features

Public and Private Preview

General Availability (GA)