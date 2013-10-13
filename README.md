elk
===

Practival exercises in the Linux Kernel

Introduction
===========

For our exercises with the Linux kernel, we will use the Ubuntu distribution and virtualization technology. The virtualization technology implements many benefits, but requires a more complex management. Fortunately there are many solutions to minimize this complexity.

One such solution is the virt-manager of Red Hat , which simplifies the management of virtual machines and can be performed in the main Hypervisors free software through a command line interface or graphical user interface ( GUI ).

Installation Ubuntu
===============

Installation virt-manager
===================

1 ) Open a terminal and run the command :

      - $ sudo apt-install virt-manager

After being executed , the command using and enjoying about 22 MB of disk space to install a set of applications virt-manager .

2 ) As part of the installation , the libvirtd daemon should be running. The libvirtd daemon is allowing the connection of virt-manager application with Hypervisor and consequently with the VMs . To check this use the following commands :

      - $ ps ax | grep libvirtd

      - $ which virt-manager

3 ) Now let's install QEMU , which will be our Hypervisor . To install QEMU run the command :

      - $ sudo apt-get install qemu

4 ) Now we turn and run virt -manager . To activate and run the virt-manager run the command :

      - $ sudo virt-manager
      
Creating a virtual machine
==========================

1) To create the virtual machine select and press "Advanced"...

2) Fill in the Name field, select the source of your image/iso and then press "Next"...

3) Select the location of the source of your image/iso, the operating system type, version, and then press "Next"...

4) Fill in values (supported by your physical machine) fields memory and CPUs are assigned to your virtual machine, and then press "Next"...

5) Fill in a value (supported by your physical machine) the field that defines the disk size that will be allocated to your virtual machine, uncheck "Allocate entire disk now" and then press "Next"...

6) Select "Advanced options", select "qemu", select where your architecture then press "Finish".

7) Created virtual machine. Now you need to customize your Linux distribution.

