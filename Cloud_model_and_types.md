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