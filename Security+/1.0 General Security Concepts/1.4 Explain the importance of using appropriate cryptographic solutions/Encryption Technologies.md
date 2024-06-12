# Trusted Platform Module (TPM)
### A spec for cryptographic functions
- cryptography hardware on a device
### Cryptographic processor
- random number generator, key generators
### Persistent memory
- unique keys burned in during manufacturing
### Versatile memory
- storage keys, hardware config info
- securely store BitLocker keys
### Password protected
- no dictionary attacks
# Hardware Security Module (HSM)
### Used in large env
- clusters, redundant power
- securely store thousands of cryptographic keys
### High-end cryptographic hardware
- plug-in card or separate hardware device
### Key backup
- secure storage in hardware
### Cryptographic accelerators
- offload that CPU overhead from other devices
# Key Management system
### Services are everywhere
- on-premises, cloud-based
- many different keys for many different services
### Manage all keys from a centralized manager
- often provided as third-party software
- separate the encryption keys from the data
### All key mgnt from one console
- create keys for a specific service or cloud provider (SSL/TLS, SSH, etc)
- associate keys with specific users
- rotate keys on regular intervals
- log key use and important events
# Keeping data private
### Our data is located in many different places
- mobile phones, cloud, laptop, etc
- the most private data is often physically closest to us
### Attackers are always finding new techniques
- it's a race to stay one step ahead
### Our data is changing constantly
- how do we keep our data protected?
# Secure enclave
### A protected area for our secrets
- often impl as a hardware processor
- isolated from the main processor
- many diff technologies and names
### Provides extensive security features
- has it's own boot ROM
- monitors the system boot process
- true random number generator
- real-time memory encryption
- root cryptographic keys
- performs AES encryption in hardware
- and more...