### A programming conundrum
- sometimes, things at the same time
- is bad if not planned for
### Time-of-check to time-of-use attack (TOCTOU)
- check the system
- when do you see the results of your last check?
- something might happen between the check and the use
![[Pasted image 20240605233650.png]]
# Race conditions can cause big problems
### January 2004 - Mars rover "Spirit"
- reboot when a problem is identified
- problem with the file system, so reboot because of file system problem
- reboot loop was the result
### Pwn2Own Vancouver 2023 - Tesla Model 3
- TOCTOU attack against the Tesla infotainment using Bluetooth
- elevated privileges to root
- earned $100000 US prize and they keep the Tesla
