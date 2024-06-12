### You can't deny what you've said
- there's no taking it back
### Sign a contract
- your signature adds non-repudiation
- you really did sign the contract
- others can see your signature
### Adds a different perspective for cryptography
- proof of integrity
- proof of origin, with high assurance of authority
# Proof of Integrity
### Verify data does not change
- data remains accurate and consistent
### In cryptography, we use a hash
- represent data as a short string of text
- a message digest, a fingerprint
### If data changes, the hash changes
- if person changes, you get a different fingerprint
### Doesn't necessarily associate data with an individual
- only tells you if data has changed
# Proof of origin
### Prove the message was not changed
- integrity
### Prove the source of the message
- authentication
### Make sure the signature isn't fake
- non-repudiation
### Sign with the private key
- the message doesn't need to be encrypted
- nobody else can sign this (obviously)
### Verify with the public key
- any change to the message will invalidate the signature
