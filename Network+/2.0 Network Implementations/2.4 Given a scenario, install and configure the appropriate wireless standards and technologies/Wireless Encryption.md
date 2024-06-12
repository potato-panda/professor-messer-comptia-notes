# Securing a wireless network
### An organization's wireless network can contain confidential information
- not everyone is allowed to access
### Authenticate the users before granting access
- who gets access to the wireless network?
- username, password, multi-factor authentication
### Ensure that all communication is confidential
- encrypt the wireless data
### Verify the integrity of all communication
- the received data should be identical to the original sent data
- a message integrity check (MIC)
# WPA (Wi-Fi Protected Access)
### 2002: WPA was the replacement for serious cryptographic weaknesses in WEP (Wired Equivalent Privacy)
- Don't use WEP encryption
### Needed a short-term bridge between WEP and whatever would be the successor
- runs on existing hardware
### WPA: RC4 with TKIP (Temporary Key Integrity Protocol)
- Initialization Vector (IV) is larger and an encrypted hash
- every packet gets a unique 128-bit encryption key
# Wireless encryption
### All wireless computers are radio transmitters and receivers
- anyone can listen in
### Solution: Encrypt the data
- everyone has an encryption key
### Only people with the right key can transmit and listen
- WPA2 and WPA3
# WPA2 and CCMP
### Wi-Fi Protected Access II (WPA2)
- WPA2 certification began in 2004
### CCMP block cipher mode
- Counter Mode with Cipher Block Chaining Message Authentication Code Protocol, or Counter/CBC-MAC Protocol
### CCMP security services
- Data confidentiality with AES encryption
- Message Integrity Check (MIC) with CBC-MAC
# WPA3 and GCMP
### Wi-Fi Protected Access (WPA3)
- introduced in 2018
### GCMP block cipher mode
- Galois/Counter Mode Protocol
- a strong encryption than WPA2
### GCMP security services
- Data confidentiality with AES
- Message Integrity Check (MIC) with Galois Message Authentication Code (GMAC)
# The WPA2 PSK problem
### WPA2 has a PSK brute-force problem
- listen to the 4-way handshake
	- some methods can derive the PSK hash without the handshake
- Capture the hash
### With the hash, attackers can brute-force the pre-shared key (PSK)
### This has become easier as technology improves
- a weak PSK is easier to brute force
- GPU processing speeds
- cloud-based password cracking
### Once you have the PSK, you have everyone's wireless key
- there's no forward secrecy
# SAE
### WPA3 changes the PSK authentication process
- includes mutual authentication
- creates a shared session key without sending that key across the networks
- no more four-way handshakes, no hashes, no brute force attacks
- add perfect forward secrecy
### Simultaneously Authentication of Equals (SAE)
- a Diffie-Hellman derived key exchange with an authentication component
- everyone uses a different session key, even with the same PSK
- and IEEE standard - the dragonfly handshake
# Wireless security modes
### Configure the authentication on your wireless AP/ wireless router
### Open System
- no authentication password is required
### WPA/2/3-Personal / WPA/2/3-PSK
- WPA/2/3 with a pre-shared key
- everyone uses the same 256-bit key
### WPA/2/3-Enterprise /WPA/2/3802.1X
- authenticates users individually with an authentication server (i.e. RADIUS)
![[Pasted image 20240513151831.png]]