### Simple Network Management Protocol
- a database of data (MIB) - Management Information Base
- the database contains OIDs - Object Identifiers
- Poll devices over udp/161
### SNMP v1 - the original
- structured table, in-the-clear
### SNMP v2 - a good step ahead
- data types enhancements, bulk transfers, still in-the-clear
### SNMP v3 - the new standard
- message integrity check (MIC), authentication, encryption
# SNMP OIDs
### An object identifier can be referenced by name or number
- .iso(1).org(3).dod(6).internet(1).mgmt(2).mib-2(1).snmp(11).snmpOutTraps(29).0
- .1.3.6.1.2.1.11.29.0
### Every variable in the MIB has a corresponding OID
- some are common across devices
- some manufacturers define their own object identifiers
### The SNMP manager requests information based on OID
- a consistent reference across devices
![[Pasted image 20240513164926.png]]
# Graphing with SNMP
![[Pasted image 20240513165030.png]]
# SNMP traps
### Most SNMP operations expect a poll
- devices then respond to the SNMP request
- this requires constant polling
### SNMP traps can be configured on the monitored device
- communicates over udp/162
### Set a threshold for alerts
- if number of CRC errors increases by 5, send a trap
- monitor station can react immediately