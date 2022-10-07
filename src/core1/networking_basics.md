# Section 2: Networking Basics

## 2.1 Ports and Protocols

- Protocols used to efficiently transfer large amounts of data for different applications
- IP is protocol that usually transmits the data over the internet using encapsulation.
- Multiplexing: multiple functions inside of single network
- TCP: Transmission Control Protocol
  - connection oriented. Formal setup and close
  - reliable form of deliver. Recovery for errors, manage out of order messages
  - flow control. Receiver manages how much data is sent
- UDP: User Datagram Protocol
  - connection less, no formal or close to connections
  - unreliable delivery. No error recovery, no reordering of data
- IP: internet protocol. Delivery truck methodology to data. All devices that connect
  to networks have IP and MAC address.
- Non-ephemeral port number: assigned to specific application (0-123)
- Ephemeral port number: 1024 to 65535. Determined real time by client
- Most servers are non-ephemeral
- Port numbers are for communication not security. Active port numbers must be known.
  PCT application used different ports then DUP

| Name   | Port Number | Description |
| ------ | ---------------- | ------------------------- |
| FTP    | TCP/20 active, TCP/21 | Used for transmission of files |
| SSH    | TCP/22 | Encrypted communications and remote          |
| Telnet | TCP/23 | Test format remote access and |
| SMTP   | TCP/25 | Simple mail transfer         |
| DNS    | UDP/53 | Domain names services        |
| HTTP   | TCP/80 | No secure web pages         |
| HTTPS  | TCP/423 | Secure web pages           |
| POP    | TCP/110 | Mail receiving protocol    |
| IMP    | TCP/143 | Mail receiving protocol    |
| RD | TCP/3389 | Remote desktop protocol. single application or entire desktop |
| SB     | TCP/137 Net Bios, UDP/138 data gram service, TCP/139 session service | Service message block. Used by Microsoft software for file sharing, printer sharing. Also called IFS |
| FP     | TCP/548 | Apple file sharing protocol |
| ALP    | TCP/427, UDP/427 | Service location services |
| CPD    | UDP/67, UDP/68 | IP network assignment |
| LDAP   | TCP/389 | Lightweight directory access. Store and retrieve information in network directory |
| SPASM  | DUP/161 queries, UDP/162 traps | Simple network Management Protocol. V1 not secure, v2 is secure and support bulk transfer, v3 has encryption and authentication process |

## 2.2 Network Devices

- NIC: Network Interface Card
  - Basic interface for network applications. All devices connected to networks
    have some sort of NIC
  - Specific card required for different mediums: WIFI, Ethernet
  - Generally built into device
- Repeater
  - Receives and repeats signals. No decisions
- Hub: multi-port repeater
  - Incoming traffic is repeated across all ports. Functions as multi-port repeater
- Bridge: switch with 2-4 ports
  - Forwarding decisions based on MAC address
  - connects different network architectures, example: Ethernet to WIFI
  - PAW is example of bridge
- Switches
  - Application specific integrated circuit
  - forwarding based on MAC address
  - Many ports and features: core of enterprise networks
  - Multi-layer switches can forward based on IP address
  - Unman aged Switches have basic forwarding, plug and play. Low price point
  - Managed switches: configure CLANS, interconnect with other switches
    - traffic prioritization based on application
    - Redundancy support structure
    - Spanning tree protocol TSP
    - External management for administration and troubleshooting
- Router
  - Makes forwarding decisions based on IP address. Each port on router is separate
    network.
  - Can connect LAN’s, LAN's and internet
- PAW
  - Wireless access point is not router nor switch, it is bridge. WIFI
- Wireless LAN Controller
  - Centralized management of AP's trough single pane of glass
  - Allows for deployment of new access points
  - Performance/security monitoring
  - Configuration and updates
  - Cloud based solutions exists with no dedicated hardware options available
- Firewall
  - Two types hardware and software based. filter traffic by port number only.
    PSI layer 4
  - Filters based on application, encryption download/upload.
  - Can be used for proxy traffic, PSI layers
