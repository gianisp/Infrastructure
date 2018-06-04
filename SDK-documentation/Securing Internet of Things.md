# Overview
Internet of Things solutions in an industrial scale and scenario requires a proven and solid end to end cyber security strategy. KONGSBERG has through years of experience with advanced, distributed automation and control systems acquired valuable experience in the field of securing installations, equipment, sensors and data.

We have developed an end to end approach, following our kognifai IoT reference architecture, segregating components and zones, as well as taking care of the life cycle management of operating long living solutions in the industrial space.

In this article, we will dive deeper into the different zones that include:
*	Devices and sensors
*	Offshore gateways
*	Cloud entry points (gateways)
*	Services

Approaching the security solution by using zones are meaningful not only when speaking of network segregation and access rights, but also for protecting legacy equipment and solutions. Each zone often has its own protocols, authentication methods and data. Zone segregation is also a subject for classification and certification on installations under strict regulations.

Data and access between the different zones are limited and controlled through firewalls, authentication regimes and protocol security.
 
# The Control Zone

The control zone contains the automation and control systems, sensors, and other physical hardware.
Systems in this zone are likely to be using legacy protocols, authentication and can also be under a less frequent software update regime. It is therefore of highest importance to protect this zone from external unintended intervention.
Equipment in this zone can be protected by products like the KONGSBERG Malware Protection System, scanning all network traffic and all USB storage devices entering the zone.
Firewalls protect the zone and controls all traffic leaving it, limiting it to a short listed, secure protocols and applications.
Remote Services and access to PC-s in this zone can be done through certified and operator initiated system like the KONGSBERG Remote Services solution.

# The Server Zone
The server zone typically contains servers for collecting, analytics and distribution of data collected from the control zone.
On installation with several sensors this zone is often equipped with an IoT Gateway device for collecting, analytics, compression and buffering of data before transmitting it to the central cloud IoT Gateway service.
Larger installation in day to day operation the zone can be equipped with application servers for offshore and onboard Performance Management, Decision Support and Condition Monitoring solutions.
The gateway device can be a software client running on existing hardware, a smaller hardware device capable of communicating on serial lines, industrial busses and IP networks or a computer capable of buffering thousands of events per second.
The server zone can be virtualized through virtual networks and can be connected to the cloud gateway through a closed segregated network or by using secure and encrypted protocols.
Both the IoT Gateway and the router are equipped with certificates managed centrally for secure authentication, authorization and encryption.

# The Publish Zone
The publish zone contains any offshore, user facing applications, providing application firewall functionality.

# The Cloud Gateway Zone
The cloud gateway contains the end point for the IoT traffic, receiving data from all authenticated IoT Clients and Gateways, making the data available for consumers in the Service Zone through queues and buffering.

# The Service Zone
All data consuming services, analytics and databases are in the service zone, protecting both data in traffic and at rest.

# Publish Zone
Applications, APIs, distribution and integration solutions are contained in the Publish Zone. The zone is protected by Application Firewalls, DDoS measurements. Access to Apps, APIs and data is controlled by authentication schemes and Identity Management enforcing the correct level of security for the solution and protection level.
