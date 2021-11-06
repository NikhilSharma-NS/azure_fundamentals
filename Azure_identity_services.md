#### Azure_identity_services


- What is Identity

In Computing, "identity" is a representation of a person , application or device

- Usually requires a password a secret key or certificate to prove
  
- Many applications require us to log in to use some of its functionality 
  
Client-Server Model

```

Client APP 
Web Browser      -> User Name and Password  ->   Server Web Site
Mobile APP                                            |
                                                     DB
```
- Traditionally companies have written their own code to handle above part
  
- Some of the more famous hacks have been on custom created identity systems

Hacks

- Some companies were storing the password in plain text
- Some companies were using a simple , reversible hash algo (MD5)
- Some companies were storing the "salt" along with the data
- Not enforcing password change policies
- Not enforcing password complexity policies
  
- Azure Provides an Identity Management System based on their popular Active Directory

1) Azure Active Directory (Azure AD or AAD)

- Azure  Active Directory is not same as Active Directory
- Traditional AD does not work with Internel protocols
- Azure AD provides "identity as a Service"
- Instead of having to write code to handle users , password , password reset
  
AAD Model
```
                                                   (a)
                                           Identity Provider
          UserId,password(b->a)                                  Trust Key (a---c)
          Signed token(a->b)

   (b)
Client App
Browser                              -> Signed Token(b->c)     ->            Server    (c)
Mobile APP                                                                  Web Server


```

other open source example -> SAML OpenID WS Federation 


##### Benefits of Azure AD

1) Security
   
2) Reduces development time and easier support
   
3) Multifactor authentication user access reviews 
   
4) Just in time elevation of privileges and conditional access and all of these

5)(Centralized Administration) we will get centralized dashboard where we can get logging and reporting and grant people access and take their access away

6) Azure AD integration with windows active Directory Inside of our Coporate Env (Only one user id and password , Single Sign-On)
   
7)  Azure AD Integration with Other Azure services like : databases using their windows user id and password as well and storage account and databases
   
More on 

8) Azure AD Microsoft's preferred solution for identity Management
   
9) Azure AD Powers Other Microsoft Services

Azure,Skype,Outlook,OneDrive,Xbox,Office 365,Teams,SharePoint,PowerBI

10) Compelte solution for managing users,group,roles
    
11)  Conitional Access
User A attempts to log in to the app from within the company office, as she does every day
User B attempts to log in to the app for first time in 4 months
Admin C attempts to log in to the app from their phone 
Admin D attempts to logn in to the app from location 1200 miles from the office

so we can treat some access attempts as routine and some as not normal

Signal 
Decision
Enforcement
   
##### The Difference between Authentication and Authorization

1) Authentication is a user providing who they are - user id and password
   
2) Authorization is ensuring that a user is permitted to perform an action

##### Azure Multi-Factor Authentication
   
1) Require 2 or more pieces of evidence (factors) in order to log in
   
2) 3 Factor that we can use
Somethings we know - password
somethings we have - Mobile, access to email account
something we are - Fingerprint

3) Password could be 1 piece of evidence and second piece of evidence is required
  a unique time-limited code sent to us ( we have google auth app)