- Cable Modem
  - Allows for connection to broadband/cable service provider
  - Uses DOC SIS (Data over Cable Service interface)
  - 4 bit/s to 250 bit/s. gigabit speeds possible
- SLD modem
  - ADSL: Asymmetric Subscriber Line, uses telephone line to bring internet connection
  - Download speed is almost always faster than upload.
  - Significant dependence on distance from distribution center/office for actual
    throughput
- Path Panel
  - Cables go trough the wall and ceiling to path panel to network closet
  - Combination of punch down blocks and Rh-45 connectors
  - Allows for cabling to be done in one go. Path panel changes can be administered
    whenever needed.
- PoE: Power over Ethernet
  - Allows for delivery of electrical power to be delivered over Ethernet connections
    requires specialized switches and/or power injectors alongside appropriate devices
    to support POE
  - Used by phones, cameras, AP's,
- EP: Ethernet over power
  - Allows for power line communication over existing power lines. Allows for Ethernet
    network installation without cable installations.
  - 500 megabits/s
  - Used by adapters, smart energy devices, intra-building networks and vehicles

## 2.3 SOHO Networks

### Installing SOHO Network

- SOHO Router: all-in-one device. Integrated router, switch, PAW, firewall
- Routing via WAN and SLD port. Route between internal network an outside network
- Minimal configuration required. Automatic by connecting appropriate devices
- Allows for wireless management. Configure frequencies, security protocols, IP
  addressing
- Can integrate enterprise level security

### SOHO Firewall

- Every SOHO router has integrated firewall
  - DMZ: ports can be configured to allows unrestricted access. However best practice
    is to declared rules for forwarding
- NAT: Network address Translation. Allows for more devices to connect to outside
  internet than there are addresses available. Converts internal private IP address
  to public address.
  - Static: one-to-one mapping. Best for internet access to internal network device.
    Does not usually change
  - Dynamic: maps internal IP to single public IP address form NAT pool of IP addresses.
    Varies between availability of public addresses
  - PAT (Port Address Translation): router makes the forwarding decisions based
    on port numbers between external and internal. Afterwards it changes the port
    number to the destination

### Other Terms

- Port forwarding: 24x7 access to service hosted internally. External port maps
  to internal host
- UPnP: universal plug and play. Allows devices to automatically configure and find
  other network devices.
  - Applications can use this but requires option to be supported.
- IoT: internet of things. Home/building automation, wireless devices. Management
  and security concerns. But makes things convenient
- Content Filtering: filters content IP, port
  - Whitelist: nothing past firewall except for defined items
  - Blacklist: everything allowed except for defined items
- MAC Filtering: allows for communications to be blocked based on MAC address
- Wireless: best practice to use, highest level of encryption available. WPA2 over
  WPA. WPA better than PEW.
- QoS: quality of service. Change priority of traffic types. For voice, gaming, web,
  streaming, etc. must be chosen carefully in enterprise setting

## 2.4 Wireless Standards

### 802.11/WIFI

- Standard Managed by IEEE LAN/MAN
- All standards are tested many times
- Lower frequencies offer lower speeds but longer range
- MIM: multiple input multiple output. Uses multiple antennas
- Channels: groups of frequencies than can be numbered. None should be overlapping
  if possible
- Bandwidth: how much of the frequencies in use

| Name/Version | Speed | Release Date  | Things of Note |
|--------------|-------|---------------|----------------|
| WIFI 1/802.11a | 5 GHz/54 bit/s | October 1999 | Released alongside b |
| WIFI 2/802.11b | 2.4 GHz/11 Bits/s | October 1999 | More channels
| WIFI 3/802.11g | 2.4 GHz/54 Bit/s | June 2003 | Increased channel bonding |
| WIFI 4/802.11n | 2.4 or 5 GHz 600 Bit/s | October 2009 | 8 MU-MIM. Multi-user |
| WIFI 5/802.11ac | 5 GHz/6.8 Bit/s |  January 2014 | Backwards compatibility
|WIFI 6/ 802.11ax | N/A | N/A | N/A |

