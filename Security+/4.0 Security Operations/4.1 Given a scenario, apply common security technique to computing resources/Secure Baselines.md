### Security of app env should be well defined
- all app instances must follow this baseline
- firewall settings, patch levels, OS file versions
- may require constant updates
### Integrity measurements check for secure baselines
- perform often
- check against well-documented baselines
- failure requires immediate correction
# Establish baselines
### Create a series of baselines
- foundational security policies
### Baselines often available from the manufacturer
- app dev
- OS dev
- appliance manufacturer
### Many OS have extensive options
- over 3,000 group policies settings in Windows 10
- only some are associated with security
# Deploy baselines
### With established detailed security baselines
- how to put these baselines in action?
### Deploy baselines
- usually managed through centrally administered console
### May require multiple deployment mechanisms
- Active Directory group policy, MDM, etc
### Automation is the key
- deploy to many devices
# Maintain baselines
### Many of these are best practices
- rarely change
### Other baselines may require ongoing updates
- a new vuln is discovered
- an updated app has been deployed
- new OS is installed
### Test and measure to avoid conflicts
- some baselines may contradict others
- enterprise env are complex