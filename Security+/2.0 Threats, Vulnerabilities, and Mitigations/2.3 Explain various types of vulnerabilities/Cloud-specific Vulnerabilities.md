# Security in the cloud
### Cloud adoption has been nearly universal
- it's difficult to find a company NOT using cloud
### We've put sensitive data in the cloud
- attacks would like this data
### We're not putting in the right protections
- 76% of orgs aren't using MFA for mgnt console users
### Simple best practices aren't being used
- 63% of prod code is unpatched
- vulns rated high or critical (CVSS>=7.0)
# Attack the server
### DoS
### Authentication bypass
- take advantage of weak or faulty authn
### Directory traversal
- faulty configs put data at risk
### Remote code execution
- take advantage of unpatched systems
# Attack the app
### Web app attacks have been increased
- Log4j and Spring Cloud Function
- easy to exploit, rewards are extensive
### Cross-site (XSS)
- take advantage of poor input validation
### Out of bounds write
- write to unauthed memory areas
- data corrupted, crashing, code execution
### SQL injection
- get direct access to a db