# SwitchingNetworkProject
Full Switching Network Project depends on CCNA 200-301 and CCNP Encor 350-401
🚀 Excited to share the successful completion of a full switching project using CCNA and CCNP protocols! This experience has been a fantastic journey, showcasing the power of advanced networking skills to enhance connectivity and efficiency. Proud to contribute to seamless and robust network infrastructure! 🌐 #Networking #CCNA #CCNP #NetworkEngineering 



In this project, I used a hierarchical design. 

In the Core Layer, 2 core SWs (Core 1 is the primary, and Core 2 is the backup) connected them all with 3 cables (2 forward with load balance and 1 is hot-standby in case of any failover). 

also, I used the following protocols: 

Management VLANs: I created 2 MGMT VLANs, to be able to reach the network. 

Rapid STP

LACP

Load Balance

DTP

VTP: initially create all needed VLANs through the main core SW when is set to server mode and the rest of SWs were in the client mode and then I turned all SWs to transparent mode

Storm Control

UDLD



In the Distribution Layer, I used 2 Distribution SWs (Distribution1 is the primary, and Distribution2 is the backup) and connected them all with 3 cables (2 forward with load balance and 1 is hot-standby in case of any failover).

and for more redundancy, all Core SWs are connected to all Distribution SWs in case of any failover. 

I used the same protocol which I used in the Core Layer

In the Access Layer, I used 4 Access SWs, every SW is connected to both Distribution SWs via 2 load-balanced cables. every access SW is connected to 4 vPCs 

I used the below protocols in this layer: 

Management VLANs

Rapid STP

VTP

LACP 

DTP

PortFast 

Port Security

and to secure the network from loops

BPDU Guard

BPDU Filter

LoopGuard

Storm Control. 
