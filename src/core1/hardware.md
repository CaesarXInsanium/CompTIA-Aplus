# Section 3: Hardware

## 3.1 Copper Network Cables

- Cable is fundamental for network communication. There is only one chance to
  do correct installation
- Twisted Pair
  - Balanced pair operation. Two wires transmit equal and opposite signals
  - Transmit+, transmit, receive +, receive --
  - Twist keep interference minimal. Constantly moving away from interference. Opposite
    signals are compared to each other at the end
  - Different pairs have different twist rates

### Cabling standards

- AA (Electronic Industries Alliance)
  - Alliance of trade associations
  - Georgia
- TIA (Telecommunications industry association)
  - Standards, market analysis, trade shows, government affairs
  - Anticholinergic
- International SIP /ICE 11801 cabling standards
  - International version

#### Cobber cable categories

| Category    | Maximum Supported Ethernet standard | Maximum supported distance|
|--------------|------------------------------|------------------------------|
| CAT 3       | 10BASE-T                            | 100 Meters               |
| CAT 5       | 100BASE-TX                          | 100 meters               |
| CAT 5e      | 100BASE-TX                          | 100 meters               |
| CAT 6       | 10GBASE-T                           | 37-55 meters             |
| CAT 6a      | 10GBASE-T                           | 100 meters               |

### Cable Protection

- No plenum: air circulation in drop ceiling of building.
  - Aside from ventilation
- plenum: building air circulation. Heating and air conditioning
  - fire hazard and fume hazard, one wires go on fir
  - plenum rated cable uses DEP or low-smoke PVC in order t
                reduce risk of fumes
  - traditional cable jacket uses PVC that release fume
                when burnt
  - plenum rated is not as flexible. Safety precautions i
                more important. Worst case planning

### Un-shielded vs Shielded Cables

- UTP: un-shielded twisted pair
  - No additional shielding other than the PVC. Most common pair cabling
- TSP: shielded twisted pair
  - Additional protections protect against interference
  - Can shield individual pairs or overall cable.
  - Cable must be grounded
  - -U = PUT, -S = braided shielding, -F = foil shielding
  - Braided: around entire cable
  - Foil: around the cable and no shielding around the pairs is the F/UT
- Termination
  - AA/TIA-568-B
    - Eight conductor 100-ohm balanced twisted pair cabling
  - T568A and T568B
    - Different pins assignments for 8P8C connectors
    - Assigns the T568A pin-out to horizontal cabling
    - T568B more commonly used by organizations.
    - Do not terminate with opposite pin outs.
    - A: W, G, WO, B, WB, O, W Br, Br
    - B: WO, O, W, B, WB, G, W Br, Br
- Coaxial Cables
  - Two or more forms share the common axis
  - GR-6 used in television/digital cable
  - GR-59 used for something and something

### Fiber optic Communication

- Transmission by light: visible spectrum. Allows for very high speeds
- Difficult to monitor/tap into without breaking. Longer communication distances
- Slow degradation. Immune to radio and electrical interference
- Core of glass with cladding covered in coating
- Multi mode: light bounces inside the core with the cladding as it travels
  - Shorter range fiber
  - Uses cheaper light source. LED
- Single mode: long distance communication. 80 km without help
  - Uses more expensive light source like laser

### Video cables

- VGA
  - DB-15 connector: DE-15. 15 pins inside the connector.
  - Uses color blue as result of standard
  - Send analog signal. Degradation after 5-10 meters
- HDMI" HIGH DEFINITION MULTIMEDIA INTERFACE
  - Video audio stream
  - 20 meters distance max dropout after wards
  - 19 pin type a
  - Mini HDMI type c.
- Display Port
  - VASE standard. Royalty free. Data sent in packets form
  - Compatible with HDMI/DIV. Can use passive adapter
- DIV. -- digital visual interface
  - Single dual link: 60 and 85 fps
  - DIV-A: analog signals
  - DIV-D: digital signals
  - DIV-I: both

### Multipurpose cables

- Lighting
  - 8 pin digital signals. Apple propriety
  - Higher power output than micro-USB. Can be inserted either way
  - Simpler design and greater durability
- Thunderbolt
  - High speed serial connector. Can send power and data
  - V1: uses display port
  - V2: uses aggregated channels. Uses mini display
  - V3: 40 gits. Max 3 meters. Allows daisy-chaining.
