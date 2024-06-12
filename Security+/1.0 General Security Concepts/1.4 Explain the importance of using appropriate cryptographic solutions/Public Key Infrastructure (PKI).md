### Policies, procedures, hardware, software, people
- digital certs: create, distribute, manage, store, revoke
### This is a big, big endeavor
- lots of planning
### Also refers to the binding of public keys to people or devices
- the cert authority
- it's all about trust
# Symmetric encryption
### A single, shared key
- encrypt with key
- decrypt with same key
- if it gets out, use a new key
### Secret key algorithm
- a shared secret
### Doesn't scale very well
- can be challenging to distribute
### Very fast to use
- less overhead than asymmetric encryption
- often combined with asymmetric encryption
# Asymmetric encryption
### Public key cryptography
- two (or more) mathematically related keys
### Private key
- keep this private
### Public key
- anyone can see this key
- for public distribution
### The private key is the only key that can decrypt data encrypted with the public key
- you can't derive the private key from the public key
# The key pair
### Asymmetric encryption
- Public Key Cryptography
### Key generation
- build both the public and private key at the same time
- lots of randomization
- large prime numbers
- math
### Everyone can have the public key
- only Resource Owner has the private key
# Key escrow
### Someone else holds your decryption keys
- your private keys are in the hands of a 3rd party
- this may be within your own org
### This can be a legitimate business arrangement
- a business might need access to employee information
- government agencies may need to decrypt partner data
### Controversial?
- of course
- may be required