- Bluetooth
  - Radio high speed PAN. Connects various devices
- RID:
  - radio frequency IP. Tags for tracking and personal authentication. Inventory
    tracking, pet tracking. RD signals powers the tag
- NFC
  - near field communication. Uses RID. Credit cards and communication
- Zig bee
  - open standard for 802.11.4PAN. less energy than Bluetooth and WIFI, longer distances.
    Used in mesh network. IoT communication standard
- Z-wave
  - propriety home automation. Uses mesh network. IoT communication standard

### Cellular Network Communications Technologies

Uses cellular technology that separates sections of land covered by antenna named
cells. Each antenna covers area with certain frequencies

- 2G:
  - GAM: Global System for Mobile Communications
  - CDMA: Code Division Multiple Access
  - Only has support for voice communications
- 3G:
  - Provided internet connectivity
- 4G:
  - Converged GAM and CDMA providers. Used EDGE (Enhanced Data Raters for GAM Evolution)
  - Support for up to 150Mbit/s. 300 Bit/s LET
- 5G
  - Next generation. Launched in 202 but with limited availability

## 2.5 Network Devices

- Web Server
  - Responds to browser requests for HT PP/S uses HTML
  - Web pages are stored in server then sent out on request. Static pages are download
    completely and dynamic pages are built in real time
- File Server
  - Used as centralized storage. Uses SB. Front end standards handle complexity
- Print Server
  - Provides connectivity to printer devices over network. Usually built into the
    printer itself
- CPD
  - Automatic IP configuration server. Built in router or managed central server
- DNS
  - Dedicated server to store domain names and their IP addresses. Usually managed
    by the enterprise network or ISP
- Proxy
  - Intermediate server that makes request to externs services on behalf of client
    and then provides results back to client
  - Examines information before handing back to client
  - Access control content management
- Email Server
  - Store and send email on behalf of client.
- Authentication server
  - Provides authentications and centralized management. Used in enterprise setting.
    Has built in redundancy
- SEMI
  - Security information and event management
  - Provides logging for all devices and servers
  - Log aggregation and storage. Can provide alerts
  - Allows for viewing of mapping and correlation
  - Forensic analysis, gathers details on events
- Slog
  - Standard message logging, integrated into SIM
  - WORM drive technology. Write once read many. Allows for secure logging to protect
    security logs
- IDS and IPS
  - Intrusion detection/prevention
  - Exploits, cross-site scripting, buffer overflows and other vulnerabilities
  - Alarm and alert or can allow for prevention
- All-in-one security application
  - Next-generation firewall. Unified threat management
  - Many features. Spam filtered
  - Can act as router and switch
- Endpoint management server
  - Manage all devices from single console and scripts
  - Software, driver installation. Security updates
  - Remote troubleshooting
- Legacy systems
  - Old and very important systems. Very relevant to work setting
  - Embedded systems: purpose-built devices, can have direct access to OS

## 2.6 IPv4 and IPv6

- IPv4
  - Is usually primary IP protocol
  - Subset mask allows for varying sizes of networks
  - Each device must have default gateway for access to outside network
- IPv6
  - Link-local: non rout able local network address
  - Uses fe80::/10. Last digits are used from the MAC address in device for uniqueness
  - First half is network address. Second half is device address. Allows for further
    subnetting but not needed due to large number of addresses
  - Has 128-bit address. Very large number of address and networks
- PSI layer 3 address
- DHCP: process for automatic IP configuration
  - 1> discover: devices sends CPD broadcast. Port 68. Router can forward CPD request
  - 2> offer: CPD server receives request and sends offer of IP address
  - 3> request: client sees IP address and officially makes request for that address.
    If multiple offers, then first received is used
  - 4> acknowledgement: server sends acknowledgement to client and self-configures
