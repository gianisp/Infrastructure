
## Life Cycle Management
The customer connection and hosting environment are easy to deploy and maintain trough benefits such as:
* Automatic configuration and deployment through Self-Service Portal
*	Based on commercially available HW, standard protocols and Kongsberg templates
*	Hardware management and continuous product development
*	Node management can include malware protection and intrusion detection
*	Marine approved HW (by DNV GL)
*	Kongsberg provides third line support on hardware and software solutions

## Remote Services
K-GSN is the basis for providing Remote Services, using remote access tools like BOMGAR. KONGSBERG Remote Services is a tool for certified Kongsberg engineers worldwide to connect to an installation upon customer request and provide support.
KONGSBERG Remote Service though K-GSN gives access to:
*	Operational support and guidance
*	Inspection of offshore systems and interfaces
*	Preparation and investigation prior to service visits
*	Remote update of offshore systems
*	Remote commissioning
 
 ![](https://github.com/kognifai/Infrastructure/blob/master/.attachments/Remote%20Services.png)
 
## Technical Specifications
K-GSN can be deployed using a range of HW and SW components, depending on end characteristics and delivery scale. The global network solution consists of two groups of devices, communication hubs and node network devices. All network traffic between network devices are encrypted. Any IP-based communication link can be utilized as a communication carrier.

![](https://github.com/kognifai/Infrastructure/blob/master/.attachments/Technical%20Specifications.png)
 
## Technology Components
*	IPSEC encrypted MPLS based Service Provider WAN. Controlled and maintained only by KONGSBERG’S PKI regime.
*	Geo redundant global network without any single point of failure
*	Customer segregation by VRF technology
*	Router onboard a vessel will always connect to the nearest available communication HUB
*	Equipment vendors can be given access to one or more vessels via the K-GSN network
*	Marine approved Cisco ISR Router that are a combined device that acts as WAN router, Firewall and switch. Controlled and maintained only by KONGSBERG’S certified personnel.
*	KONGSBERG uses Open standards and well known Cisco products in the K-GSN solution and have a close collaboration with Cisco and their products.

![](https://github.com/kognifai/Infrastructure/blob/master/.attachments/Technology%20Components.png)

## Detailed description
The network is designed to interconnect KONGSBERG controlled support and data centres, and nodes owned by customers of KONGSBERG.
## Internet as carrier
Internet is the primary carrier between sites, due to cost issues with leased lines. Most of the sites will also be carried by a satellite link.
## Scalability
The network design is scalable up to 50 000 logical separated networks and more than 30 000 nodes within the KONGSBERG global IP addressing plan. In addition, close to 25 000 nodes with private IP addressing plan can be deployed within this design.
## Customer separation
All communication shall be carried by a common network infrastructure. The solution provides a reliable and secure separation of each customer communicating through the network.
