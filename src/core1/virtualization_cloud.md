# Section 4: Virtualization and Cloud

        ◦ 4.1 Cloud
            ▪ Models
                • IaaS: Infrastructure as a Service
                    ◦ Hardware as a service
                    ◦ Provide hardware to run applications but end user is responsible for installation and management and security and even OS
                    ◦ Data is in infrastructure but still within end user control
                    ◦ Common implementation is web server. 
                • SaaS: Software as a Service
                    ◦ On demand software: no local installation. 
                    ◦ Email distribution, payroll software, 
                    ◦ Central management of data b y third party provider
                    ◦ Complete application of offering. No developing required
                    ◦ Gmail
                • PaaS: Platform as a Service
                    ◦ No server no software no team
                    ◦ Someone else handles platform. End user handles development
                    ◦ No direct control of data, people. Infrastructure
                    ◦ Managed by trained security professionals. Put building blocks together. Develop app from available platform
                    ◦ Salesforce.com: SaaS modules for control from customers
                • Cloud deployment
                    ◦ Private: private virtualized local data centers. All costs maintained by single entity
                    ◦ Public: available to everyone on internet
                        ▪ AWS, Azure
                    ◦ Hybrid: mix of public and private
                    ◦ Community: several organizations share the same resources
                        ▪ Shared resources, underlying infrastructure. Metered costs or up front costs
                    ◦ Metered and non
                        ▪ Metered: pay for everything done, cost to upload, store, download
                        ▪ Non-metered: flat costs for everything for block of storage
                    ◦ Characteristics
                        ▪ Rapid elasticity. Scale up and down as needed from the usage
                        ▪ On demand self-service. Adding software networks, servers and storage is challenge. Instant resource provisioning. 
                        ▪ Resource pooling. All of computing power in one place. One large resource instead of many small resources. Virtualize any and all smaller servers and resources. 
                        ▪ Measured service. Cost of utilization are very closely tracked. Resource planning and granular change-backs
            ▪ Services
                • Email
                    ◦ Email is staple. Detailed electronic communication
                    ◦ Of site is Challenge of maintenance. Expensive hardware and storage
                    ◦ Cloud base email hosting is flat cost. Personal options have no direct cost except with data
                    ◦ Gmail
                • Storage
                    ◦ Store files in the cloud. Access share and edit
                    ◦ Collaborations for files and access
                    ◦ Synchronization app. Store files in the local drive. App synchronized to the cloud. 
                    ◦ Gmail, Dropbox, one drive, box
                • Virtual application streaming
                    ◦ On demand applications. Started is streamed down
                    ◦ Components are download as needed. Unused components will not be downloaded. 
                    ◦ After use all files are saved and upload. Easy to update. Update from single location
                    ◦ Mobile phones and tablets can be streamed and use the applications without installation. 
                    ◦ Online advertisements. 
                    ◦ Applications for laptops and desktops. New apps can be added as needed and updated
                • Virtual desktops
                    ◦ Users connect to pre-built desktop. Log in to VDI to use their desktop
                    ◦ Access from any OS. Via web browser
                    ◦ Virtual NIC, all communication ins the desktop are local to the virtual desktop. No sensitive information sent from local device
        ◦ 4.2 Client Side Virtualization
            ▪ Virtualization
                • One computer multiple operating systems
                • Separate OS, CPU, memory, network.
                • Host based virtualization is normal desktop plus others
                • Standalone server that hosts virtual machines
                • Existed since 1967
            ▪ Hypervisor
                • Virtual machine manager
                • Requires CPU that support virtualization. But some software can support without hardware support
                • Hardware management of virtual OS
            ▪ Resource requirements
                • Intel: VT, AMD: AMD-V
                • Sufficient memory, for host and guests, storage and network
                • Can use standalone, NAT, bridged. Allows for virtual switches
            ▪ Emulation vs virtualization
                • Virtualization is native OS
                • Emulation is one device running processes designed for completely different architecture
                • Code Is interpreted for running on current hardware. Slower than running native
            ▪ Security
                • Sweet for bad-guys. Control of hypervisor is control of guest OS
                • VM escaping: malware recognizes that it is inside of a virtual machine and compromises the hypervisor. Can jump between guest OS
                • Many hosted services are virtual environments malware on one customers server can gather information from others
                • Very rare
            ▪ Guest security
                • Same controls and security as local machine
                • Lo0k out for rouge virtual machines. 
                • 3rd party VMs are dangerous. Only run trusted virtual machines
            ▪ Network requirements
                • Most client side virtual machines managers are virtual internal networks
                • NAT is used. Shared network address
                • Bridged network address allows for direct connection to local network
                • Privates address allow it to only contact other virtual machines
        ◦ 5.1 Trouble shooting
            ▪ Change control
                • Change management: formal process for managing change in systems
                • Nothing changes are without process. Plan for changes. Determine risk of change
                • Recovery plan for if change does not work positively. Test before change
                • Document all steps
            ▪ Steps to troubleshooting
                • Identity problem
                    ◦ Information gathering, get as many details as possible
                    ◦ Duplicate issue if possible. 
                    ◦ Identify symptoms, question users
                    ◦ Determine if anything change has occurred. Check records, environment changes and infrastructure changes.
                    ◦ Gather log files. 
                    ◦ Approaches multiple problems individual level
                    ◦ Perform backups. 
                • Establish theory
                    ◦ Start with the obvious. 
                    ◦ Consider everything.
                    ◦ Make list of all possible causes. Begin with the easiest problems to test first
                    ◦ Research knowledge base. Google search
                • Test theory
                    ◦ Determine theory. 
                    ◦ Re-establish theory
                    ◦ Call an expert to fix the problem
                    ◦ 
                • Evaluate theory
                • Establish plan of action
                • Implement plan
                • Verify system functionality
                • Document findings
