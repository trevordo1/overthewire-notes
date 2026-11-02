# ROUTERS
> what is a router? 
    A router is a device that connects two separate networks together
    A network is just a place where devices can talk to each other within itself, but what happens when you want to visit a site that is not on your network? You need a router!

> why can't two devices on separate networks talk to each other?  
    It doesn't work because of how devices find destination mac addresses on a switch (ARP Frame) -----> reminder: ARP frame is the message a device sends out to every device connected to the network to ask if they have a certain IP address. A switch does not automatically know the MAC address of a device until it sends a frame through it.

    When an ARP message is sent out looking for an IP that is not on the network, it defaults to sending the message to its GATEWAY

    > EXAMPLE: my network is the range 10.1.1.0 -> 10.1.1.255, so if I try to find the device on the IP 23.1.1.0, my device already knows that it is not on the network so it defaults to sending the frame to my GATEWAY

# GATEWAY 

A gateway is the place where traffic goes in order to talk to devices that are not on your network. For home networks, it is usually a router. 

Routers only talk on l3 or IP addresses. They look at the IP src and the destination IP. 
Then it sends out an ARP frame to other swithces that are connected to it. 
The switch with the correct device sends a message back to the router, which sends it back to the source mac address. 
The source device then sends a message to the router's mac address, but the destination device's IP address
MEssage goes from the router, to the destination IP address's switch

# DNS SERVER
A server that is on your sw


