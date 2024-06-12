# Dynamic routing protocols
### Listen for subnet information from other routers
- sent from router to router
### Provide subnet information to other routers
- tell other routers what you know
### Determine the best path based on the gathered information
- every routing protocol has its own way of doing this
### When network changes occur, update the available routes
- different convergence process for every dynamic routing protocol
# Which routing protocol to use?
### What exactly is a route?
- is it based on the state of the link?
- is it based on how far away it is?
### How does the protocol determine the best path?
- some formula is applied to the criteria to create a metric
- ranks the routes from best to worst
### Recover after a change to the network
- convergence time can vary widely between routing protocols
### Standard or proprietary protocol?
- OSPF and RIP are standards, some functions of EIGRP are Cisco property
# Distance-vector routing protocols
### Information passed between routers contain network details
- how many "hops" away is another network?
- the deciding "vector" is the "distance"
### Usually automatic
- relative little configuration
### Good for smaller networks
- doesn't scale well to very large networks
### RIP (Routing Information Protocol), EIGRP (Enhanced Interior Gateway Routing Protocol)
# Distance-vector routing
![[Pasted image 20240510160851.png]]
# Link-state routing protocols
### Information passed between routers is related to the current connectivity
- if it's up, you can get there
- if it's down, you can't
### Consider the speed of the link
- faster is always better, right?
### Very scalable
- used most often in large networks
### OSPF (Open Shortest Path First)
- large, scalable routing protocol
# Hybrid routing protocols
### A little link-state, a little distance-vector
- not many examples of a hybrid routing protocol
### BGP (Border Gateway Protocol)
- determines best route based on paths, network policies, or configured rule-sets