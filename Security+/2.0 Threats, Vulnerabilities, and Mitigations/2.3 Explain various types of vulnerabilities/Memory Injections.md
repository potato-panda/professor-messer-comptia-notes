# Finding malware
### Malware runs in memory
- memory forensics can find the malicious code
### Memory contains running processes
- DLLs (Dynamic Link Libraries)
- threads
- fuffers
- memory mgnt functions
- and much more
### Malware is hidden somewhere
- malware runs in its own process
- malware injects itself into a legitimate process
# Memory injection
### Add code into the memory of an existing process
- hide malware inside of the process
### Get access to the data in that process
- and the same rights and permissions
- performs a privilege escalation
# DLL injection
### Dynamic-Link Library
- a Windows library containing code and data
- many apps can use this library
### Attackers inject a path to a malicious DLL
- runs as part of the target process
### One of the most popular memory injection methods
- relatively easy to implement
![[Pasted image 20240605175244.png]]