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

# intro to vRealize Automation