- USB
  - Universal serial bus. Simplifies connections
  - USB 1.1: low speed and full speed
  - USB 2.0: 480 bits
  - USB 3: super speed. 5 gigabits at 3 meters
  - A plug, b plug, mini-b plug, micro-b plug
  - USB-c plug.
  - USB 3.1: super speed plus. 10 git/s
  - USB 3.2: up to 20 git/s
  - USB-c: can be plugged into two methods. Does not grantee USB 3.1. Must support
    the standards
- DB-9
  - Serial cable connector. Has different sizes
  - Sends serial data over rs-232
  - Serial communication standard. Uses as console as management port

### DATA cables

- Peril AT attachment
  - 1.0: 1.5 gits.
  - 2.0: 2.0gbit/s
  - 3.0: 6 gits.
  - 3.2: 16 gits.
  - SATA drives have both the data and power sections.
- PARA cables
  - Parallel AT attachment. PC/AT
  - Create 1999.
  - Allows for the connection two different storage devices other than hard drives
  - Two drives supported on single connection. Addition cables needed for more
  drives
  - One pin then to be missing in order to allow for the cable to only be able to
    connect one way
- SCSI drive cables
  - Small computer systems interface.
  - Created to string many peripherals into single cable controller. Max 16 devices
  - Multiple formats, parallel and serial devices
  - Created before USB, the USB of the old times
  - Well supported in enterprise, support present in virtual machines
  - All devices in SCSI bus had separate ID number.
  - Logical units are defined within single SCSI ID
  - Serial attached SCSI SATA devices have no jumpers, terminators and settings
  - Moved from parallel to serial
  - Point to point connection, no termination required
  - Control and management of SCSI

### Adapters and Converters

- Allow conversion from interfaces to others as long as they are compatible
- Convert from one format to another: IE Ethernet to USB
- Can be temporary or permanent
- DIV to HDMI
  - Electrical compatible
  - No signal conversion, no loss of video quality
- DIV to VGA
  - Analog signals, backwards compatible. 640x480 resolution only
  - May only need adapter
  - Converter required for digital signal
  - USB to Ethernet

## 3.2 Connectors

- RJ 11
  - 6 position 2 conductor
  - Telephone connection cable
  - Might have 4 wires but not likely, but used interchangeably
- RJ 45
  - 8 position 8 conductors
  - Similar to jr 48c
  - Use with t1/wan data lines
- RS-232
  - Serial connection, recommend standard 232
  - Built for modem communication,
  - Use as configuration port, serial console interface
  - De-9
- BN connector
  - Bayonet Weill conformance
  - Twist to lock cable, circular connector, used on coaxial cables
  - Rigid bulky
  - Ds3 wan links
  - Diff
- F connector
  - Used in cable television, cable modem
  - Rf-6, gr-59. Twisting cable.
- USB
  - A, b, mini-b, micro-b, c
  - Type-C connectors are relatively small and can be connected either way
- Lighting
  - 8 pin digital signals, simple durable design
- SCSI interface
  - Different types, many pins are lot of pings.
- E data
  - Has ears and square. Sara has l shaped
- Rolex connector
  - 4 pin peripheral power connectors
  - 12v AMD 5v power for older components
  - Power supply has different mole connectors

## 3.3 Overview of Memory

- Random access memory, RAM is not hard drive/storage
- Data and programs can only be used when moved to RAM
- Slots
  - Sections to install RAM modules
  - Memory types/standards have changed over the years
  - One of the most important components of computer
  - Check motherboard documentations
- DIMM
  - Dual inline memory module
  - Electrical contact are different from each side.
  - 64 bit data width,
- SODIMM
  - Small outline dim, half size, used for laptops
  - Needs constant refreshing, in order to keep integrity of the data
  - Any piece of memory can be accessed at any type. Different from older
- Dram
  - Synchronous dram, synced with the common system clock
  - Classic dram does not wait for clock signal
  - Dr syncs however many times the system clock rate. Sr sync s one per system clock
  - This determined how many times per cycle can data be accessed.
- DDR
  - Ddr2: twice as fast. Not compatible with DDR slots
  - Ddr3: wise as fast as ddr2. Maximum size 16 GB per dim. Not backwards compatible
  - Ddr4:speed increases, maximum of 64gb per dim. Not backwards compatible
  - Each version has different keys a slot that only allow the correct version
    to be installed on the slots.
- Memory technologies
  - Multi channel memory
  - Dual channel triple, quad
  - Use to increase performance of computers.
  - Memory modules should match. Exact is the best. Increase throughput
