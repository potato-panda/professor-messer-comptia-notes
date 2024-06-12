### Define different VLANs
- organizational, network engineering, security
### You only have access to your VLAN
- good security best practice
### "Hop" to another VLAN
- this shouldn't happen
### Two primary methods
- switch spoofing
- double tagging
# Switch spoofing
### Some switches support automatic configuration
- is the switch port for a device?, or is it a trunk?
### There's no authentication required
- pretend to be a switch
- send trunk negotiation
### Now you've got a trunk link to a switch
- send and receive from any configured VLAN
### Switch administrators should disable trunk negotiation
- administratively configure trunk interfaces and device/access interface
# Double tagging
### Craft a packet that includes two VLAN tags
- takes advantage of the "native" VLAN configuration
### The first native VLAN tag is removed by the first switch
- the second "fake" tag is now visible to the second switch
- packet is forwarded to the target
### This is a one-way trip
- responses don't have a way back to the source host
- Good for DoS
### Don't put any devices on the native VLAN
- change the native VLAN ID
- force tagging of the native VLAN
![[Pasted image 20240514170010.png]]
![[Pasted image 20240514170135.png]]
![[Pasted image 20240514170145.png]]
![[Pasted image 20240514170154.png]]
![[Pasted image 20240514170203.png]]