# RAT-C2
A C2 project created in golang which leverages a RAT(remote access trojan) to perform tasks on a victim computer.A RAT is a tool used by
attackers to remotely perform actions on a compromised victim’s machine, such as accessing the filesystem, executing code, and sniffing network traffic.
Building this RAT requires building three separate tools: a client implant, a server, and an admin component. The client implant is the portion of the RAT 
that runs on a compromised workstation. The server is what will interact with the client implant, much like the way Cobalt Strike’s team server—the
server component of the widely used C2 tool—sends commands to compromised systems. Unlike the team server, which uses a single service to facilitate server and
administrative functions, we’ll create a separate, stand-alone admin component used to actually issue the commands. This server will act as the 
middleman, choreographing communications between compromised systems and the attacker interacting with the admin component.