- Self checking
  - Used in critical systems: cm servers, database, things that are important
  - Parity memory adds parity bit that detects error but no correction
  - ECC detects and corrects errors. Not all systems use this

## 3.4 Storage Devices

### Storage Types

- Optical formats
  - Small bumps are read with a laser beam.
  - Microscopic binary storage,
  - CD-ROM(compact disk ROM). 7000 megabytes
  - DVD-ROM(digital versatile disk) 4.7 GB, 8.5 dual layer
  - Blu ray-disc: 25 GB single, 50 GB dual layer
  - Writing to optical media, burners don't crest bumps, darken photosensitive dye
  - Cd-re
  - DVD-R/RE. Dual layer
  - Blu-ray disc recordable. BD-RE
- SSD
  - Non-volatile memory, no moving parts
  - Very fast performance, no spinning drive delays
  - 2.5" SATA interface.
  - m.2 interface. Smaller form factor. No DATA or power cables. Faster than DATA
    compatibility.
    - B key, m key, b and m key. Certain m.2 with support both.
    - B key: pice x2
    - M key: pice x4. Will be faster than b. use for lanes fl pice

- HDD
  - Non-volatile magnetic storage. Rapidly rotating platters. Random access,
  - Moving parts: platters, actuator arm. Mechanical components limit the access
    speed. Mechanical
                    components can break
  - Faster rotating speed mean lower reading latency average
  - H
  - Hybrid drives
  - Solid std hybrid drive. Both spinning drive and dds as cache. Allows for increase
    in speed without added cost of SSD
  - Uses same form factor.
- USB flash drives
  - EEPROM: electrical erasable programmable read only memory
  - No volatile memory. No power required to retain data
  - Limited number of writers.
  - Not designed for archival storage. No good for backup
  - Secure digital
  - Compact flash drive

### RAID

- Data redundancy
- Drives storage large amounts of data. HDD have moving components, they will eventually
  break
- How to secure data if drive breaks
- Create array of drives
- RAID: redundancy array of independent disk: inexpensive disks
- Different raid levels. Some redundant others not. Sue correct
- Software based RAID
- Feature of the operating systems.
- Not special hardware controllers. Slower performance
- Hardware based raid
  - Feature of the hard drive controller
  - Configure outside the OS, invisible to OS
  - High performance designed for speeds. Higher costs
- Hot swap-able drives
  - Add and remove while the system OS is running
  - Drive chassis: two or more drives
  - Easy to repair, combine with RAID for 100% uptime
- RAID 0: striping
  - File blocks are split between two or more physical drives
  - High performance, data is written quickly,
  - No redundancy, drive failure will break array. Single drive failure is complete
    failure
- RAID 1: mirroring
  - File blocks are duplicated, between two or more physical drives, high disk
    utilization, every file is duplicated
  - If one drives fails exact duplicate is still available
- RAID 5: striping with parity
  - File block are stopped. Along with parity block. Requires at least three discs
  - High redundancy. Data is available after drive failure
    - Performance affected due to data reconstruction
    - Nested RAID: RAID 1+0: RAID 10: strip of mirrors
    - Speed of stripping, redundancy of mirroring, best
of both worlds.
    - Mirror of each set of blocks. Needs at least 4 identical drives

## 3.5 Motherboard

### Form Factors

Determined by physical size, case sizing, has basic layout. Room for small changes.
Which motherboard for which purpose

- ATX
  - Advanced technology extended, created by inlet in 1995
    - 20-24 pin connector for power
    - 4/8 CPU power.
    - Larger form factor
- Micro-ATX
  - Smaller version, less expansion.
  - Backward compatibility, similar mounting points, similar power.
  - Actively manufacturing.
- ITX
  - Series of low power. VIA technologies 2001. Screw compatible with ATX
  - Single purpose computing. Streaming media.
- Mini-ITX: same as normal ITX but even smaller.

### Bios Security

- BIOS Security
  - Bios password
    - skips step from starting, needs password to start OS
    - Supervisor password: restrict BIOS changes. BIOS configurations
- Full disk encryption
  - Complete encryption. Including OS
  - Bit locker in Windows: RPM integration
- TPM: trusted platform module. Can be added to motherboard. Built into systems.
  Add advanced cryptographic function
- Lo jack for laptops. Track location of laptops. Built into BIOS. Reinstall itself
  if OS is installed. Phone home function. Remote lock of laptop
