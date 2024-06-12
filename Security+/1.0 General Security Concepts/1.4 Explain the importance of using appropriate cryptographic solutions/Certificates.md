# Digital certificates
### A public key cert
- binds a public key with a digital signature
- and other details about the keyholder
### A digital signature adds trust
- PKI uses Certificate Authorities for additional trust
- Web of Trust adds other users for additional trust
### Certificate creation can be built into the OS
- part of the Windows Domain services
- many 3rd-party options
# What's in a digital cert?
### X.509
- standard format
### Details
- serial number
- version
- signature algo
- issuer
- name of cert holder
- public key
- extensions
- and more...
# Root of trust
### Everything associate with IT security requires trust
- a foundational characteristic
### How to build trust from something unknown?
- someone/something trustworthy provides their approval
### Refer to the root of trust
- an inherently trusted component
- hardware, software, firmware, or other components
- hardware security module (HSM), secure enclave, certificate authority, etc.
# Certificate Authorities
### You connect to a random website
- do you trust it?
### Need a good way to trust an unknown entity
- use a trusted third-party
- an authority
### Certificate Authority (CA) has digitally signed the website cert
- you trust the CA, therefore you trust the website
- real-time verification
# Third-party certificate authorities
### Built-in to your browser
- any browser
### Purchase your web site certificate
- it will be trusted by everyone's browser
### CA is responsible for vetting the request
- they will confirm the cert owner
- additional verification info may be required by the CA
# Certificate signing request
### Create a key pair, then send the public key to the CA to be signed
- a cert signing request (CSR)
### The CA validates the request
- confirms DNS emails and website ownership
### CA digitally signs the cert
- returns to the applicant
![[Pasted image 20240605152231.png]]
# Private certificate authorities
### You are your own CA
- build it in-house
- your devices must trust the internal CA
### Needed for medium-to-large orgs
- many web servers and privacy requirements
### Impl as part of your overall computing strategy
- Windows Certificate Services, OpenCA
# Self-signed certificates
### Internal certificates don't need to be signed by a public CA
- your company is the only one going to use it
- no need to purchase trust for devices that already trust you
### Build your own CA
- issue your own certs signed by your own CA
### Install the CA cert/trusted chain on all devices
- they'll now trust any certs signed by your internal CA
- works exactly like a cert you purchased
# Wildcard certificates
### Subject Alternative Name (SAN)
- extensions to an X.509 cert
- lists additional id info
- allows cert to support many different domains
![[Pasted image 20240605152635.png]]
### Wildcard domain
- certs are based on the name of the server
- a wildcard domain will apply to all server names in a domain
# Key revocation
### Certificate Revocation List (CRL)
- maintained by the CA
- can contain many revocations in a large file
### Many different reasons
- changes all the time
### April 2014 - CVE-2014-0160
- Heartbleed
- OpenSSL flaw put the private key of affected web servers at risk
- OpenSSL was patches, every web server certificate was replaced
- Older certs were moved to the CRL
![[Pasted image 20240605153032.png]]
# OCSP stapling
### Online Certificate Status Protocol (OCSP)
- provides scalability of OCSP checks
### The CA is responsible for responding to all client OCSP requests
- this may not scale well
### Instead, have the cert holder verify their own status
- status info is stored on the cert holder's server
### OCSP status is "stapled" into the SSL/TLS handshake
- digitally signed by the CA
# Getting revocation details to the browser
### OCSP
- the browser can check cert revocation
### Messages usually sent to an OCSP responder via HTTP
- easy to support over Internet links
- more efficient than downloading a CRL
### Not all browsers/apps support CCSP
- early IE versions did not support OCSP
- some support OCSP, but don't bother checking