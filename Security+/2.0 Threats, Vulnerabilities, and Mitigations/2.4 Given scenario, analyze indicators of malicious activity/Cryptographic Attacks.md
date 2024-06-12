### You've encrypted data and sent it to another person
- is it really secure?
- how do you know?
### Attacker doesn't have the combination (the key)
- so they break the safe (the cryptography)
### Finding ways to undo the security
- there are many potential cryptographic shortcomings
- the problem is often the implementation
# Birthday attack
### In a classroom of 23 students, what is the chance of two students sharing a birthday?
- about 50%
- for a class of 30, the change is ~70%
### In the digital world, this is a hash collision
- a hash collision is the same hash value for two different plaintexts
- find a collision through brute force
### Attacker will generate multiple versions of plaintext to match the hashes
- protect yourself with a large hash output size
# Collisions
### Hash digests are supposed to be unique
- different input data should not create the same hash
### MD5 hash
- Message Digest Algorithm 5
- first published in April 1992
- collisions identified in 1996
### December 2008: Researchers created CA certificate that appeared legitimate when MD5 is checked
- build other certs that appeared to be legit and issued by RapidSSL
# Downgrade attack
### Instead of using perfectly good encryption, use something that's not so great
- force the system to downgrade their security
### SSL stripping
- combines an on-path attack with a downgrade attack
- difficult to impl, but big returns for the attacker
- attacker must sit in the middle of comms
- victim's browser page isn't encrypted
- strips the S away from HTTPS
![[Pasted image 20240606164849.png]]
# Plaintext / unencrypted passwords
### Some apps store password "in the clear"
- no encryption; you can read it
- rare
### DO NOT STORE PASSWORDS AS PLAINTEXT
- anyone with access to the file or db has all the creds
### Get a better app
# Hashing a password
### Hashes represent data as fixed-length string of text
- message digest, or "fingerprint"
### Will not have a collision (hopefully)
- different inputs should not have the same hash
### One-way trip
- impossible to recover the original message from the digest
- a common way to store passwords
# The password file
### Different across OS and apps
- different hash algos
# Spraying attack
### Try to login with an incorrect password
- eventually locked out
### There are some common passwords:
- https://en.wikipedia.org/wiki/List_of_the_most_common_passwords
### Attack an account with the top three (or more) passwords
- if they don't work, move to the next account
- no lockouts, no alarms, no alerts
# [[Password Attacks#Brute force|Brute force]]