- Secure boot
  - only available in UEFI. Digitally sign known-good software. Cryptographically
    secure.
    Software won't run without proper signature
  - Available in Windows/Linux

### BIOS Updates

- Updates to firmware. No volatile memory software.
- Computer BIOS, GPU, game console.
- Fix bugs and increase performance
- Not usual to part of maintenance. Upgrade for specific reasons
- In windows section Bios version in System information
- Compare to existing version. Keep backup
- Before upgrading
  - Some updates are bland
  - Check for new features
  - Located power source reliable
  - Try UPS
- Modern upgrades are executable. Most upgrade apps will check for prerequisites.
  Require reboot, save documents and backup
- Newer options can be available
- Multiple BIOS versions, upgrade from USB flash drive possible depending on motherboard

### CPU Features

- Multiple cores increasing all the time. All cores have independent cache. L3 may
  be shared
- CPU die: unique for each model
- CPU cache:
  - High speed memory, holds data instruction and results
  - Different levels of cache
  - Level 1: first check
  - Level 2: secondary data.
  - Level 3: still on the on chip share across cores
- Virtualization: run other operating systems within single hardware platform. Share
  physical hardware components
  - Performance and hardware management challenges. Software based is limited
  - Virtualization extensions added to processor
  - VT for inlet
  - AMD-v for AMD
- Hyper threading
  - Run multiple thread concurrently, one core can act like two. Waiting on data
    to load, and other thread can be processed. Requires CPU support
- Speed: real speed.
  - Gigahertz, is billions of cycle per second
  - Actual speed has to take into account clock speed, CPU architecture, bus speed,
    bus width, l1 cache, l2 cache, OS support
  - Not good measure for performance
- Overclocking
  - Increase speed rate past the rated value,
  - More power required, produces more heat, at certain point system becomes unstable
  - Needs CPU/motherboard support.
  - Change the base system clock. Needs unlocked CPU
  - Run stress test to conform stability
  - Will void warranty?
- Integrated GPU
  - Graphics processing united. Part of video adapter, motherboard or CPU
  - Graphics rendering requires separate dedicated GPU
- Intel vs AMD
  - Differences are subtle
  - AMD is usually cost less
  - Laptops have large choices with Intel.
  - Intel is now value and AMD is performance but has decent value still

### CPU cooling

- Case fans
  - Cool air is pulled through the persona computer, most common method of cooling.
  - Check for good airflow
  - Motherboard and layout must be checked for location
  - different sizes and styles
- On-board fans
  - Designed to cool an entire adapter card
  - Can be bulky, usually seen on high-end Gaming PCs
- Fan specifications
  - Has standard sizes
  - Different speeds, higher speed for higher heat output
  - Variable noise levels.
- Heat sink
  - Designed to dissipate heat trough thermal conduction
  - Fins increase the surface are to transfer heat to cooler air
  - Thermal past creates good conduct for proper transfer of heat
- Fanless/passive
  - No noise/ single operations
  - Specialized servers, TV set box.
  - Functions are very controlled for low heat put. Low power component
  - CPU s usually component that generates the most amount of heat
- Liquid cooling
  - Coolant for high-end computing
  - Overclocking cooling
  - Requires cooler with proper cooling capabilities

### Expansion Cards

- Extend the functionality of computer
- Simple process designed for end user installation
- Install hardware and drivers for OS
- Check adapter card documentation
- has minimum requirements, support forums
- May need drivers before/afters installation
- Driver installation
  - Check manufacturer website for updates to drivers
  - Uninstall previews device drivers
  - Manual installation trough Windows device manager
- Onboard video
  - Allows for use of integrated graphics of CPU
- Video cards
  - High-end video capabilities for video games,
    rendering, accelerator
- Audio cards or analog/digital signals
- Network cards: multi-port Ethernet, super high
  speed Ethernet
- USB expansion: add additional USB ports
- Storage cards:
  - ESTATE: plug in external DATA drives

## 3.6 Peripherals

- Printer
  - Physical output from computer, paper documents, photos
  - All in one. Printer, scanner, copier, fax
  - Connects via USB, Ethernet, wife, Bluetooth
- Scanner
  - Take printed document into electric document
  - Connection via wife or USB.
  - Flatbed: can scan single sheet at a time
  - May include automatic document feeder
- Bar code/QR code reader
  - Connection via USB or wife
  - Software can be downloaded with mobile devices for
