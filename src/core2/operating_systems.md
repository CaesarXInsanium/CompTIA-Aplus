# Section 1: Operating Systems

## Section 1.1: Operating Systems Overview

- Reasons for OS
  - control of interaction between components: memory, hard drive, keyboard, CPU
  - common platform for applications. Executed inside of OS
  - method for humans to interface with computer
- OS features
  - file management: add delete, rename
  - application support: memory management, swap files
  - input and output support, printers, keyboards, hard drivers
  - OS configuration and management tools
- Microsoft Windows
  - largest family of OS; Windows 7,8,10,11
  - large industry support
  - broad selection of OS options.
  - Software support.
  - Large installation base for security explorations
  - large hardware support creates integration challenges
- Apple macOS
  - desktop OS designed for running on Apple hardware
  - advantages, easy to use, compatible with Apple hardware ecosystems
  - requires Apple hardware, less support, higher hardware cost
- Linux -Distros
- no single OS, combination of features and variations are the distrobutions
  - many distros
  - cost free, works on much hardware.
  - Good community
  - limited driver support for non-mainstream hardware, laptops
  - no dedicated support team
  - OS technologies

    - 32 vs 64 bit for the CPU suport.
    - 4gb mas RAM on 32 bit
    - 17billionGB for 64bit. OS has max RAM value
    - hardware drivers are specific to the OS version. Swtichin
            between the two versions
    - 32 bit software cannot run on 64 bit architecture
    - 64 can run 32 bits.

  - Windows on Mobile Device

    - fully feaured tablets. Have touchscreen, keyboard and stylus
    - early versionw as Windows Mobile. No longer support

  - Google Android

    - open handset alliance, based on Linux
    - supported by differente manufacturers
    - android apps are developed on other OS using the android SDK
    - app are also available on third party sites

  - Apple iOS

    - available based onUnix. Closed source. Exclusive to Apple
            products
    - apps created using iOS SDK only on macOS
    - apps must be approved by apple before release to had end
            users installed

  - ChromeOS

    - based on linux and focused on Chrome Browser. Most apps are
            webbased
    - many manufacturors, relatively cheap
    - relias on cloud, connect to internet

  - Vendor limitations

    - end-of-life, update policies,
    - ios, android, windows 10 check and prompt for updates
    - chrome os update automatically
    - there is compatibilatiy between OS's
    - almost no direct application compatibiity
    - many apps have been designed to run on multiple operating
            systems

- Section 1.2: Windows 7

  - basic

    - release on 2009, end of life on 2015
    - similar to windows vista. Increase peformance
    - new fetures compared to vista
    - starter, home basic, home premium, ultimate, preffesional
            enterprise

  - Starter

    - built for netbooks, no DVD or media center
    - no window aero, no interconenction sharing
    - no Iis web server
    - no enterprise technologies, domain conenction, bitlocker,
            EFS
    - only suported 32 bit. Max 2 gb ram

  - Home Premium

    - consumer edition, DVD playback, graphics, interconnection
    - no enterprise technologies
    - support 64bit and 2 CPUs

  - Ultimate

    - complete functionality
    - dommain support remote dekstop, enterprise technologies
    - same as windows 7 enterprise

  - proffesional

    - all home premium, connection to windows domain
    - support desktop host
    - no bitlocker,

  - enterprise

    - sold only in volume license. Multiligual user interface
            packages
    - bilocker drive encryption

  - Hardware requirements

    - 1 ghz proccesor, 1gb RAM 32 bit 2 gb 64 gib
    - 16 gb 32 20b 64
    - directx9 graphics device

- Windows 8 and 8.1

  - Basic

    - release 2012, new user interface, no start button
    - 8.1 was free update. Stadalone version
    - support ended 2018, extemded support to 2023
    - versions: core, pro, enterprise

  - Core

    - basic version for the home, x86 and x64
    - MS account intergration. Windows defender, windows media
            player

  - pro: proffesional

    - bitlocker support, EFS, fiullmdisk and file level
            encryptions
    - join windows domain for IT management
    - group policy support

  - enterprise

    - software assurance customers, full fetures
    - applocker, windows to go, direct access, brachcache
    - all features

  - requirements

    - PAE: physicaly address extension
    - allow 32 bit pcpu to use more than 4 gb RAM
    - NX processor bit for security
    - SSE2: intruction set for thirdparty applications and drivers
    - 1 gb and 2 gb
    - 16gb and 20 gb
    - directx 9 graphics with WDDM compatible driver

- Windows 10

  - released 2015

  - single platform for desktops, laptopos phones, and all in one
        devices

  - upgrade were free for the first year.

  - Windows 10 is a service. Periodic updates to OS. Rolling release
        model

  - Home

    - retail sales, intergration with MS account, one drive backup
    - windows defender
    - cortana: digital assitant

  - pro

    - additional management features, remote desktop host, remove
            control each computer
    - bitlocker, full disk encryption.
    - Join windows domain, active directory

  - education/enterprise

    - very similar with minor differences volume linceses
    - applocker, determine was apps can run
    - branch cache, remote site file caching.
    - Granular UX control. Define user enterprise. Kiosk, control

  - requirements

    - same as Win8, PAE, NX, SSE2,
    - max ram is 129gb home, 2048gb for pro and enterprise

