#### Overview of Cloud Models

1) Infrastructure-as-a-Service(Iaas)

Virtul machines,networking,load balancer,firewalls

2) Platform-as-a-Service(Paas)

Upload code packages and have them run, without access to the hardware

3) Software-as-a-Service(SaaS)

Access to configuration only

###### Shared Responsibility Model

| Responsibility                        | SAAS    | Paas    | laas | On-Prem | By                                        |
|---------------------------------------|---------|---------|------|---------|-------------------------------------------|
| Information and data                  | C       | C       | C    | C       | Responsibilty always retained by Customer |
| Devices(Mobile and Pcs)               | C       | C       | C    | C       |                                           |
| Accounts and Identities               | C       | C       | C    | C       |                                           |
| Identity and directory infrastructure | M and C | M and C | C    | C       | Responsibilty Varies By service Type      |
| Application                           | M       | M and C | C    | C       |                                           |
| Network Controls                      | M       | M and C | C    | C       |                                           |
| Operating System                      | M       | M       | C    | C       |                                           |
| Physical hosts                        | M       | M       | M    | C       | Responsibilty Transfers to Cloud Provider |
| Physical network                      | M       | M       | M    | C       |                                           |
| Physical datecenter                   | M       | M       | M    | C       |                                           |
|                                       |         |         |      |         |                                           |
|                                       |         |         |      |         |                                           |
| Microsoft : M and Customer  C         |         |         |      |         |                                           |


##### something as as service

- the idea ia that we don't own that thing 
- someone else owns it and you benefit from it - "as a service"
- you are not in control of how it's delivered (for the most part)
- Pay as you go 

Example:
Cooking at home -> Cooking as a Service (restaurant)
Driving your own car -> Driving as a Service(taxi)

1) Software as a Service

- we don't control the servers (or even know what they are)
- we don't control the software (or even know what version number is running)
- we control the data and settings only
- it stands alone as a useful product ; doesn't require something else to be useful
  
Example : Microsoft office 365(SharePoint,Outlook,word,Excel etc)

2) Platform as a Service

- we don't control the servers (but we might be able to pay more for performance)
- we control data and settings
- Often it's programmable and we can upload our own code
- Provides useful features above the raw storage or compute uderneath
- It's a platform that we need to build upon to  be useful

Example : App Services - Platform as a Service
Azure SQL Database - Platform as a Service

3) Infrastrcuture as a Service

- we can control the virtual hardware
- it's a virtual imitation of a real piece of a network
- Falls into 3 categories - compute , networking and storage
  
Example :
Virtual Machines - Infrastructure as a Service
Azure Storage - Infrastructure as a Service
Load Balancer - Infrastructure as a Service

#### Serverless Model

- There are still servers .. we just don't ever have to deal with them
- Even less access to the server than PaaS
- Even with Pass we have to chosse an App Service Plan
- With Paas , Scaling is our responsibility
- Serverless means not worrying about choosing the right plan
- Serverless means not worrying about scaling
- Serverless means we might pay $0 if we don't use the service
  
Azure Serverless Offers

Compute - Azure Functions
Compute - Serverless Kubernetes (Virtual Nodes w/ ACI)
Database - Azure SQL Database Serverless
Database - Cosmos DB Serverless(preview)

#### Cloud Types

1) Public Cloud

Azure owns the hardware on their network and infrastructure 