- Display
  - Output in visual form for human understanding. Many standards.
  - Sizes and resolutions
- CR Headset
  - Determines what one sees. Shows only virtual world and can allow for control
  - X,y,z axis detection
  - Gaming, education, art, travel
- Optical drive
  - Read and store into optical mediums, CD, DVD, blew-ray
  - Read only media. Common for video distribution
  - Limited storage sizes,
- Mouse
  - USB connection, PS/2 adapter.
  - Most common is optical mice which has little moving parts
- Keyboard
  - Connect via USB, or wireless. Special keyboards/button might require software
    and drivers
- Touch pad
  - Integrated device into keyboard. Allows for mouse replacement. Does not need
    to move around
- Signature pad
  - Allows for signing with small digitizer. Connect via
USB.
- Gaming
  - Game pad, joystick. Use mostly
- Webcam
  - Video capture. Can also include audio and video capabilities
  - Laptops usually have webcams built into the device
- Microphone
  - Usual for devices with no/insufficient microphones. USB
- Speaker
  - Analog output devices. Connect via YRS jacks
  - Allows for speaker output
- Headset
  - Headphones and microphones
  - Desk and mobile use
  - Wireless/Bluetooth
- Digital projectors
  - Not always LCD.
  - Metal halite lamp. Very bright but very hot. Brightness measured in nits.
  - Very expensive
  - Always let bulbs cool. Fans will run after shutting off.
- External storage
  - Small devices that connects to computer that have portable storage
  - different connectivity
  - Very mobile, can be security concern
- KVM switch
  - Keyboard video and mouse. Use multiple computers with single keyboard and mouse
- Magnetic reader
  - Point of sale terminal
  - Method of payment. Integrated circuit built into credit card
  - Magnetic strip reader to slide down
  - Reader is USB connected
- NFC
  - Mobile device payment method built into many devices
  - Con tactless payments
- Smart card reader
  - Embedded circuitry
  - Useful form of authentication, username, password, smart card
  - Can be built in or external via USB

## 3.7 Computer Power

ALWAYS DISCONNECT FROM POWER SOURCE WHEN SERVICING DEVICE
SOME DEVICES STORE CHARGE IN CAPACITORS. DISCHARGE THEM

- Power supply
  - Pc uses DC power to do things. Supply converts AC power to DC
- Amp and Volt
  - Ampere: the rate of electron flow past point in one second
  - Voltage: electrical pressure of electrons
  - Watts: measurement of real power sewage
  - Volts \ amps = watts

### Current

- AC power
  - direction of current constantly reverses. Distributes electricity over long distances
  - Frequency varies per country
- DC power
  - Current moves in one direction with constant voltage
- Dual voyage power supply can manually switch between different volts. Measure
  with multimeter
- Auto-switching will do this automatically.
- Do not connect 115v power supply to 215v outlet

### Power Supplies

- 24-pin mono power
  - Main mono power:
  - 20 pin was original TAX standard.
  - You can connect 24 pin connector to 20 pin motherboard
  - Some keys in motherboard to allow for connection only one way
  - Use as little as force necessary to connect

- Power supply output
  - Different voltages for different components
  - Positive or negative voltage is difference in potential using electrical ground
    as common reference point
- Constant power supply
  - +12v pice adapters, hard drive motors
  - +5v motherboard components
  - +3.3v m.2 slots, RAM slots, motherboard logic circuit
  - -12v integrated LAN, serial ports
  - -5v available for IS adapters, most cards didn't use it. Modern PCs lack this
- Sizing power supply
  - Power supplies rated by watts
  - Size depends on usage case
  - Physical is relatively standard. Propriety sizes used for pre-builds
  - Calculate the watts required for all the components
  - Video radiators are usually the biggest power draw.
  - 50% capacity good rule of thumb

### 3.8 Custom Computer Systems

- Graphics works station
  - CAD, CAM
  - SAD high speed storage
  - High-end video
  - Maximum RAM
- Audio/video editing
  - Specialized audio and video, HQ audio, powerful video
  - Large fast hard drive SAD
  - Dual monitors
- Virtualization
  - Maximum RAM.
  - Maximum CPU cores. Constant processes
- Gaming PC
  - SAD storage
  - High-end video/ socialized GPU
  - High definition sound card
  - High-end cool: high utilization for long time
