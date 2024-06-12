# Secure coding concepts
### Balance between time and quality
- programming with security in mind is often secondary
### Testing x3
- the Quality Assurance (QA) process
### Vulnerabilities will eventually be found
- and exploited
# Input validation
### What is the expected input?
- validate actual vs expected
### Document all input methods
- forms, fields, type
### Check and correct all input (normalization)
- a ZIP code should only only X characters long with a letter in the X column
- fix any data with improper input
### The fuzzers will find what you missed
- don't give them an opening
# [[Replay Attacks#Browser cookies and session IDs|Secure cookies]]
### Sensitive information should not be saved in a cookie
- isn't designed to be secure storage
# Static code analyzer
### Static Application Security Testing (SAST)
- help to identity security flaws
### Many security vulnerabilities found easily
- buffer overflows, database injections, etc.
### Not everything can be identified through analysis
- authn security, insecure cryptography, etc
- don't rely on automation for everything
### Still have to verify each finding
- false positives are an issue
![[Pasted image 20240607182016.png]]
# Code signing
### An app is deployed
- users run app executable or scripts
### So many security questions
- has the app been modified in any way?
- can you confirm that the app was written by a specific dev?
### The app code can be digitally signed by the dev
- asymmetric encryption
- a trusted CA signs the dev's public key
- dev signs the code with their private key
- for internal apps, use your own CA
# Sandbox
### Apps cannot access unrelated resources
- they play in their own sandbox
### Commonly used during deployment
- can be useful prod tech
### Used in many different deployments
- VMs
- mobile devices
- browser iframes (Inline Frames)
- Windows User Account Control (UAC)
# Application security monitoring
### Real-time information
- app usage, access demographics
### View blocked attacks
- SQL injection attempts, patched vulnerabilities
### Audit the logs
- find the info gathering and hidden attacks
### Anomaly detection
- unusual file transfer
- increase in client access