# [[Network Hardening#Password complexity and length|Password complexity and length]]
# Password age and expiration
### Password age
- how long since password was modified
### Password expiration
- passwords valid for a certain period
- 30, 60 , 90 days policy
- system remembers password history, requires unique password (no password reuse up to X previous passwords)
### Critical systems might change more frequently
- every 15 days or every week
# Password managers
### Important to use different passwords for each account
- remembering all of them would be impractical
### Store all passwords in a single db
- encrypted, protected
- can include MFA tokens
### Built-in to many OS
- and some browsers
### Enterprise password managers
- centralized management and recovery options
# Passwordless authentication
### Many breaches are due to poor password control
- weak passwords, insecure implementation
### Auth without password
- solves many password management issues
### You may already be passwordless
- facial recog, security key, etc
### May not be primary authn method
- used with a password or additional factors
# Just-in-time permissions
### In many orgs, IT team is assigned admin/root elevated account rights
- this is a great account to attack
### Grant admin access for a limited time
- no permanent admin rights
- the principle of least privilege
### A breached user account never has elevated rights
- narrow scope of breach
### Request access from a central clearinghouse
- grants/denies based on predefined security policies
### Password vaulting
- primary creds are stored in this vault
- vault controls who gets access to creds
### Accounts are temporary
- JIT process creates a time-limited account
- admin receives ephemeral creds
- primary passwords are never released
- creds are used for one session then deleted
