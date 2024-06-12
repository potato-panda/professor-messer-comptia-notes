### Identification
- this is who you claim to be
- usually your username
### Authentication
- prove you are who you say you are
- password and other authentication factors
### Authorization
- based on you identification and authentication, what access do you have?
### Accounting
- resourced sued: login time, data send and received, logout time
# Authenticating systems
### You have to manage many devices
- often device that you'll never physically see
### A system can't type a password
- and you may not want to store one
### How can you truly authenticate a device?
- put a digitally signed certificate on the device
### Other business processes rely on the certificate
- access to the VPN from authorized devices
- management software can validate the end device
# Certificate authentication
### An organization has a trusted Certificate Authority(CA)
- most orgs maintain their own CAs
### The org creates a cert for a device
- and digitally signs the cert with the org's CA
### The cert can now be included on a device as an auth factor
- the CA's digital sig is used to validate the cert
# Cert-based authentication
![[Pasted image 20240604165741.png]]
![[Pasted image 20240604165758.png]]
![[Pasted image 20240604170036.png]]
> Compare if signed by CA

# Authorization models
### The user or device has now authenticated
- to what do they now have access?
- time to apply an authz model
### Users and services -> data and applications
- associating individual users to access rights does not scale
### Put an authz model in the middle
- define by Roles, Organizations, Attributes, etc...
# No authz model
### A simple relationship
- user -> resource
### Some issues with this method
- difficult to understand why an authz may exist
- does not scale
![[Pasted image 20240604173009.png]]
# Using an authz model
### Add an abstraction
- reduce complexity
- create a clear relationship between users and the resource
### Administration is streamlined
- easy to understand the authzs
- support any number of users or resources
