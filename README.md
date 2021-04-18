# VacantSwarm

VacantSwarm is a consumer router application that runs on the LAN with other devices. When a virus is detected on the network via IPS it triggers to try to contain it or stall until you can shut off the devices. Alerting you immediatley with a small alarm, email, or SMS. Each container has a few ports open that route back to a honeypot for basic services. The services in the honeypot are lightweight and only accept handshakes, maximizing the number of services it can monitor for in favor of being able to simulate exactly what it wants to do within one. For example, SSH -> Server to access a file on partition 1.


Thought Board

OpenZFS on ARM + Deduplication w/ Memory through Docker for miminal footprint with a lot of small (16MB containers)

Unsure if ARM will work with it... Docker has the functionality on ZFS and a few other file systems to share memory among containers for .so modules and the like. Should be able to achieve 16MB each and fill a typical home network with ~4GB of RAM for the swarm + 2GB for the honeypot + Router.

IPS

Early Warning System 

Countermeasures


Virus detected... launch a swarm of IP addresses in vacant slots. Having ports open that forward back to a honeypot. Honeypot does basic statistics on ports it goes after. Optionally: Data is sent back to a cloud service to be analyzed anonamously. 
