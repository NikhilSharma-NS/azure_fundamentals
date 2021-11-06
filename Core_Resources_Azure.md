#### Core Resources in Azure

Getting Deep into Technical

- Compute services
- Networking services
- Storage services
- Database services
- Azure marketplace
  
1) Compute Services
   
- Virtual Machine
- App Services
- Azure Container Instance 
- Azure Kubernetes Service
- Windows Virtual Desktop
  
Compute - Executing code in the cloud

1.1) Virtual Machine

- Infrastructure as as service - Iaas
- Take an existing machine from our env into the cloud - a copy
- Windows or Linux os - several of each
- A "slice" of a physical machine shared with other customers
- Full control over it, as if it was your machine
- Over 200 to choose from
- Number of CPU cores,CPU Speed , RAM size , temporary disk size , IOPS etc

1.2) App Services

- A new paradigm for running code in the cloud
- Give your code and configuration to Azure annd they will run it
- promise of performance but no access to hardware
- Platform as a Service - PaaS
  
1.3) Containers

- Another paradigm for running code in the cloud
- Containers contain everything the app needs to run in a "container image"
- Fastest and easiest to deploy
- Azure container service - single instance , quickest way to deploy a container
- Azure Kubernetes Service - runs on a cluster of services enterprise-grade

1.4) Windows Virtual Desktop

- Desktop version of windows that runs in the cloud
- Software installed, your files - avaliable from anywhere
- Can even see your desktop on iOS and android or from any web browser
- Runs on azure
  

2) Networking Services
   
- Virtual Networks
- VPN Gateway
- VNet Peering
- ExpressRoute
  

Types of  Networking Services

- Connectivity Services
- Protection Services
- Delivery Services
- Monitoring Services
  
2.1) Connectivity Services

Virtual Networks - Emulating a physical network

Microsoft global Network alraedy exists, so a virtual network is just software configuration

Virtual Private Network - Connecting 2 network as if they were on the same network , uses a Network Gateway

ExpressRoute -  High Speed private connection to Azure

2.2) Protection Services

- DDos Protection - Distributed denial of service attack protection
- Azure Firewall
- Network Security Groups
- Private Link

2.3) Delivery Services

- Load Balancer - distribute traffic evenly between multiple backend servers
- Application Gateway - A higher-level of load balancer with an optional firewall
- Content Delivery Network - Stores common static files on the edge , closer to the user
  for(perceived) improved performance
- Azure front Door Service - A load balancer,CDN and firewall all-in-one


2.4) Monitoring Services

- Network Watcher
- ExpressRoute Monitor
- Azure Monitor
  

3) Storage Services

- Container(Blob) Storage
- Disk Storage
- File Storage
- Storage Tiers
  
Storage - one of the foundationla technologies on which much is built

3.1) Container(Blob) and File Storage

- The Azure Storage account
- General Purpose v2(gpv2) is the most Common Type
- Blobs,Tables,Queues,Files
- Azure Data Lake Storage gen2 is the cheapest type of storage
- Pay per GB (~1.8 cents per GB)
- Access tiers - Hot,Cool,Archive
- Performance tiers - Standard or Premium
- Location
- Redundancy / Replication
- Failover options
  
3.2) Disk Storage

- Azure Virtual Machine disks
- managed disks
- Reserve capacity in advance
- Optimized to virtual hard disks
  
4) Database Services

- Cosmos DB
- Azure SQL Database
- Azure Database for MYSQL
- Azure Database for PostgresSQL
- SQL Managed Instance
  
Most sophisticated applications have some types of database

4.1) Cosmos DB 

- Extremely Fast storage
- Designed for modern application such as mobile video games , social network and things requring thousand of global replication
- NoSQL Storage
- Multi-modal
- Supports many open-source APIs and protocols
  
4.2) Azure SQL Database

- Runs on the SQL server engine underneath
- Relational DB
- Database as as service
- Easy to replicate
- Easy to scale
- Easy to migrate from SQL Server on-prem

4.3) Azure Database for MYSQL

- Managed MYSQL database
- Common open-source DB
- Makes migration to the cloud easier if you rely on this one
- Wordpress uses it
  
4.4) Azure Database for PostgreSQL

- Managed PostgreSQL database
- Open-source DB
- Has better support for clusters and more complex server setups
- Makes migration to the cloud easier if you reply on this one
  
4.5) Azure Managed Instance

- Most Compatible with existing SQL server
- Minimal code changes
- Fully managed by Azure
- Always up-to-date
  


5 ) Azure Marketplace 

Many types of services not just provided by Microsoft




