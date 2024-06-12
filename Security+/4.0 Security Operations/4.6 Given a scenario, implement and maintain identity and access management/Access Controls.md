### Authz
- process of ensuring only authz rights are exercised
- policy enforcement
- process of determining rights
- policy definition
### Users receive rights based on Access Control models
- different business needs or mission requirements
# [[Mitigation Techniques#Least privilege|Least privilege]]
# Mandatory Access Control (MAC)
### The OS limits the operation on an object
- based on security clearance levels
### Every object gets a label
- confidential, secret, top secret, etc.
### Labelling of objects uses predefined rules
- the admin decides who gets access to what security level
- users cannot change these settings
# Discretionary Access Control (DAC)
### Used in most OS
- a familiar access control model
### Example: You create a spreadsheet
- as owner, you control who has access
- you can modify access at any time
### Very flexible access control
- very weak security
# Role-based access control (RBAC)
### You have a role in your org
- manager, director, team lead, project manager
### Admins provide access based on role of user
- rights gained implicitly instead of explicitly
### In Windows: Use Groups to provide role-based access control
- you are in Shipping and Receiving, so you can use the shipping software
- you are a manager, so you can review shipping logs
# Rule-based access control
### Generic term for following rules
- conditions other than who you are
### Access is determined through system-enforced rules
- sysadmins, not users
### Rule is associated with the object
- system check the ACLs for that object
### Rule examples
- Lab network access only available between 9AM and 5PM
- only Chrome browsers may complete this web form
# Attribute-based access control (ABAC)
### Users can have complex relationships to apps and data
- access may be based on many diff criteria
### ABAC can consider many parameters
- a "next generation" authz model
- aware of context
### Combine and eval multiple parameters
- resource info, IP address, time of day, desired action, relationship to data, etc.
# Time-of-day restrictions
### Almost all security devices include a time-of-day option
- restrict access during certain times or days of week
- usually not the only access control
### Can be difficult to impl
- esp. in a 24hr env
### Time-of-day restrictions
![[Pasted image 20240610172410.png]]
