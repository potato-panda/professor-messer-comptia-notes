# Hashes
### Represent data as a short string of text
- a message digest, a fingerprint
### One-way trip
- impossible to recover the original message from the digest
- used to store passwords / confidentiality
### Verify a downloaded document is the same as the original
- integrity
### Can be a digital signature
- authn, non-repudiation, and integrity
### Will not have a collision (hopefully)
- different messages should not have the same hash
# A hash example
### SHA256 hash
- 256 bits / 64 hexadecimal chars
# Collision
### Hash functions
- take an input of any size
- create a fixed size string
- message digest, checksum
### The hash should be unique
- different input should never create the same hash
- if they do, it is a collision
### MD5 has a collision problem
- found in 1996
- don't use MD5 for anything important
# Practical hashing
### Verify a downloaded file
- hashes may be provided on the download site
- compare the downloaded file hash with the posted hash value
### Password storage
- instead of storing the password, store a salted hash
- compare hashes during the authn process
- nobody ever knows your actual password
# Adding some salt
### Salt
- random data added to a password when hashing
### Every user gets their own random salt
- the salt is commonly stored with the password
### Rainbow tables won't work with salted tables
- additional random value added to the original password
### This slows things down the brute force process
- it doesn't completely stop reverse engineering it
# Digital signatures
### Prove the message was not changed
- integrity
### Prove the source of the message
- authn
### Make sure the signature isn't fake
- non-repudiation
### Sign with private key
- the message doesn't need to be encrypted
- nobody else can sign this (obviously)
### Verify with public key
- any change in message will invalidate the signature
