
# High-level Design

## Layered approach
The network design is segmented into two main layers:
- Interlan layer - This provides site-to-site connectivity
- Node layer - This handles connections to adjacent networks within the node.


## Interlan

One of the key features of the interlan layer is the customer separation mechanism. This mechanism ensures that there is no communication between nodes belonging to different customers and all communication is encrypted. This layer can utilize a broad variety of communication carriers such as internet, satellite communication, serial lines, ATM and frame relay. Nodes connect to the interlan through communication hubs.


## Communication hubs

The interlan consists of at least one communication hub. Redundancy is provided by having at least two geographically separated hubs, and a redundant individual customer setup on these hubs.

## Route reflector
A route reflector service is provided to keep track of the active communication hubs.

![](Images/Route%20Reflector.png)

## Node

Node layer consists of different local networks interconnected by a network device. There are also one or many connections to the interlan layer for routing to external nodes. Each node belongs to one customer only.

## Interlan connection

The external connection to interlan can be formed in numerous ways such as through customer infrastructure and the internet.

![](Images/Interlan%20Connection.png)

Through a divided part of satcom bandwidth services such as encryption and WAN optimization can be provided by the satcom provider. The node network device gets a dedicated link to the satcom modem on-site.

![](Images/customer%20node.png)

Direct link to communication hub

A direct link between the node network device and the communication hub is preferred whenever suitable. Customer separation is handled either by the communication hub or VLAN-separation through a trunk. This connection form requires a physical secure and controlled environment. Preferably, an environment controlled by Kongsberg.

## Node security zones

The node is separated in different security zones and represents different security levels. Kongsberg global IP address plan is designed to handle up to eight security zones.

## Management

Network devices are centrally managed, Traffic related to management is separated in a dedicated network security domain. The following are the main management services:

* Monitoring
* Configuration management
* yslog collection
* Certificate enrolment / Certificate revocation list

## Public Key Infrastructure (PKI)

All communication is authenticated and encrypted by Kongsberg controlled PKI regime. In addition, PKI is also the trust-point for customer separation. Certain parts of the certificate-distinguished name (DN) are unique for each logical network and ensures no communication among different networks (customers).
