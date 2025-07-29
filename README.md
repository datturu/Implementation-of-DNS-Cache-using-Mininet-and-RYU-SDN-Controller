**Enhancing Network Performance with DNS Cache in Ryu SDN Controller using Mininet**
**Overview**
This project aims to improve network performance by implementing an efficient DNS cache within a Software-Defined Networking (SDN) framework. We address the issue of slow DNS resolution times for frequently accessed domain names, which causes delays and depletes network resources. Our solution uses the Ryu SDN controller in a Mininet virtual environment to internalize DNS requests, thereby speeding up query responses and enhancing overall network efficiency.

**Key Goals**
Reduce DNS Resolution Times: Optimize the process of translating domain names to IP addresses.

Implement DNS Cache: Develop and deploy a robust DNS caching system within the SDN architecture.

Enhance Network Performance: Improve user experience, reliability, and overall network efficiency within the SDN domain.

**Technologies Used**
Software-Defined Networking (SDN): Centralized control and programmable infrastructure.

Ryu SDN Controller: An open-source, Python-based controller for managing virtual networks.

Mininet: A network emulator for creating virtual network topologies for testing.

DNS (Domain Name System) & DNS Cache: Core internet infrastructure for name-to-IP translation, with caching to speed up repeated queries.

BIND9: Open-source DNS server software used for DNS services.

Oracle VirtualBox & Ubuntu: Virtualization platform and guest operating system for the environment setup.

Proposed Approach
We set up a virtualized environment using Oracle VirtualBox with Ubuntu. Within this, Mininet creates a virtual network topology. The Ryu SDN controller is then integrated to manage network flows and specifically implement the DNS caching mechanism. Python scripts are used to define the topology and control the DNS caching logic.

**Challenges Faced**
During implementation, significant version compatibility issues arose between Mininet, Ryu, and Eventlet (a concurrency library). These hurdles highlight the importance of careful version management and thorough testing for seamless integration in SDN environments.

Testing Procedure
Execute a Mininet topology script.

Connect the Ryu SDN controller script to integrate DNS caching.

Access Mininet hosts via xterm.

Use nslookup or dig multiple times to verify DNS query caching and improved response times.