- BOOT: older version of CPD. Did not configure everything.
  - Static address: address manually assigned by user. CPD reservation can allow
    IP address reservation via MAC address
  - APIPA: link-local address. Communicate inside of subset but to outside.
    169.254.0.1 to 169.254.255.254
  - IP uses
    - SAL VAN/TS: PCT 443
    - Avoids most firewalls
    - No VAN clients
    - Has authentication
    - Can be run inside server or can be configure to OS
    - Also referred to as client-to-site VAN. Create encrypted tunnel. Requires
      separate software
  - LAN: group of devices that shared broadcast domain. Share same switch
  - CLAN: logical separation of networks into different broadcast domains. Reduces
    number of switches necessary. Devices cannot communicate to devices in separate
    LAN's

## 2.7 Internet Connection Type

- Broadband
  - Transmission of communication over multiple frequencies.
  - Allows for multiple traffic types.
  - Data on cable: DOC SIS (Data over Cable Service Interface Specification)
  - High speed: 4 Bit/s to 250. Gigabit possible
- SLD Modem
  - ADSL(Asymmetric Digital subscriber lines)
  - Uses existing land phone technology
  - Need LAN needs to be physically close to provider. 100 ft. closer to office
    faster the connection speed
  - 53 Bit/s down, 16 Bit/s up common
- Dial up
  - Uses voice telephone lines.
  - 56 knit/s. compression to t320 knit/s
  - Very slow, no scalable. Used in legacy systems. Network utility. Emergency connective
- Fiber
  - Fiber optics to the home. Converged services: voice, video, data
  - Enhanced features. Gigabit speeds easy. Allows for
- Satellite
  - Communication to a satellite. Send data to and from satellite. Very high ping
    but high throughput.
  - Allows connection to remote/rural site.
  - Very sensitive to bad weather
- WISD
  - Integrated services digital network
  - BREE: basic rate interface (2b +d)
    - 2 54 knits/s bearer B
    - One 16 knit/s signaling D. management information
  - PRO: primary rate interface
  - Delivery over T1 or E1
  - Commonly used from the PTS to large phone systems
- Cellular
  - Mobile devices: many antennas place into areas of land called cells
  - Tethering allows for sharing of internet connection to other devices
- Line of sight services
  - Uses high frequencies
  - Visual path between antennas. Common in metropolitan areas.
  - Options available for none-line-of-sight.
  - WiMAX network uses microwaves to send connection

### Network Types

- LAN
  - Local area network. Local is relative. Building or group of buildings
  - Ethernet and 802.11 wireless
- WAN
  - Wide area network. Spanning globe. Connect LABS across distance
  - Point to point serial. Terrestrial and non-terrestrial
  - Can be slower than LAN
- PAN
  - Personal area network. Bluetooth, IR, NFC…
- MAN
  - Metropolitan area network. Larger than LAN smaller than WAN
  - Managed by central provider or government. Own right of way
- WEN
  - Wireless mesh network. Internet of things
  - Mesh cloud. For connections
  - Self-form automatically. Self-heal: reacts automatically to changes
  - 802.11, Zig bee, z-wave

## 2.8 Network Tools

- Cable Crimper
  - Pinches modular connector to wire, Ethernet
  - Metal prongs are pushed through insulation. Plug permanently pressed into cable
    sheath
  - Best practices: get good crimper, cable snips, wire stripper. Use correct modular
    connectors. Practice
- Multimeter
  - AC voltage. Check wall outlet voltage.
  - DC voltage. PC power supply output voltages. COS battery power
  - Continuity, cables fuse status, wire mapping
- Tone generator
  - Follow the tone to track a specific wire.
  - Tone generator plays sound. Probe listens to audio and alerts
  - Allows for easy wires tracking.
- Cable tester
  - Continuity test. Crosses wires, missing pins
  - No testing for crosstalk, signal loss
- Loop back plugs
  - Useful for testing physical ports. Different plugs for serial, RS-232
  - Ethernet fiber, T1,
  - Not cross over cables
- Punch down blocks
  - Punch wire into wiring block. Each wire must be punched individually punched
  - Tools trims wires.
  - Documentation is key. Try to keep the twists
- WIFI Analyzer
  - Analyzer hears everything. Purpose built hardware or mobile device add-on software.
    Uses 802.11
  - Identify errors and interference
