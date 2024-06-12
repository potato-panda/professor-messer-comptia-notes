# Encrypting stored data
### Protect data on storage devices
- SSD, hard drive, USD drive, cloud storage, etc
- these are data at rest
### Full-disk and partition/volume encryption
- BitLocker, FileVault, etc
### File encryption
- EFS (Encrypting File System), third-party utilities
# Database encryption
### Protecting stored data
- and the transmission of that data
### Transparent encryption
- encrypt all db info with a symmetric key
### Record-level encryption
- encrypt individual columns
- use separate symmetric keys for each column
# Transport encryption
### Protect data traversing the network
- you're probably doing this right now
### Encrypting in the app
- browsers can communicate using HTTPS
### VPN
- encrypts all data transmitted over the network
- client-based VPN using SSL/TLS
- site-to-site VPN using IPsec
# Encryption algorithm
### There are many many different ways to encrypt data
- the proper "formula" must be used during encrypt/decryption
### Both sides decide on the algo before encrypting the data
- the details are often hidden from end user
### There are advantages and disadvantages between algos
- security level, speed, complexity of implementation, etc
# Encryption algo comparison
![[Pasted image 20240605131150.png]]
# Cryptographic keys
### There's very little that isn't known about the cryptographic process
- the algo is usually a known entity
- the only thing you don't know is the key
### The key determines the output
- encrypted data
- hash vale
- digital signature
### Keep your private key private
- it protects your data
# Key lengths
### Larger keys tend to be more secure
- prevent brute-force attacks
- attackers can try every possible key combination
### Symmetric encryption
- 128-bit or larger symmetric keys are common
- these numbers get larger and larger as time goes on
### Asymmetric encryption
- complex calculations of prime numbers
- larger keys than symmetric keys
- common to see key lengths of 3072 bits or larger
# Key stretching
### A weak key is a weak key
- by itself, it's not very secure
### Make a weak key stronger by performing multiple processes
- hash a password. hash the hash of the password, and continue ...
- key stretching, key strengthening
### Brute force attacks would require reversing each of those hashes
- the attacker has to spend much more time, even though the key is small