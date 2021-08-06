# RIIM battery lifetime estimation tool
## Description
This worksheet helps users estimate the current consumption and hence the battery lifetime of a RIIM mesh node	

In RIIM, mesh routers can be battery operated using a time syncronization method called TSCH (Time Slotted Channel Hopping)						
This means that nodes only wake up and listens for packets or sends packets at predetermined timeslots			

If a packet is not received within a short time window, the node can quickly go to sleep again to reduce current consumption.						

The current consumption and thus the battery lifetime of devices is not totally deterministic.					

Examples of factors that influence the battery lifetime are given below:						
- In a dense network, one can receive packets from more devices and thus spend more time receiving packets than in widespread network.					
 In a sensor network sending data to the cloud, one mesh router might be the only one in connection with the border router.
 Then all the other nodes will send their data through this specific node which increases the number of received and sent packets for this node. 
Therefore, the battery lifetime of this specific node will be lower than the other nodes.

- In a network with much noise and long distance between nodes, there will be more packet loss and thereby more retransmissions. 
This will reduce battery lifetime

The tool is applicable for RC1882CEF-IPM in current revision(Not the HP - 500mW versions)						
						
## How to use this tool:						
Open the input tab and give as much and as accurete information about the network, settings, and the node that is investigated for battery lifetime.						
This is done by entering your data in the orange fields						
Then observe how the current consumption and battery lifetime changes based on the input						
