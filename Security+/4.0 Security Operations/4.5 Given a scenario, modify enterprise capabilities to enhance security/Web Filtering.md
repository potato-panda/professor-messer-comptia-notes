# [[Firewall Types#The universal security control|Content filtering]]
### Control traffic based on data within the content
- URL filtering, website category filtering
### Corporate control of outbound and inbound data
- sensitive materials
### Control of inappropriate content
- NSFW, parental controls
### Protection against evil
- AV, anti-malware
# URL scanning
### Allow/deny based on URL
- URI
- allow/deny list
### Managed by category
- auction, hacking, malware, travel, recreation, etc
### Can have limited control
- URLs not only way to navigate
### Often integrated into NGFW
- filters traffic based on category or specific URL
# Agent-based
### Install client software on the user's device
- usually managed from a central console
### Users can be located anywhere
- local agent makes the filtering decisions
- always-on, always filtering
### Updates must be distributed to all agents
- cloud-based updates
- update status shown on console
# [[Advanced Networking Devices#Proxies|Proxies]]
# [[Network Appliances#Forward proxy|Forward proxy]]
# Block rules
### Based on specific URL
- \*.professormesser.com:Allow
### Category of site content
- usually divided into over 50 diff topics
- adult, edu, gambling, gov, home and garden, legal, malware, news, etc
### Diff dispositions
- edu:Allow
- home and garden:Allow and Alert
- gambling:Block
# Reputation
### Filter URLs based on percevied risk
- a good reput is allowed
- bad are blocked
- risk: trustworthy, low, med, suspicious, high risk
### Automated reputation
- sites are scanned and assigned a reput
### Manual reput
- managers can administratively assign a rep
### Add these dispositional to the URL filter
- high risk:Block, trustworthy:Allow
# DNS filtering
### Before connecting to a website, get IP address
- perform DNS lookup
### DNS is updated with real-time threat intel
- both commercial and public list
### Harmful sites are not resolved
- no IP address, no connection
### This works for any DNS lookup
- not just web filtering