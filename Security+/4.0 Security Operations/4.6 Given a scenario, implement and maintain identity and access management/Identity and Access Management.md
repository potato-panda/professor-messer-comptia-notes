# IAM
### Apps are available anywhere
- desktop, browser, mobile device, etc.
### Data can be located anywhere
- cloud storage, private data centers, etc.
### Many diff app users
- employees, vendors, contractors, customers
### Give the right permissions to the right people at the right time
- prevent unauthd access
### Identify lifecycle management
- every entity (human and non-human) gets a digital identity
### Access control
- an entity only gets access to what they need
### Authn and authz
- entities must prove they are who they claim to be 
### Identity governance
- track an entity's resource access
- may be regulatory requirement
# Provisioning/de-provisioning user accounts
### User account creation process
- and account removal process
### Provisioning and de-provisioning occurs for certain events
- hiring, transfers, promotions, job separation
### Account details
- name, attributes, group permissions, other permissions
### An important part of the IAM process
- an initial checkpoint to limit access
- nobody gets admin access
# Permission assignments
### Each entity gets limited permissions
- just enough to do job
- group assignments are common
### Storage and files can be private to that user
- even if another person is using the same computer
### No privileged access to the OS
- specifically not allowed on a user account
# Identity proofing
### I could be anyone
- IAM process should confirm who they are
### Resolution
- who the system thinks you are
### Validation
- gathering info from the user (password, security Qs, etc.)
### Verification/Attestation
- passport, in-person meeting, etc.
- automated verification is also an option
# Gaining access
![[Pasted image 20240610161831.png]]
# Single Sign-on (SSO)
### Provide creds one time
- get access to all available or assigned resources
- no additional authn required
### Usually limited by time
- a SSO auth can work for 24 hours
- authn again after expires
### Underlying authn infra must support SSO
- not always an option
# [[Authentication Methods#LDAP (Lightweight Directory Access Protocol)|LDAP]]
# X.500 Distinguished Names
### *attribute=value* pairs
### Most specifically attribute is listed first
- this may be similar to the way you already think
![[Pasted image 20240610162158.png]]
# X.500 Directory Information Tree
### Hierarchical structure
- builds a tree
### Container objects
- country, org, organizational units
### Leaf objects
- users, computers, printers, files
![[Pasted image 20240610162311.png]]
# Security Assertion Markup Language (SAML)
### Open standard for authz and authz
- you can auth through a third-party to gain access
- one standard does it all, sort of
### Not originally designed for mobile apps
- this has been SAML's largest roadblock
# The SAML auth flow
![[Pasted image 20240610162451.png]]
# OAuth
### Auth framework
- determines what resources a user will be able to access
### Created by Twitter, Google, and many others
- significant industry support
### Not an auth protocol
- OpenID Connect handles the single sign-on auth
- OAuth provides authz between apps
# Federation
### Provide network access to others
- not just employees - partners, suppliers, customers, etc.
- provides SSO and more
### Third-parties can establish a federated network
- auth and authz between the two orgs
- login with Facebook creds
### Third-parties must establish a trust relationship
- and degree of trust
# Interoperability
### Many diff ways to comm with an authn server
- more than a simple login process
### Often determined by what is at hand
- VPN concentrator can talk to a LDAP server
### A new app uses OAuth
- need to allow authn API access
### Interop is dependent on the env
- often part of much larger IAM strategy