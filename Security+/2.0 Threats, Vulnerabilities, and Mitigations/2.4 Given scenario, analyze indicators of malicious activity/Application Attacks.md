# Injection attacks
### Code injection
- adding you own code into a data stream
### Enabled because of bad programming
- the app should properly handle input and output
### So many different injectable data types
- HTML, SQL, XML, LDAP, etc
# [[Buffer Overflows|Buffer overflows]]
# [[Replay Attacks|Replay attacks]]
# Privilege escalation
### Gain higher-level access to a system
- exploit a vuln
- might be a bug or design flaw
### Higher-level access means more capabilities
- commonly is the highest-level access
### High-priority vuln patches
- close ASAP
- any user can be admin
### Horizontal privilege escalation
- User A can access User B resources
# Mitigating privilege escalation
### Patch quickly
### Updated AV/Anti-malware software
### Data Execution Prevention
- only data in executable areas can run
### Address space layout randomization
- prevent a buffer overrun at a known memory address
# Elevation of privilege vulnerability examples
### CVE-2023-29336
- Win32k Elevation of Privilege Vulnerability
- May 2023
### Win32k Kernel driver
- Server 2008, 2008 R2, 2012, 2012 R2, 2016
- Windows 10
### Attacker would gain SYSTEM privileges
# [[Cross-site Scripting|Cross-site requests]]
### Cross-site requests are common and legitimate
- site loads text from visited site
- loads video from YouTube and images from Instagram on visited sites
### HTML on a website directs requests from your browser
- normal and expected
- most of these are unauthed requests
# The client and the server
### Website pages consist of client-side code and server-side code
### Client side
- renders page on screen
- HTML, JavaScript
### Server side
- performs requests from clients
- HTML, PHP
- transfer money from one account to another
- post a video on YouTube
# Cross-site request forgery
### One-click attack, session riding
- XSRF, CSRF (sea surf)
### Take advantage of trust that a web app has for the user
- web site trusts your browser
- requests are made without victim consent or knowledge
- attacker posts a Facebook status on your account
### Significant web app dev oversight
- app should have anti-forgery techniques added
- usually a cryptographic token to prevent a forgery
1. Attacker creates a funds transfer request
2. Request is sent as a hyperlink to a user who may already be logged into a bank web site
3. Visitor clicks the link and unknowingly sends the transfer request to the bank web site
4. Bank validates the transfer and sends the visitor's funds to the attacker
# Directory traversal
### Or path traversal
- read files from a web server that are outside the website's file directory
- users shouldn't be able to browse the server's folders
### Web server software vulnerability
- won't stop users from browsing past the web server root
### Web app code vulnerability
- take advantage of badly written code