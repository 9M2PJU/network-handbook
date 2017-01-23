# network-handbook README File
---
# My Notes  



### CompTIA+ Certification  

Entry level certification

### Comptia Network + Objectives N10-006
  
- See PDF
- Navigate to Pearson VUE in For test takers tab (https://home.pearsonvue.com/)
- CompTIA blueprint will list the metadata of the exam
- Not all multiple choice questions
- Passing is 720 and above from scale 100-900

### 1. Network Architecture for CompTIA Network

- Introducing network devices
- Understanding network services and applications
- Configuring network services and applications
- Understanding WAN technologies
- Installing and terminating network cables and connectors
- Differentiating between common network topologies
- Differentiating between common network infrastructures
- Implementing a network addressing scheme
- Understanding routing concepts and protocols
- Introducing unified communication technologies
- Comparing cloud and virtualization technologies
- Implementing a basic network

### Objective 1.1 - Explain the Functions and Applications of Various Network Devices 
- Core connectivity devices
- Security devices
- Special purpose devices

#### Hub
- Works at OSI Layer 1 (Physical)
- Hubs are multiport repeaters
  * Regenerate the signal  
- One big collision domain
- Good for network diagnostics and nothing else

#### Switch
- Successor to the bridge
- Works at OSI Layer 2 (Data Link)
  * Can also function at OSI Layer 3 (Network)
- Switches store an in-memory MAC (aka media access control) table and provide dedicated bandwidth to each port (collision domain)

#### Router
- Operates at OSI Layer 3 (Network)
- Seperate entire networks
- Modular design (especially Cisco)

#### Wireless Acess Point
- Provides IEEE 802.11 connectivity
- Many support Power over Ethernet (PoE)
  * IEEE 802.af specifies 15.4W power
- Wireless LAN controllers
  * Centralized management of many WAPs
  
#### Ethernet Domains

- Hub
  * One collision domain
- Switch
  * Four collision domains
- Router
  * Four broadcast and collision domains

#### Configuring a Router

- VMWare or Virtualbox will allow for creation of computer and aoppliance instances in software
  * Vyos
  
    `$ show int`   
    `$ config`   
    `# set interfaces ethernet eth0 address 10.0.0.254/24`   
    `# save`   
    `# ping 10.0.0.254`   
    `# clear`   
  * Ability to use tab completion with various CLI's
  * NOTE - Always ensure that you save configuration changes. A common beginner's mistake is making configurations and not saving the changes
  
#### Security Devices

- Firewall
  * Exist as software or hardware varieties
  * Selectively allow or block network traffic
    - IP addresses, port numbers - packet-filtering firewall
  * Stateful packet inspection - Identifies sessions and can enforce rules on high level applications and services
  * Serves as a gatekeeper

- Intrusion Detection
  * Intrusion Detection System (IDS) - Passive detection of network traffics
    - Also called NIDS
  * Host-Based IDS (HIDS) - Protects local computer (Tripwire)
  * Intrusion Prevention System (IPS) - Active prevention of network attacks
  * Threat detection often involves signatures and anomolies
  
### Proxy/COntent Filter


  
### Objective 1.1 Appendix

#### Useful Links

- Understanding Network Hubs -> (http://www.techiwarehouse.com/engine/5ea76190/Understading-Networking-Hubs)
- Network Bridges -> (http://compnetworking.about.com/cs/internetworking/g/bldef_bridge.htm)
- Network Switch -> (https://en.wikipedia.org/wiki/Network_switch)
- Difference Between Hubs, Switches, and Routers -> (http://www.webopedia.com/DidYouKnow/Hardware_Software/router_switch_hub.asp)
- How Does a Network Switch Work? -> (http://www.cisco.com/cisco/web/solutions/small_business/resource_center/articles/connect_employees_and_offices/how_does_a_network_switch_work/index.html)
- Networking Basics - What You Need to Know -> (http://www.cisco.com/cisco/web/solutions/small_business/resource_center/articles/connect_employees_and_offices/networking_basics/index.html)
- Router (Computing) -> (https://en.wikipedia.org/wiki/Router_%28computing%29)
- Router Hardware 101 -> (http://lifehacker.com/5830886/know-your-network-lesson-1-router-hardware-101)
- Understanding Routing -> (http://www.enterprisenetworkingplanet.com/netsp/article.php/3607381/Networking-101-Understanding-Routing.htm)
- Wireless Access Point (https://en.wikipedia.org/wiki/Wireless_access_point)
- Access Point, Wireless (http://compnetworking.about.com/cs/wireless/g/bldef_ap.htm)
- Configuring a Wireless Access Point (http://www.dummies.com/how-to/content/configuring-a-wireless-access-point.html)
- Power over Ethernet (PoE) -> (https://en.wikipedia.org/wiki/Power_over_Ethernet)
- PoE Explained -> (http://www.veracityglobal.com/resources/articles-and-white-papers/poe-explained-part-1.aspx)
- Piet Mondrian -> (http://www.theartstory.org/artist-mondrian-piet.htm)
- Collision Domain -> (https://en.wikipedia.org/wiki/Collision_domain)
- Broadcast Domain -> (https://en.wikipedia.org/wiki/Broadcast_domain)
- Collision Domains vs. Broadcast Domains -> (http://ciscoskills.net/2011/03/30/collision-domains-vs-broadcast-domains/)
- Collision & Broadcast Domains -> (http://study-ccna.com/collision-broadcast-domain)
- VMware Workstation -> (http://www.vmware.com/products/workstation)
- VMware Solution Exchange (Virtual Appliances) -> (https://solutionexchange.vmware.com/store)
- Oracle VM VirtualBox -> (https://www.virtualbox.org/)
- VyOS Virtual Router -> (http://vyos.net/wiki/Main_Page)
- Firewall (Computing) -> (https://en.wikipedia.org/wiki/Firewall_(computing))
- Stateful Firewall -> (https://en.wikipedia.org/wiki/Stateful_firewall)
- What is Stateful Inspection? -> (http://www.webopedia.com/TERM/S/stateful_inspection.html)
- HIDS/NIDS -> (http://searchsecurity.techtarget.com/definition/HIDS-NIDS)
- HIDS -> (https://en.wikipedia.org/wiki/Host-based_intrusion_detection_system)
- NIDS -> (https://en.wikipedia.org/wiki/Intrusion_detection_system)
- IPS -> (https://en.wikipedia.org/wiki/Intrusion_prevention_system)
- Tripwire HIDS -> (http://www.tripwire.com/)
- Proxy Server -> (https://en.wikipedia.org/wiki/Proxy_server)
- Content Control Software -> (https://en.wikipedia.org/wiki/Content-control_software)
- Websense Content Filter Appliance -> (https://www.websense.com/content/v-series-appliances.aspx)
- Using the PING Command -> (https://technet.microsoft.com/en-us/library/cc737478(v=ws.10).aspx)
- Using NSLOOKUP -> (https://support.microsoft.com/en-us/kb/200525)
- Traffic Shaping -> (https://en.wikipedia.org/wiki/Traffic_shaping)
- Blue Coat Traffic Shapers -> (https://www.bluecoat.com/products/packetshaper)
- Load Balancer -> (https://en.wikipedia.org/wiki/Load_balancing_(computing))
- F5 Networks Load Balancers -> (https://f5.com/glossary/load-balancer)
- Meaning of 'RTFM' -> (http://www.internetslang.com/RTFM-meaning-definition.asp)
- Rack Unit -> (https://en.wikipedia.org/wiki/Rack_unit)


