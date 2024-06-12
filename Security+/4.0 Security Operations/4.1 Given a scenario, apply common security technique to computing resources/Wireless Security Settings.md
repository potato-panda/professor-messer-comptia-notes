# Securing a wireless network
### An org's wireless network can contain confidential info
- not everyone is allowed access
### Auth users before granting access
- who gets access to the wireless network?
- username/password, MFA
### Ensure that all comms is confidential
- encrypt wireless data
### Verify the integrity of all comms
- received data should be identical to the original sent data
- a message integrity check (MIC)
# The WPA2 PSK problem
### WPA2 has a PSK brute-force problem
- listen to the four-way handshake
	- some methods can derive the PSK hash without the handshake
- capture the hash
### With the hash, attackers can brute-force the pre-shared key (PSK)
### This has become easier as tech improves
- a weak PSK is easier to brute-force
- GPU processing speeds
- cloud-based password cracking
### Once you have PSK, you have everyone's wireless key
- there's no forward secrecy
# WPA3 and GCMP
### Wi-Fi Protected Access 3
- introduced 2018
### GCMP block cipher mode
- Galois/Counter Mode Protocol
- a stronger encryption than WPA2
### GCMP security services
- data confidentiality with AES
- Message Integrity Check with Galois Message Authentication Code
# [[Wireless Encryption#SAE|SAE]]
# Wireless authentication methods
### Gain access to a wireless network
- mobile users
- temp users
### Credentials
- shared password/PSK
- centralized auth (802.1X)
### Configuration
- part of the wireless network connection
- prompted during connection process
# [[Wireless Security#Wireless security modes|Wireless security modes]]
# [[AAA framework]]
# Gaining access
![[Pasted image 20240607180943.png]]
# [[Authentication Methods#RADIUS (Remote Authentication Dial-in User Service)|RADIUS]]
# [[Authentication Methods#IEEE 802.1X|IEEE 802.1X]]
# [[Port security#IEEE 802.1X and EAP|IEEE 802.1X and EAP]]