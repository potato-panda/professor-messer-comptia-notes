### Many networks are relatively open on the inside
- once you're through firewall, there are few security controls
### Zero trust is a holistic approach to network security
- covers every device, process, person
### Everything must be verified
- nothing is inherently trusted
- MFA, encryption, system permissions, additional firewalls, monitoring and analytics, etc.
# Planes of operation
### Split the network into functional planes
- applies to physical, virtual, and cloud components
### Data plane
- process the frames, packets, and network data
- processing, forwarding, trunking, encrypting, NAT
### Control plane
- manages the actions of the data plane
- define policies and rules
- determines how packets should be forwarded
- routing tables, session tables, NAT tables
# Extend the physical architecture
### Separate into functional tasks
- incorporate into hardware or software
![[Pasted image 20240604202121.png]]
# Controlling trust
### Adaptive Identity
- consider the source and requested resources
- multiple risk indicators - relationship to the org, physical location, type of connection, IP address, etc
- make the authn stronger, if needed
### Threat scope reduction
- decrease the number of possible entry points
### Policy-driven access control
- combine the adaptive identity with a predefined set of rules
# Security zones
### Security is more than a one-to-one relationship
- broad orgs provide a security-related foundation
### Where are you coming from and where are you going?
- trusted, untrusted
- internal network, external network
- VPN1, VPN5, VPN11
- Marketing, IT, Accounting, HR
### Using the zones may be enough by itself to deny access
- for ex. **Untrusted** to **Trusted** zone traffic
### Some zones are implicitly trusted
- for ex. **Trusted** to **Internal** zone traffic
# Policy enforcement point
### Subjects and systems
- end users, applications, non-human entities
### Policy enforcement point (PEP)
- the gatekeeper
### Allow, monitor, and terminate connections
- can consist of multiple components working together
![[Pasted image 20240604203028.png]]
# Applying trust in the planes
### Policy Decision Point
- there's a process for making an authn decision
### Policy Engine
- evaluates each access decision based on policy and other information sources
- grant, deny, or revoke
### Policy Administrator
- communicates with the Policy Enforcement Point
- Generates access tokens or credentials
- Tells the PEP to allow or disallow access
![[Pasted image 20240604203344.png]]
# Zero trust across planes
![[Pasted image 20240604203400.png]]
