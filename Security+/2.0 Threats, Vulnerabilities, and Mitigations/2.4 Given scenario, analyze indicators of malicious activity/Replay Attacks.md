### Useful info is transmitted over network
- can be take advantage of
### Need access to the raw network data
- network tap, ARP poisoning, malware
### The gathered info may help attacker
- replay the data to appear as someone else
### This is not on-path attack
- actual replay doesn't require the original machine
# Pass the hash
1. Victim computer sends normal auth request to server (passing through the switch)
2. Attacker has redirected that request (from the switch) to their computer capturing creds
3. Attacker can now replay that request to the server
4. Attacker gains access posing as the victim
### Avoid this type of replay attack with a salt or encryption
- use a session ID with the password hash to create a unique auth hash each time
# Browser cookies and session IDs
### Cookies
- info stored on your computer by the browser
### Used for tracking, personalization, session mgnt
- not generally a security risk, not executable
	- unless someone gets them
### Could be considered a privacy risk
- lots of personal data there
### Session IDs are often stored in cookies
- maintains sessions across multiple browser sessions
# Session hijacking (Sidejacking)
### If attacker gets the session ID, attacker can pose as the victim
# Header manipulation
### Info gathering
- Wireshark, Kismet
### Exploits
- Cross-site scripting
### Modify headers
- Tamper, Firesheep, Scapy
### Modify cookies
- Cookies Manager+ (Firefox add-on)
# Prevent session hijacking
### Encrypt E2E
- they can't capture your session ID if they can't see it
- additional load on the web server (HTTPS)
- Firefox extension: HTTPS Everywhere, Force-TLS
- many sites are now HTTPS-only
### Encrypt end-to-somewhere
- at least avoid capture over a local wireless network
- still in-the-clear for part of the journey
- personal VPN
