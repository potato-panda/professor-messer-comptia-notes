### A logistical challenge
- how do you share an encryption key across an insecure medium without physically transferring the key?
### Out-of-band key exchange
- don't sent the symmetric key over the net
- telephone, courier, in-person, etc
### In-band key exchange
- it's on the network
- protect the key with additional encryption
- use asymmetric encryption to deliver symmetric key
# Real-time encryption/decryption
### There's a need for fast security
- without compromising the security part
### Share a symmetric session key using asymmetric encryption
- client encrypts a random (symmetric) key with a server's public key
- the server decrypts this shared key and uses it to encrypt data
- this is the session key
### Impl session keys carefully
- need to be changed often (ephemeral keys)
- need to be unpredictable
# Symmetric key from asymmetric keys
### Use public and private key cryptography to create a symmetric key
- math is powerful
![[Pasted image 20240605141404.png]]