- Windows in the enterprise - features

  - Windows at work

    - large scale support, thousands of devices
    - security concerns, local files
    - working on spreadsheet, vs movies
    - geographical sprawl cache data between sites

  - domain services

    - active directory, large database for network.
    - Distributed architecture, has many servers is no suitalbe
            for hom use
    - everythong is documented in one place
    - authentication and management

  - bitlocker and EFS

    - data confidnetialoty,
    - built into NTFS, rpotect individual files
    - encryption everything.
    - Bitlocker will encryption everythong including OS
    - home and business

  - media center

    - video, music and television portal
    - record shows from tV turner
    - not available on window 10

  - desktops

    - work has standard desktop, common user interface, limited
            customizations
    - home has little if any restrictions

- Section 1.3: Installing Operating Systems

  - Boot -- installation of OS requires boot media

    - USB drive, USB must be bootable, computer must be able to
            boot from USB
    - CD-ROM, DVD-ROM. More common.
    - Use PXE. Preboot executiong enviroment, can boot from
            network interface
    - Netboot allows to install macOS from network

  - boot methods

    - SSD, store os isntallation files
    - external/hot swappable drive
    - some external drive can mount ISO image
    - internal hard drives

  - types onf isntallations

    - unattended installation, answer questions in a
            file(unattened.xml)
    - no installation interruptions, can same time
    - in-place upgrade: maintains applications and data. Changing
            OS files from one to another
    - clean install deletes everything and install new clean OS
    - migration tools can help
    - image, deploys clone on every computer for same
            configurations
    - repair installation, fix problems with OS, does not change
            user files
    - multiboot: multiple OS to boot from on single computer and
            user can change
    - recovery partitions that allows for installation files and
            backtup
    - refresh and restore

  - disk partition

    - seperate physical drive into logical pirces, useful for data
            seperations
    - required for maintaining seperate operating systems
    - called volumes by MS

  - MBR: master boot record

    - primary: bootable partitions, maximun of four primary
            partitions per disk. One of primary partitions can be marked
            as active
    - extended: neccesary for extending partions, can create
            multiple logical partitions
    - extended on bootable

  - GPT: GUID partition table

    - global uniqe identifier
    - requires UEFI BIOS, can have up to 128 partitions
    - does not require extended partitions

  - partitioning

    - may already be partitioned, existing partitions not always
            compatible with the OS
    - BISO-compatible mode disable UEFI secureboot
    - be careful: serious rick for data loss. Not neccesary for
            day to day operations

  - storage types

    - layerd on top of partitions and file systems

    - basic disk storage, basic disk partitions cant span seperate
            physical disks

    - dynamic disk storage

      - span multiple disks for create large volumes.
      - Duplacated data accress physical disks, split data
      - not all windows versions and editions support this

  - file systems

    - foundatoin for files and must be ormatted

    - FAT32 and NTFS can be used by Win10

    - FAT: File allocation table.

      - FAT32 larger volumes, 2 terabytes is maximun volume. 4Gb
                is max file
      - exFAT: microsoft fhash FS,

    - NTFS: NT file system

      - improvement over FAT32. Quotes files compressions,
                encryptions, symbolic links, larger files, security ,
                recoverability
      - CDFS -- compact disk file system. Older standard

    - ext3/ext4: extended file systems used by many linux distros

    - NFS: network file systems allows for access to files over
            network.

    - HFS/HFS+: use by the apple. Replaced by APFS

    - swap partition: use for memory management, frees RAM and
            copiess back to RAM when needed.

  - Format

    - quick: create new file talbe but does not erase data. Not
            check of drive. Create new file table.
    - Full format: writes zeroes to the entire disk. Data in
            unrecorable. Checks for bad sectors, full format

  - other

    - load alternative third party drivers when neccesary
    - workgoup vs business setup. Home vs business.
    - Determined time/data/region/language
    - driver installation software, and updates
    - load drivers, apps and recent updates
    - can create recovery partition for potential OS fixes

  - Installing Windows

    - prepare boot drive

      - is there data in the drive, important data
      - has the drive been formatted, what are the partitions
      - backup old data if neccesary

    - before installation

      - check minimun OS requirements, RAM, Disk space,
      - run hardware compatibility check, run manually
      - plan for installation questions, drive partition
                configuration, licnese keys
      - application compatibility, check with app developver

    - reasons to upgrade

      - keep files in place and only change OS files
      - installation dletes everything and puts in new files
      - maintain consistency customized configurations
      - saves times in configurations and settings managements
      - in place: uipgrade the existent OS. Keeps all the
                applications,
      - clean install: wipe everything and reload everything
      - upgrading windows 10 si easy, just download the relevant
                ISO
      - cannot upgrade between different architectures
      - windows isntallation program is similar between the
                diffferent windows versions
      - windows 10 creates a recovery partition, system
                partitions, and primary installation

    - post installation

      - does it work? Does it boot?
      - Begin the testing,
      - install service packs, patches applications, driver
                updates, application updates

