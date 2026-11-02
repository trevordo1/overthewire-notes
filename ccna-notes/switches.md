# SWITCHES

a switch is a device that allows other devices on the same network to talk to each other. It is a physical piece of hardware, so devices that are connected via wifi will not go directly through the switch. the connection must be ethernet. 

# HUBS
Before switches, there were hubs. Hubs suck because if you wanted to communicated to one device on the hub, it would send your packets and requests to every device and only the device the request from the client is for would respond. The rest of the devices would just ignore the packet. This is fine if there are no bad actors on the hub with you. They could easily take the packet sent to them and therefore get all your data. 


TREVOR ----------packet-----> HUB -----------------> ciara
                            
                               |
                               |
                               v
                               laura


# SWITCHES
goated hardware. The switch looks just like a hub, but it has a brain that knows where to send each packet of information. When a client sends a request to a server, it looks at the different IP addresses that are connected to the ports and only sends the request to the server it is requesting from. 

EXAMPLE: Trevor wants to send ciara message. Trevor sends to ciara ip. Switch takes information, looks for ip on which port, then sends packet only to that port. 

 CAM table (content addressable memory) --------> a table that shows which source mac address is on each port of the switch

    How does a switch know a devices MAC address before it is added to the CAM table? 
        ARP: Address resolution protocol
            Sends out a frame to all of the devices on the switch. It asks each one if their ip address is the one the request is for. 
            The place that the ARP message is sent is FFFF.FFFF.FFFF which is basically just a way to ask for each port's device's mac address. The devices on the switch all receive the message, they only respond if their mac address is the one that the ARP is asking for

# MAC ADDRESS 
the address attatched to each individual device
Never changes even if it switches networks or wifi

# LAYERS 
L1 Physical ----> electircal signals, wires, ethernet
L2 Datalink -----> mac address: the indiviadual address for each device
L3 IP 


switches can exist on either l2 or l3

# ACCESS POINT
basically a switch for wireless
the unifi shit that was in the office and is now around the stairs
is mostly like a hub. Connects to a switch via ethernet. It acts more like a hub because the wireless packets are able to be seen by all devices in the area

# QUIZ

1. Switches populate the cam table when a message is sent from a mac address. It will then have a memory of the device that is on the port