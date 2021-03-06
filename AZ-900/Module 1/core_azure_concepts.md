### Describe Azure Core Services

- Basic understanding : Azure is cloud computing services which allows its users to run there solution on the remote hardware (Cloud) and solution maybe a website, ML models or bunch of VMs
- Basic services are - Computing Power and Storage, and it follows pay-as-you-go pricing model

- Virtualization : 
    - It refers to removing or separating tight coupling of hardware and OS using Hypervisors

- Azure Services are as follows  :
    Compute - e.g. adding VMs/Container  
    Network - e.g. VPNs adn Load balancing can be one example
    Store - Files, Blobs, Queue and Disks
    Mobile - Build/Deploy/Notifications, usage of cognitive services
    Databases - Open source db tools
    Web - Build/Deploy/Scale web app
    IOT - Connect/Monitor/Manage your IOT asset
    Big Data - Run Analytics on Big Data
    AI - Forecast future, behavioural insights
    DevOps - CI/CD


- Azure subscription can be understood like this 
    - at the top level, we have Azure Account and as we go down Subscription -> Resource group and at the tail it will be resource
    
#### Public, Private and Hybrid 
- Public clouds are Internet facing and are open to everyone's use and hardware of the cloud are managed by the third party
- Organisation have their own cloud and for that they have set up of the hardware resources 
- Hybrid consists of both the types of cloud model. For example - Azure and On-Premise model

### Cloud Computing Advantages

#### High Availability
- No apparent downtime based on the SLA

#### Scalability 
- Vertical : Adding more RAMs or CPUs to VMs
- Horizontal : adding instances of the resources

#### Elasticity 
- auto-scalable environment

#### Agility 
- Building and deploying easily

#### Geo-distribution & Disaster Recovery
- Customer will always have the best performance
- Back and data replication

#### Capital & Operational Expenditure
- Upfront cost for the hardware or the setup
- Other is money spent on the maintenance, services and product

### Computing Models
#### IAAS 
- Setting up hardware is already done by the Cloud Provider and then tenant is in charge configuring OS and Network
- Benefits 
    - No CapEx
    - Agility
    - Management
    - Consumption based model
    - Skills - Making the workload secure and safe
    - Cloud benefits
    - Flexibility 
#### PAAS
- Cloud provides manages the configuration and networking resources and cloud tenant deploy there application to the hosting environment.
- Same benefits as IAAS, however focuses more on the Productivity
#### SAAS
- Microsoft Office 365, everything is already deployed to cloud.
- More for the software usage 
#### Serverless computing
- Enables developers to focus more on the application development, rest of the configuration are already taken care by the cloud provider

### Azure Terms
#### Resource group 
- Resources are contained into groups that acts as a logical container. It can be understood as **Space** in Cloud Foundry Environment
#### Management Group
- Manages access, policy and compliance over multiple subscription
#### Azure Resource Manager
- It is the deployment and management service for Azure
- Describe what you want to deploy
- Role based access control 
- Tags can be used to organize the resources

### Azure Regions
- Azure organizes datacenters into regions
#### Regions
- Geographical area/plane that contains multiple datacenter that are nearby and connected together with low-latency network
- **Region Pair** makes Azure more reliable in the case of disaster. Other region can be used if primary region is down
#### Availability Zone
- Physically separate data centers within an Azure Region
- Zonal Services are specific to a particular zone eg. VMs, Managed Disk
- Zonal redundant services replicates automatically across zone eg. SQL Databases
- Availability zones are connected through high-speed, private fiber-optic networks.
#### Azure Region Pair
- Each Azure region is always paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. 
- This approach allows for the replication of resources (such as VM storage) across a geography that helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect both regions at once.
- If a region in a pair was affected by a natural disaster, for instance, services would automatically failover to the other region in its region pair.
#### Azure Subscription
- Defines boundaries around Azure products, Services and Resources
- Billing Boundaries
    - Azure generates separate billing reports and invoices for each subscription
- Access based
    - Specific subscription for each department
        
