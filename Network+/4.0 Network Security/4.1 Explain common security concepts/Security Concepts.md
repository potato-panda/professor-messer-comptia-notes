# Vulnerabilities
### A weakness in the system
- allows the bad guys to gain access or cause a security breach
### Some vulnerabilities are never discovered
- or discovered after years of use
### Many different vulnerability types
- data injection
- broken authentication process
- sensitive data exposure
- security misconfiguration
# Zero-day attacks
### Many applications have vulnerabilities
- we've just not found them yet
### Someone is working hard to find the next big vulnerability
- the good guys share these with the developer
### Attackers keep these yet-to-be discovered holes to themselves
- they want to use these vulnerabilities for personal gain
### Zero-day
- the vulnerability has not been detected or published
- zero-day exploits are increasingly common
### Common Vulnerabilities and Exposures (CVE)
- https://cve.metre.org/
# Threat
### A vulnerability can be exploited by a thread
- may be intentionally (attacker) or accidental (fire, flood, etc)
- many of these threads are external to the organization
### A resource can have a vulnerability
- the vulnerability can be exploited by a threat agent
- the threat agent takes a threat action to exploit the vulnerability
### The result is a loss of security
- data breach, system failure, data theft
# Insider threats
### We give people tons of access
- least privilege, anyone?
### You have more access than others just by entering the building
- lock away your documents
- some organizations have very specific procedures
### Significant security issues
- harms reputation
- critical system disruption
- loss of confidential or proprietary information
# Vulnerability databases
### Researchers find vulnerabilities
- everyone neeeds to know about them
### Common Vulnerabilities and Exposure (CVE)
- a community managed list of vulnerabilities
- sponsored by the U.S. Department of Homeland Security (DHS) and Cybersecurity and Infrastructure Security Agency (CISA)
### U.S. National Vulnerability Database (NVD)
- a summary of CVEs
- also sponsored by the DHS and CISA - https://nvd.nist.gov
### NVD provides additional details over the CVE list Patch availability and severity scoring
![[Pasted image 20240513221112.png]]
![[Pasted image 20240513221121.png]]
# Exploits 
### Take advantage of a vulnerability
- gain control of a system
- modify data
- disable a service
### Many exploit methods
- built to take advantage of a vulnerability
- may be complex
# Least Privilege
### Rights and permissions should be set to the bare minimum
- you only get exactly what's needed to complete your objective
### All user accounts must be limited
- applications should run with minimal privileges
### Don't allow users to run with admin privileges
- limits the scope of malicious behavior
# Role-based access control (RBAC)
### You have a role in your organization
- manager, director, team lead, project manager
### Administrators provide access based on the role of the user
- rights are gained implicit instead of explicitly
### In Windows, use Groups to provide role-based access control
- you are in shipping and receiving, so you can use the shipping software
- you are the manager, so you can review the shipping logs
# Zero trust
### Many networks are relatively open on the inside
- once you're through the firewall, there are few security controls
### Zero trust is a holistic approach to network security
- covers every device, every process, every person
### Everything must be verified
- nothing is trusted
-  multifactor authentication, encryptions, system permissions, additional firewalls, monitoring and analytics, etc