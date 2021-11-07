#### Overview of Azure Authentication and RBAC

- Microsoft's preferred solution for access control
- Create roles that represent the common tasks of the job
Accountant
Developer
Business Lead
- Assign granular permissions to that role
- Assign users to that role
- Do not assign granular permissions to an individual
Reader
Contributor
Owner

##### Locks

- Read only can Not Delete
- Using RBAC, we can restrict who has access to locks

##### Resource Tags

- Can add metadata to Azure resources
- Helps with billing and support issues
  
##### Azure Policy

1) Governance

- Who goven or set the rules or policies across a larger group of people
- Create Rules across all of our azure resources
- Evaluate compliance to those rules

Example of built-in Policies

- Require SQL Server 12.0
- Allowed Storage Account SKUs
- Allowed Locations
- Allowed Virtual Machine SKUs
- Apply tags and its default value
- Not allowed resource types

- We can create custom policies using JSON definition
  
2) Azure Blueprints
   
- Azure Subscription templates with Roles and Policies already defined
- It is combined set of policies and roles that we can use

3) Cloud Adoption framework for Azure

Cloud Adoption is set of documentation guidance,tools
In there contains microsoft's learnings,their beet practices for companies and organizations who are looking ot make this move.

```
Define   -> Plan -> Ready -> Adopt(migrate,Innovate) -> 
Strategy 

        (Govern              Manage)
```

Define Strategy -> Understand motivations Business outcomes , Business justifications , Prioritize project
Plan -> Digital estate Initial organization alignment Skills readliness plan and Cloud adoption plan
Ready -> Azure setup guide First landing zone Expand the landing zone , Best practices
Adopt -> 
 Migrate-> Azure migration guide,Migration scenarious , Best practices,Process Improvement
 Innovate -> Azure innovation guide,innovation scenarious, Best practices, Process Improvement

Govern -> Methodology,Benchmark,Initials best practise,Governance maturity
Manage -> Business commitments Opearations baseline , Opearations maturity