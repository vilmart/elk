elk
===

Practival exercises in the Linux Kernel

Introduction
============

To execute exercises with the Linux kernel will use a virtual machine that is going to use virtualization technology. 
Virtualization implements many benefits but requires greater management complexity.

Fortunately there are many solutions to minimize this complexity and the Open Source world leads this area. 
One such solution is the virt-manager of Red Hat, which simplifies the management of virtual machines, 
which features a command line interface or graphical user interface (GUI).

Installation Virt-Manager
====================

1) Open a terminal and run the command:

       - $ sudo apt-intall virt-manager

After being executed, the command using and enjoying about 22 MB of disk space to install a set of applications virt-manager.

2) As part of the installation, the libvirtd daemon should be running. 
The libvirtd daemon is allowing the connection of virt-manager application with Hypervisor and consequently with the VMs. To check this use the following commands:

       - $ ps ax | grep libvirtd

       - $ which virt-manager

3) Now let's install QEMU, which will be our Hypervisor. To install QEMU run the command:

       - $ sudo apt-get install qemu

4) Now we turn and run virt-manager. To activate and run the virt-manager run the command:

       - $ sudo virt-manager
