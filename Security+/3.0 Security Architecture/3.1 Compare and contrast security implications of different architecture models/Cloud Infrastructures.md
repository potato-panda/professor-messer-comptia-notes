# Cloud responsibility matrix
### IaaS, PaaS, SaaS, etc.
- who is responsible for security?
### Security should be well documented
- most cloud providers provide a matrix of responsibilities
- everyone knows up front
### These responsibilities can vary
- with different cloud providers
- contractual agreements
### Example
![[Pasted image 20240607112611.png]]
# Hybrid considerations
### Hybrid cloud
- more than 1 public/private cloud
- adds additional complexity
### Network protection mismatches
- auth across platforms
- firewall configs
- server settings
### Different security settings
- logs are diverse and cloud-specific
### Data leakage
- data is shored over the public Internet
# Third-party vendors in the cloud
### You, the cloud provider, and third parties
- infra tech
- cloud-based apps
### Ongoing vendor risk assessment
- part of overall vendor risk mgnt policy
### Include third-party impact for incident response
- everyone is part of the process
### Constant monitoring
- watch for changes and unusual activity
# Infrastructure as code
### Describe an infra
- define servers, networks, and apps as code
### Modify the infra and create versions
- same way you version app code
### Use that code to build other app instances
- build same way every time based on code
### An important concept for cloud computing
- build a perfect version every time
# Serverless architecture
### Function as a Service (FaaS)
- apps are separated into individual, autonomous functions
- remove the OS from equation
### Dev still creates the server-side logic
- runs in a stateless compute container
### May be event triggered and ephemeral
- may only run once for one event
### Managed by a third-party
- all OS security concerns are at the third-party
# Microservices and APIs
### Monolithic apps
- one big app that does everything
### App contains all decision making processes
- UI
- business logic
- data input and output
### Code challenges
- large codebase
- change control challenges
### APIs
- application programming interfaces
### API is the "glue" for the microservices
- work together to act as the app
### Scalable
- scale just the microservices you need
### Resilient
- outages are contained
### Security and compliance
- containment is built-in