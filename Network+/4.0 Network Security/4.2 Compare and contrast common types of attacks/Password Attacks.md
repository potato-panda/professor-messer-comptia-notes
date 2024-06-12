# Plaintext / unencrypted passwords
### Some applications store passwords "in the clear"
- no encryption. you can read the stored password
- this is rare, thankfully
### Do not store passwords as plaintext
- anyone with access to the password file or database has every credential
### What to do if your application saves passwords as plaintext:
- get a better application
# Hashing a password
### Hashes represent data as a fixed-length string of text
- a message digest, or "fingerprint"
### Will not have a collision (hopefully)
- different inputs will not have the same hash
### One-way trip
- impossible to recover the original message from the digest
- a common way to store passwords
# A hash example
### SHA-256 hash
- used in many applications
![[Pasted image 20240514175518.png]]
# The password file
### Different across operating systems and applications
- different hash algorithms
![[Pasted image 20240514175637.png]]
# Brute force
### Try every possible password combination until the hash is matches
### This might take some time
- a strong hashing algorithm slows things down
![[Pasted image 20240514175820.png]]
### Brute force attacks - Online
- keep trying the login process
- very slow
- most accounts will lockout after a number of failed attempts
### Brute force the hash - Offline
- obtain the list of users and hashes
- calculate a password hash, compare it to a stored hash
- large computational resource requirement
# Dictionary attacks
### Use a dictionary to find common words
- passwords are created by humans
### Many common wordlists available on the 'net'
- some are customized by language or line of work
### The password crackers can substitute letters
- p&ssw0rd
### This takes time
- distributed cracking and GPU cracking is common
### Discover passwords for common words
- this won't discover random character passwords