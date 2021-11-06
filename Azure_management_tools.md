1) Azure Management Tools 

Azure CLI
PowerShell
Azure Portal
Azure Cloud Shell
Azure Mobile App

1.1) Azure Mobile App

monitor the health and status of resources from our phone
Run Commands,start,stop and restart servers

2) Azure Advisor - Run and analyze our actual usage of azure and make suggestions to us

High Availability 
Security
Performance
Operational Excellence
Cost

3) Managing Azure with ARM Templates
   
Azure Resource Manager (ARM)

- The deployment and management service for Azure
- Management layer that allows you to create,update and delete resources called deployments
- All actions that we take to manage our Azure resources goes through ARM layer
  
```
Azure-Portal    Azure-Power-Shell     Azure-CLI     Rest-Client

                              SDKs


                     Azure Resource Manager          <-------->      Authentication


 Data          Web         Virtual        Service                 ....Other 
 Store         App         Machine        Management              Service


```


The actual things they are creating are called arm template

4) Azure Monitor
   
- Azure monitor is sort of centralized dashboard for most of our resoures 
  

```                               
                                         Insight    - Application Container VM Monnitoring_solution 
                                         
Application                              Visualize  - Dashbaords  Views Powe BI Wroekbooks
Opearting System        Metrics        
Azure Resources                          Analyze    - Metrics_Analytics Log_Analytics
Azure Subscription      Logs                 
Azure Tenant                             Respond    - Alerts Autoscale
                            
Custome Sources                          Integrate  - Logic_Apps Exports_Apis 




```

5) Azure Service Health

this is where we go to things that affets us
It handles the issues that are across Azure

we can enable the sms or email of the standard alert modes 