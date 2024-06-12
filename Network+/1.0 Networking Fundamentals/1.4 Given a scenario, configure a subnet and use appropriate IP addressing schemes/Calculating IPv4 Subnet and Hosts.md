# Why subnet the network?
> In a network diagram of routers and IP addresses with subnet masks, and each one of these networks is subnetted into its own range of IP addresses. 
> 
> Well, the question, of course, is **why do we go through this process of performing all of these calculations, splitting the network up into these smaller pieces, and having to manage all of these separate IP subnets?** 
> 
> Well, one of the most common reasons is that it's **very difficult to connect all devices to all other devices in the world simultaneously**. It would require a massive amount of technology to be able to know where every single device happens to be at any particular time.
> 
> Instead, **we use routers to separate the network into smaller pieces, and we simply send our traffic to the next router, who then determines where the next route would be after that.** 
> 
> It's a much simpler way of being able to manage such a large number of devices on a network, and yet still allow us to communicate to all of these separate endpoints. 

# VLSM (Variable Length Subnet Mask)
### Class-based networks are inefficient
- subnet mask is based on the network class
### Allow network admins to define their own masks
- customize the subnet mask to specific network requirements
### Use different subnet masks in the same classful network
- 10.0.0.0/8 is the class A network then
- 10.0.1.0 /24 and 10.0.80./26 would be VLSM

# Defining subnets
### IP address: 10.0.0.0
- class A, subnet mask: 255.0.0.0.
- "Classful" addressing
We have
![[Pasted image 20240506162410.png]]
and cut it to
![[Pasted image 20240506162450.png]]

# Calculating subnets and hosts
### Powers of two
![[Pasted image 20240506163945.png]]
![[example.png]]
---

![[example 2.png]]
---

![[example 3.png]]
