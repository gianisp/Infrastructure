# Layered approach
The network design is segmented into two main layers. The interlan layer provides site-to-site connectivity and the node layer handles connections to adjacent networks within the node.


# Interlan
One of the key features of the interlan layer is the customer separation mechanism. This mechanism ensures that there is no communication between nodes belonging to different customersand, all communication is encrypted. The layer can utilize a broad variety of communication carriers, such as internet, satellite communication, serial lines, ATM and frame relay. Nodes connect to the interlan through communication hubs.


# Communication hubs
The interlan consists of at least one communication hub. Redundancy is provided by having at least two geographically separated hubs, and redundant individual customer setup on these hubs

# Route reflector
A route reflector service is provided to keep track of active communication hubs.

# Node
The node layer consists of different local networks interconnected by a network device. There are also one or more connections to the interlan layer for routing to external nodes. Each node belongs to one customer only.

# Interlan connection
The external connection to interlan can be formed in numerous ways.
Through customer infrastructure and the internet.

Through a divided part of satcom bandwidth
Services like encryption and WAN optimization can be provided by the satcom provider. The node network device gets a dedicated link to the satcom modem on-site.

Direct link to communication hub
A direct link between the node network device and the communication hub is preferred whenever suitable. Customer separation is handled either by the communication hub or VLAN-separation through a trunk. This connection form requires a physical secure and controlled environment. Preferably an environment controlled by KONGSBERG.

# Node security zones
The node is separated in different security zones, which represents different security levels. The KONGSBERG global IP address plan is designed to handle up to eight security zones.

# Management
The network devices are managed centrally. Traffic related to management, will be separated in a dedicated network security domain. These are the main management services:

* Monitoring
* Configuration management
* yslog collection
* Certificate enrolment / Certificate revocation list

# Public Key Infrastructure (PKI)
All communication is authenticated and encrypted by a KONGSBERG controlled PKI regime. In addition, PKI is also the trust-point for customer separation. Certain parts of the certificate-distinguished name (DN) are unique for each logical network and ensures no communication between different networks (customers).
