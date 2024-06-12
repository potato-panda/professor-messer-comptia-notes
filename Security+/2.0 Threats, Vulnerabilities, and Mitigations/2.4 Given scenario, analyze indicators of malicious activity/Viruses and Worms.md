# Virus
### Malware that can reproduce itself
- it needs you to execute a program
### Reproduces through file systems or the network
- just running a program can spread a virus
### May or may not cause problems
- some viruses are invisible, some are annoying
### AV is very common
- thousands of new viruses every week
- is your signature file updates
# Virus types
### Program viruses
- it's part of an app
### Boot sector viruses
- who needs an OS?
### Script viruses
- OS and browser based
### Macro viruses
- common in MS Office
# Fileless virus
### A stealth attack
- does a good job of avoiding AV detection
### Operates in memory
- but never installed in a file or app
1. User clicks on a malicious website link
2. Website exploits a Flash/Java/Windows vulnerability
3. Launches PowerShell and downloads payloads in RAM
4. Runs PowerShell scripts and executables in memory, exfil data, damages files
5. Adds an auto-start to Registry
# Worms
### Malware that self-replicates
- doesn't need you to do anything
- uses the network as a transmission medium
- self-propagates and spreads quickly
- can take over many systems very quickly
### Firewalls and IDS/IPS can mitigate many worm infestations
- doesn't help much once the worms get inside
# Wannacry worm
1. Infected computer searches for vulnerable systems
2. Vulnerable computer is exploited with EternalBlue
3. Backdoor is installed and downloads WannaCry