- ANS
  - Connect to network and can be accessed from anywhere in network
  - File sharing/media streaming
  - Gigabit INC for fastest transfer
  - RAID array, redundant HDD
- Standard thick client
  - Desktop application load from local storage and run on local CPU
  - Meets recommend requirements for OS
- Thin client
  - Applications are executed on remote server
  - Virtual desktop device
  - Local devices is keyboard, mouse screen
  - No huge memory and CPU needs.
  - Solid network connection

## 3.9 Common Devices

- Thin client
  - Very little configurations, provides connection to
  server where real work is done
  - Minimum client configuration, little maintenance required
  - Minimal OS
- Thick client
  - Traditional computers with all the requirements
  - Local resources are used, OS, drivers, applications
    - Ongoing support, security patches, OS system updates
  - Account setup
    - Centralized account management.
    - Microsoft Active directory
    - Thin client requires no local permissions required.
    - Thick client the device needs to be added to Microsoft domain. User authentication
      to gain access to thick client
  - Laptop
    - Thick client that moves. Add additional administrative covers
    - Touch pad configuration
    - Synchronization and backup. Cloud based or local drive
    - Wireless connections' mobility in office and elsewhere
    - VAN connectivity, local drive encryption.
  - Phone/Tablets
    - Mobile device management.
    - Touchscreen configuration. Lock codes and biometrics
    - Applications installations set by policy and requirements
    - Synchronizations and backup
    - LPNs and wireless connections

## 3.10 Multifunction Devices

### SOHO

- Small office home office
- Multifunction dices: Printer, scanner, fax, network connection, phone line connection,
  print from the web
- Printer drives are specific to printer model. For Model, OS, and current version
  of OS for the drivers. 32 bit vs 64 bit
- Duplex
  - Printing ob both sides of pages to manually flip the
    paper.
- Collate
  - Print multiple copies in proper order. Useful for large documents
- Configuration
  - Portrait vs landscape. Printer compensates. Quality for resolution, color, Grey
    scale and color saving
- Wired device
  - USB connection. Type b is most common.
  - Can use JR 54, serial, VGA
  - Db-25 parallel connection.
- Wireless device sharing
  - Bluetooth, limited range. Perfect for SOHO
  - Wi-Fi 802.11 via the access point: infrastructure mode
  - Ad hoc mode has not accessed point direct link between wireless devices
  - Device sharing
    - Integrated print server, prints directly to the
printer. Jobs are queued on printer.
    - Web based front end and client utility
    - Cloud printing to send print jobs to printer
  - Sharing OS
    - Via network ports and IP address to identify the
                printer cor configurations
    - Bonjour is for apple and allows for discovery of
                printers in LAN
    - Air print allows for printing from iOS devices
  - Printer data privacy
    - Everyone can print but restricted management
    - Set rights and permissions
    - Print and scan caching. Spool file and caching until
                print job is at top of queue

## 3.11 Printers

### Laser printers

- Combine laser, charged ions, powdered ink, heat and
  paper
- Very high quality and fast printing speeds
- Very complex different parts that can break
- Cost more due to more printer memory
- Imaging drum
- Image is drawn into photosensitive drum. Picks up toners to transfer toner to paper
- Fuser assembly to apply heat and pressure to melting toner into page
- Transfer belt and roller. Cyan, yellow magenta and black
- Is transferred into the paper
- Pickup rollers to pickup paper. Should be singl page at a time.
- Should be periodically cleaned and maintained
- Separation pad: pull just the top sheet from the paper tray. Small and inexpensive
- Duplexing assembly: allows to print on both sides of paper. Two-step process
- Steps
  - Processing: print jobs are sent into memory. How to print paper is processed.
    Must be rendered in memory
  - Charging: charge drum with negative ions.
  - Exposing: use laser to print image on drum
  - Developing: toner get into neutralize sections.
  - Transferring: transfer toner to page.
  - Fusing: heat and pressure to melt toner and fuse to paper
  - Cleaning: clean toner off toner
- Maintenance
  - Replace the toner cartridge: look for messages.
    - OPC drum is photo sensitive. Keep in bag
    - Remove packing strips from new drum
  - Maintenance kit
    - Moving parts have heat and pressure. Swap out all the moving parts
    - Manufacturers provided maintenance kits
    - Page counter allows for scheduling t maintenance.
    - Power down and replace components
    - Reset page counter when down.
    - Print out test page to allow for color calibration. To adjust to density.
      Can be automatic or manual
