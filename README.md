# sys-virtio-drivers
VirtIO Drivers are paravirtualized drivers for kvm/Linux (see http://www.linux-kvm.org/page/Virtio). In short, they enable direct (paravirtualized) access to devices and peripherals for virtual machines using them, instead of slower, emulated, ones.

Description
------------
Fix for incorrect Windows RAM reporting on the Proxmox/KVM Platform.

Requirements
------------

- Windows 2012r2 server

Role Variables
--------------

See default/main.yml for detailed information.

Example Playbook
----------------

This is an example how to use the role:

    - hosts: ad-members
      become: true
        
      roles:
        - sys-virtio-drivers

Source(s)
---------
- https://pve.proxmox.com/wiki/Windows_VirtIO_Drivers
- https://www.caretech.io/2018/05/30/proxmox-and-windows-server-2016-ram-reporting/
