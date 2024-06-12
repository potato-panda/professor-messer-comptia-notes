# Device performance
### Temperature
- internal sensors, sometimes many
- can be an early warning of excessive utilization or hardware issues
### CPU Usage
- measures performance of the processor(s)
- overall performance is usually based on these values
### Memory
- the operational resource
- running out of memory is usually a fatal event
![[Pasted image 20240513160316.png]]
# Bandwidth monitors
### The fundamental network statistic
- amount of network use over time
### Many different ways to gather this metric
- SNMP, NetFlow, sFlow, IPFIX protocol analysis, software agent
### Identify fundamental issues
- nothing works properly if bandwidth is highly utilized
# Latency
### A delay between the request and the response
- waiting time
### Some latency is expected and normal
- laws of physics apply
### Examine the response times at every step along the way
- this may require multiple measurement tools
### Packet captures can provide detailed analysis
- microsecond granularity
- gets captures on both sides
# Jitter
### Most real-time media is sensitive to delay
- data should arrive at regular intervals
- voice comms, live video
### If you miss a packet, there's no retransmission
- there's no time to "rewind" your phone call
### Jitter is the time between frames
- excessive jitter can cause you to miss information, "choppy" voice calls
![[Pasted image 20240513160822.png]]
# Monitoring the interface
### Often your first sign of trouble
- the local problems are easy to attack
### Can sometimes indicate a bigger issue
- problem with a switch or congestion in the network
### View in the operating system
- interface details
### Monitor with SNMP
- remote monitoring of all devices
- most metrics are in MIB-II format (Management Information Base)
- Proprietary MIB may in available
![[Pasted image 20240513160950.png]]
# Interface monitoring
### Link status
- link up, or link down?
- may be a problem on the other end of the cable
### Error rate
- problems with the signal
- CRC error, runt, giant
### Utilization
- per-interface network usage
- run bandwidth tests to view throughput
![[Pasted image 20240513161159.png]]
### Discards, packet drops
- no errors in the packet, but system could not process
### Interface resets
- packets are queue, but aren't sent
- connection is good, but line protocols aren't talking
- reset and hope for the best
### Speed and duplex
- these should match on both sides
- auto speed and auto duplex isn't always the best option
- check for expected throughput and late collisions