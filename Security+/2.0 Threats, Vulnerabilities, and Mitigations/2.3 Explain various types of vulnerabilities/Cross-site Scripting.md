### XSS
### Originally called cross-site because of browser security flaws
- info from one site could be shared with another
### One of the most common web app vulns
- takes advantage of the trust a user has for a site
- complex and varied
### XSS commonly uses JavaScript
- do you allow scripts? Me too
1. Attacker sends a link containing a malicious script to a victim
2. Victim clicks the link and visits legitimate site
3. Legitimate site loads in the victim's browser. Malicious script is also executed
4. Malicious script sends victim's data (session cookies, etc...) to attacker
# Non-persistent (reflected) XSS attack
### Web site allows scripts to run in user input
- search box is a common source
### Attacker emails a link that takes advantage of this vuln
- runs a script that sends cred/session IDS/cookies to the attacker
### Script embedded in URL executes in the victim's browser
- as if it came from the server
### Attacker uses cred/session IDs/cookies to steal victim's info without their knowledge
- very sneaky
# Persistent (stored) XSS attack
### Attacker posts a message to a social network
- includes the malicious payload
### It's now "persistent"
- everyone gets the payload
### No specific target
- all viewer to the page
### For social networking, this can spread quickly
- everyone who views the message can have it posted to their page
- where someone else can view it and spread it further
# Hacking a Subaru
### July 2017, Aaron Guzman
- security researcher
### When authn with Subaru, users get a token
- this token never expires!
### A valid token allowed any service request
- even adding your email address to someone else's account
- now you have full access to someone else's car
### Web front-end included an XSS vuln
- a user clicks a malicious link, and you have their token
# Protecting against XSS
### Be careful when clicking untrusted links
- never blindly click in your email inbox. Never.
### Consider disabling JavaScript
- or control with an extension
- offers limited protection
### Keep your browsers and apps updated
- avoid the browser vulns
### Validate input
- don't allow users to add their own scripts to an input field