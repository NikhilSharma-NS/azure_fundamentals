#### Azure Network Security

Defense in depth

1) Security Layer

Data - i.e. Virtual Network endpoint
Application - i.e. API Management
Compute - i.e. Limit Remote Desktop access, Windows Update
Network - i.e. NSG, use of subnets, deny by default
Perimeter - i.e. DDos, firewalls
Identity & Access - i.e. Azure AD
Physical - i.e. Door locks and key cards


| Identity and   Access          	| Apps & Data Security   	| Network Security     	| Threat Protection               	| Security Management         	|
|--------------------------------	|------------------------	|----------------------	|---------------------------------	|-----------------------------	|
| Role Based Access              	| Encryption             	| DDOS Protection      	| Antimalware                     	| Log Management              	|
| Multifactor Authentication     	| Confidential Computing 	| NG Firewall          	| AI-Based Detection and Response 	| Security Posture Assessment 	|
| Central Identity Management    	| Key Management         	| Web App Firewall     	| Cloud workload Protection       	| Policy and Governance       	|
| Identity Protection            	| Certificate Management 	| Private Connections  	| SQL Threat Protection           	| Regulatory Compliance       	|
| Privileged Identity Management 	| Information Protection 	| Network Segmentation 	| IoT security                    	| SIEM                        	|


1) Network Security Group (NSG)
   
NSG is a very simplistic set of rules but if we set them right

```
------------------------------------------------------------------------------------------------------ 
                                              Internet   
------------------------------------------------------------------------------------------------------Virtual Network
                                         Azure Infrastructure                                           
-------------------------------------------------------------------------------------------------------Virtual Network
        Front end Subnet               public facing load Balancer              NSG                   
                                                                                
                                           Web Server VMS                       DNS
-------------------------------------------------------------------------------------------------------Virtual Network
                                                  |
-------------------------------------------------------------------------------------------------------Virtual Network
        Back endd Subnet               Internal  load Balancer                   NSG                   
                                                                                
                                           Database server VMS                  DC VM
-------------------------------------------------------------------------------------------------------Virtual Network


2) Azure Firewall 

It will analyze traffic which is trying to come in and see if it matches certain known bad patterns so 
hackers are going to try to inject SQL commands into website ot the firewall is going to recognize that there are SQL commands 
into the body og the data and reject the request

--------------------------------------------------------------------------------------------------------------
XSS attack          X                  Application Gateway                Y <-valid request       Site 2 

Valid Request       Y                       WAF                           Y <-valid request       Site 1

SQL Injection       X                      L7 LB
---------------------------------------------------------------------------------------------------------------

3) Azure DDos Protection

| Feature                                                            	| Basic 	| Standard 	|
|--------------------------------------------------------------------	|-------	|----------	|
| Always on monitoring                                               	| Y     	| Y        	|
| Automatic mitigation for L3/L4 attacks                             	| Y     	| Y        	|
| L7 Protection with Application Gateway   Web application firewall  	| Y     	| Y        	|
| Globally Deployed                                                  	| Y     	| Y        	|
| Prtection policies tuned to our Vnet                               	| N     	| Y        	|
| Logging,alerting and telemetry                                     	| N     	| Y        	|
| Resource Cost Scale Protection                                     	| N     	| Y        	|

