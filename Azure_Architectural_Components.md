### 1) Core Azure Architectural Components
   
#### 1.1) Regions

60+ regions supported by azure

#### 1.2) Region Pairs

each regiob has one other region which is treated as it's pair
almost always in the same geography - data storage laws
The data connectionn between region pairs is the highest speed avaliable
Software rollouts are deployed to one region of a pair and the other is not touched
If multiple regions go down , one region of each pair is treadred as a priority

```

Example:
Canada -> Canada central    -     Canada East
Europe -> North  Europe     -     West Europe
USA    -> East US           -     West US
USA    -> East US 2         -     Central US
USA    -> North Central US  -     South Central US
Brazil -> Brazil South      -     South Central US

```
#### 1.3) Availability Zones

```
           
Availability Zone 1                       Availability Zone 2



                     Availability Zone 3


```
#### 1.4) Resource Group

```
Management Group

Subscriptions

Resource groups

Resources

```

#### 1.5) Azure Subscriptions

Subscription is a billing unit 
Users have access to one or more Subscriptions , with different roles 
All resources consumed by a Subscription will be billed to the owner
Can be used to organize resources into completely distinct accounts

```
                                           Microsoft Azure Account


HR Subscription                           Finance Subscription                             Marketing Subscription


Azure Automation                          Visual Studio Online                             Service Bus
cloud service                             Cloud Service                                    Cloud Service
VM                                        VM                                               CodePlex
SQL data warehouse                        WebApp                                           RemoteApp
Traffic Manager                           Traffic Manager                                  Traffic Manager
Service Fabric                            Site Recovery                                    StorSimple
```

#### 1.6) Management Groups

```
                                             Contoso Root Group

      Marketing Team Management  Group                                IT Team Management Group
 


Dev/Test                             Infra Team Management Group                         App Team Management Group 
Subscriptions


                               EA Subscriptions     EA Subscriptions                         Pay-As-you-Go Subscriptions
```

#### 1.7) Azure Resource Manager (ARM)

Portal 
Command Line
Azure Resource Manager API
Azure Provider Contract

#### 1.8) Azure Resources

- Instance of services that you create,that are yours to use




