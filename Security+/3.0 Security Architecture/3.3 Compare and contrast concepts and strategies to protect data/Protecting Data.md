# Geographic restriction
### Network location
- ID based on IP subnet
- can be difficult with mobile devices
### Geolocation - determine user's location
- GPS - mobile devices, very accurate
- 802.11 wireless, less accurate
- IP address, not very accurate
### Geofencing
- automatically allow/restrict access when user is in a particular location
- don't allow this app to run unless near office
### Primary job task
- an org is out of business without data
### Data is everywhere
### Encryption, security policies
### Data permissions
- not everyone has the same access
# Encryption
### Encode info into unreadable data
- original info is plaintext, encrypted form is ciphertext
### This is a two-way street
- convert between one and the other
- if you have the proper key
### Confusion
- the encrypted data is different than plaintext
# [[Hashing and Digital Signatures#Hashes|Hashing]]
# [[Obfuscation]]
- make something normally understandable very difficult to understand
### Take perfectly readable code and turn it into nonsense
- dev keeps the readable code and gives you chicken scratch
- both sets of codes perform exactly the same way
### Helps prevent the search for security holes
- makes it more difficult to figure out what's happening
- but not impossible
# Segmentation
### Many orgs use a single data source
- one large db
### One breach puts all of the data at risk
- making it easy for attacker
### Separate the data
- store it in different locations
# Permissions restrictions
### Control access to an account
- it's more than just username and password
- determine what policies are best for the org
### The auth process
- password policies
- authn factor policies
- other considerations