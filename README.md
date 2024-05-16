# VMware overview

link to video referred - https://www.youtube.com/watch?v=B_H3TJlbEiw

* VMware allows virtualization of physical servers to virtual servers.
* difference is we do buy a physical server initially but instead of installing windows/linux on it, we install ESXi (VMware's OS). It is basically a hypervisor. So within the physical computer running ESXi, the hypervisor creates VMs or virtual machines or servers.
* the more CPU, more RAM, more storage available in the server/desktop, the more VMs we can build and more resources we can allocate.
* download ESXi, configure it and use it to make VMa via a web browser  vSphere.
* vendor - the company itself is called VMware
* two primary softwares within the VMware stack - 
1. ESXi - hypervisor - standalone
2. vCenter - allows to manage multiple ESXi hosts. allows sharing resources across a pool of hosts. we can move VMs from one host to another. You can clone it and make templates. If one host goes down, VMs automatically start up in another host
* hardware needs to be compatible to install ESxi

# difference btw ESXi and vCenter

link to video referred - https://www.youtube.com/watch?v=FrAjyCdsyhM

* ESXi is a bare metal hypervisor - can run directly on physical server without any underlying OS.
* vCenter server - centralized management plaform for managing multiple ESXi hosts. can be used to create, configure and monitor VMs. provides HIGH AVAILABILITY (restart VMs on an alternate host) and FAULT TOLERANCE (create shadow instance of VM as backup incase of failure). allows VMotion (live migration of VMs between hosts) and Distributed Resource Scheduler for load balancing (DRS). 
* can access vCenter server using vSphere Client.  
* VMware vSphere is a virtualization platform. consists of a family of different software and management tools.

# Templates

* written in YAML
* infrastructure as code (IaC)
* blueprint for previous versions
* drag and drop design canvas for easy design and deployment
* can include user inputs that allow users to choose from various options at deployment time. For example, a blueprint could allow a user to choose the operating system, disk size, or the cloud endpoint where the resource should be deployed.
  
# overview on vSphere and vRealize

* vSphere is VMware’s virtualization platform.
* It transforms data centers into aggregated computing infrastructures that include CPU, storage, and networking resources.
* vSphere manages these infrastructures as a unified operating environment and provides tools to administer the data centers.
* The two core components of vSphere are ESXi and vCenter Server.ESXi is the virtualization platform where you create and run virtual machines.vCenter Server is the service through which you manage multiple hosts connected in a network and pool host resources.

* vRealize Suite is a comprehensive cloud management platform that delivers and manages IT services across private, public, and hybrid clouds.
*  products include vRealize Operations Manager, vRealize Business for Cloud, and vRealize Automation.
*  usecases -
1.  Proactively solving performance issues: It helps identify and resolve performance issues before they impact services.
2. Continuously monitoring and managing capacity: It provides insights into capacity usage and trends to help plan for future needs.
3. Streamlining processes: It streamlines processes with customizable policies, guided remediation, and automated enforcement of standards.
4. Understanding cost and consumption: It provides visibility into the cost and consumption of private and public cloud services

# intro to vRealize Automation

link to playlist referred - https://www.youtube.com/watch?v=K6efEhghKRE&list=PL2OPLXNfWYm_A0FEvlCpG3Iw5ev2ajs6p&index=1

Introduction to VRA

* vRealize is a cloud management platform. An enterprise could have multiple VMs hosted on different cloud platforms offered by different vendors. Inorder to manage these VMs originally we would have to use their dedicated portal. Managing all in a single platform instead - brings us to vRealize.
* multivendor and multiplatform support
* unified cloud management
* self service portal
* acceralated service delivery

Architecture and Components

* two components -
1. vRealize Automation Appliance Components -> linux
2. IaaS components -> windows server