- Cleaning
  - Toner and paper dust
  - Check manufacturers recommendations
  - Water and IPA
  - Outside: damp cloth
  - Inside -- wipe dust away
  - Don't use normal vacuum cleaner

### Ink jet Printers

- Ink dispersion printer, relatively inexpensive,
- Quiet, high resolution/color
- Relative expensive ink, propriety ink.
- Ink is not permanent. Clogs easily.
- Ink cartridge:
  - Place drops of ink into the page
  - CMYK: cyan magenta yellow, key(black)
  - Print head
  - Some consumer printers integrate the print head into the ink cartridge
  - Some can have them separated
- Ink
  - Feed roller
  - Pick up and feed paper through the printer
  - Must be cleaned and maintained regular
  - Duplexing options available for certain models
- Cartridge and belt
  - Ink cartridges are moved over the paper
  - Belt moves the cartridges back and forth. Moving part
- Calibration
  - Align nozzles to the paper. Lines should be crisp and color should align
  - Look at alignment page to check line and color calibration
- Maintenance
  - Cleaning print heads
  - Might have small droplets of ink.
  - Clogged heads are a big issue. Many printers clean every day.
  - Output might have streaks or sections of missing color
  - Automated cleaning process.
  - Cleaning process can be started manually
  - Check for clogged print heads.
  - Replacing ink-jet
    - Separate colors for each. Certain cartridges might combine
    - Takes seconds to replace
    - Recycle by sending to manufacturer
  - Clearing jams
    - Lots of turns and twists. Jam is inevitable
    - Remove tray paper
    - Remove paper from the path. Form pressure don't rip
    - Check for loose scraps
- Calibration
  - Check output after replacing cartridge. Align nozzles to paper
  - Printer includes calibration option

### Thermal printers

- Use white paper that turns black when heat using special paper
- Very quiet, only moving parts are used to push paper.
- Paper is sensitive to light and heat. Generally the papers fades over time
- Feed assembly: pull paper through the printer. Designed to be replaceable
- Heating element: no moving print head. Head certain
sections at a time
- Thermal paper covered in chemical that changes
colors when heated
- Thermal paper must match model of printer
- Maintenance
  - Thermal replacement
  - MUST GET CORRECT Size and type
  - Different sizes, keep list of proper of models
  - Actual replacement is easy/fast.
  - Impossible to substitute for correct type
- Cleaning
  - Liquid cleaner IPA, get cleaning pen, check manufacturers recommendations
  - Swab gently
  - Can use a cleaning card and paper pathways.
  - Blow printers to remove debris. Avoid use vacuums unless designed for computers

### Impact printers

- Print heads with small matrix of pins
- Presses against ribbon to make mark on paper.
- Good for carbon/multiple copies
- Low cost per page. But very noisy.
- Low resolution output. Use for letters and numbers
- Dot matrix print head: moves back and forth and pins are pushed across the paper
- One matrix, head must move across the paper
- Printer ribbon: modular case the contains enough ribbon. Easy to replace
- Propriety size, must fit printer model to replace
- Tractor feed: paper pulled through the holes
- Paper through the holes with the side of the paper. Holes must line up perfectly
- Maintenance
  - Ribbon replacement
  - Single ribbon. Self-contained one long circle.
  - Replace when the ink becomes too light. Ink is eventually consumed.
  - Specific to model to when replacing
  - Print head
  - Takes a lot of abuse, directly hits the ribbon and the paper.
  - Gets very hot, let it cool
  - Designed to be modular and replaced
- Paper
  - Not as easy in laser printer. Paper feed must be perfect to for holes
  - Forms must be positioned correctly. Text may need to fit predefined space
  - Paper must feed without constraint

### Virtual and 3D printers

- No physical output. Creating digital documents.
- Used to be sent electronically
- Print to file
- Saved file to printable format. Uses file format specific to be opened by printer.
- Command line necessary
- Print to PDF
  - Portable document format. One way path from application
  - Propriety adobe format. Requires software to create view
  - PDF reader built into internet browsers
- Print to XPS
  - Microsoft XPS. Similar to PDF
  - Available on all Windows back to XP
- Print to image
  - Uses graphics image file format. For image editing and sharing
  - Third party software is used to do this
- 3d printer
  - Take electronic model and create physical model
  - Additive manufacturing create object layer by layer
  - Rapid prototyping. Design and create.
  - Display designs anywhere in the world. Or space