- Section 1.4: Microsoft Command Line Tools

  - Privilages

    - user and administrator. More tasks require standard
            permissions
    - not all users can run administration commands
    - elevated privilages: require being a member of the
            administrators group
    - type help if in doubt: help dir, help chkdsk, help
            \[COMMAND\]
    - command /?

  - copy command

    - copies files from one location to another

  - dir

    - list files and directories

  - cd

    - chage working directory
    - use cd .. to switch to folder above currrent directory

  - shutdown

    - turn of a computer. And can restart.
    - Shutdown /s /t nn : /s shutdown compltely /t wait for
            specific time nn before shutting down
    - shutdown /r /t nn will rebot in nn seconds

  - dism

    - deplyment image service and management tool
    - manage windows imagin WIM images
    - to make changes to image, use this command
    - very complaicated command that has many uses

  - sfc

    - system file checker
    - scan integrity of system files.
    - Can scan and verify only. Can also make automatic repairs

  - check disk: chkdsk

    - /f : check for logical file system errors
    - /r: locates bad sectors and recover readable information
    - requires that no other program is using it
    - can automatically schedule a check for next boot sequence

  - diskpart

    - manage disk configurations and partitions

  - tasklist and tasklist

    - manage tasks from the command line
    - display list of currently runnign procccess
    - can also kill process by PID or executable name

  - manage group policy

    - manage computers in active directory domain, group policy is
            update upon login
    - gpupdate would force GP update on currently runniung
            computer an user
    - gpresult: checks and verifyes the policy settings for
            computer and user
    - gpresult /r

  - format

    - formats disk for use with windows and other file systems

  - xcopy

    - allows for copying of entire directories with /s
    - exp: xcopy /s Documents e:\\backups

  - robocopy

    - better than xcopy, allows for copy process to begin again if
            it is interrupted
    - similar syntax

- Network Command Line Tools

  - ipconfig

    - shows mac address, ip addresseses, default gateway and all
            other network information
    - determine TCP/IP adapter information, DHCP information
    - DNS, IP address, subnet mask and default gateway for all
            adapter information
    - ipconfig /all show everything, more detailed than just
            normal

  - ping

    - test reachabiloty of device, determine round trip tinme
    - uses ICMP protocol for
    - ping 10.0.0.1
    - TTL, shows how many routers there between one point to
            another

  - tracert

    - determine route that packet takes to a destination
    - takes advantage of ICMP TTL messages
    - not all devices will accept ICMP Time exceeped messages,
            firewalls can restrict ICMP protocol or set to lower
            priority
    - not all routes are going to be the same
    - Windows sends ICMP echo requests
    - Linux/Unix/MacOs allow for use of different protocols for
            the trave-route

  - netstat

    - shows network statistics for many operating systems
    - shows outbound and inbound information
    - -a shows all active connections, -b shows binaries, requires
            elevated privilages
    - -n, do not resolve names

  - nslookup

    - look up information on DNS servers
    - allows for testing of DNS configuration and functionality
    - lookup names and addresses

  - net

    - specific for the windows operating system

    - allows for viewing the network resources,

      - net view \\\\servername

    - map network shared drive to drive letter

      - net use :\\\\servername\\sharename

    - view user account information and reset passwords

      - net user username \* /domain

- Section 1.5: Window Administrative Tools

  - Computer management

    - prebuilt management console, allows for mix of predefined
            plugins that allows for customization for specific purpose
            and job
    - control panel/administrative tools
    - mmc.exe
    - handy starting point, events, user accounts, storage
            management, services and more
    - one can start the console all blank and allows for easy
            addition of the other plugins for tools

  - device manager

    - the os does not know how to talk to hardware so that it
            needs the drivers
    - device hardware are hardware specific, windows 7 drivers may
            not work on windows 10
    - common quesiton inf Technical support is "Have you updated
            the drivers?"

  - local users and groups

    - users: can be admin, guest of regular users
    - groups: logical categories of users, each with shared
            permissions and access to different things
    - easy for power users, and

  - local security policy

    - big companies have big security policies, managed trough
            active directory group policies
    - stand alone computers can use active directory, they can
            only have local policies
    - not available in home editions, require education,
            professional or enterprise

  - performance monitor

    - gather long-term statistics, control panel or administrative
            tools
    - OS metrics, disk, memory, CPU etc
    - set alerts and automated actions depending on settings and
            scripts that are set
    - allows for storage to the logs and metrics
    - allows for tracking of many different metrics for traking
            and logging

  -
