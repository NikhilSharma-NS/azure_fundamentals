Managing Azure Costs


1) Factors affecting costs
- Different services are billed based on different factors
- Free Services
  Resource Groups
  Virtual Netwrok (up to 50)
  Load Balancer (basic)
  Azure Active Directory (basic)
  Network Security Groups
  Free-Tier Web Apps(up to 10)
- Pay per usage(consumption model)
- Oportunity for cost savings
  Azure Functions
   - 1 million executions free per month
   - $0.20 per million executions
   - Cheapest virtual machine is $20 per month
- Pay per usage services
  - functions
  - Logic Apps
  - Storage (pay per GB)
  - Outbound bandwidth
  - Cognitive Services API
- Pay for time (per second)
   - per second billing means billing stops when the VM is stopped
- Stability in Pricing 
   - Pay a fixed price per month for computing power or storage capacity
   - Whether we us eit or not
   - Discounts for 1 year or 3 year commitment in VM (reserved instance)
   - Multi-tenant or isnlated environment
- Pay for Bandwidth
   - First 5GB is free
   - Inbound data is free
- Bandwidth Costs
   - Outbound data $0.05 to $0.087 / GB for Zone1(NA and EU w/o Germany)
   - Outbound data $0.057 to $0.10 / GB for DE Zone1(Germany)
   - Outbound data $0.08 to $0.12 / GB for Zone2(Asia,Africa and Oceania)
   - Outbound data $0.16 to $0.181 / GB for Zone3(Brazil)
   - Availability zone pricing is different
- 1 PB of data transfer = $52,000
  
#### Best Practices for minimizing Azure Costs

- Azure Advisor cost tab
- Auto shutdown on dev/qa resources
- Utilize cool/archive storage where possible
- Reserved Instances
- Configure alerts when billing exceeds an expected level
- Use Policy to restrict access to certain expensive resources
- Auto Scaling Resources
- Downsize when resources over-provisioned
- Ensure every resource has an owner(tags)
  
#### Spot Pricing

- Ability to use virtual machine when nobody is using it for a discounted price
- But When someone needs to use it we get kicked off
  
#### Pricing Calculator

- https://azure.microsoft.com/en-ca/pricing/calculator/
- Estimate are hard to make 100% accurate
- Configurable Options
  - region
  - tier
  - Subscription type
  - Support options
  - Dev/Test pricing
- Export and Share the estimate
- Total Cost Ownership(TCO) calculator
  - The cost of a server is more than just the cost of the hardware
  - Other Costs
    - Electricity
    - Cooling
    - Internet Connectivity
    - Rack Space
    - Setup Labor
    - Maintenance labor
    - Backup
  - https://azure.microsoft.com/en-ca/pricing/tco/calculator/

#### Azure Cost Management

- Another free tool inside Azure to analyze spending
- Analyze Spending over time
- Tracking anainst Budgets
- Schedule reports
  


