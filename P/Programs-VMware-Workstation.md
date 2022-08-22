# Programs - VMware Workstation

## Keyboard Shortcuts

Move Focus Out of Virtual Machine

- Alt + Control

Move Focus Into Virtual Machine

- Control + G

Switch to Fullscreen

- Move focus into virtual machine.
- Alt + Control + Enter

Exit Fullscreen

- Move focus out of virtual machine.
- Alt + Control + Enter

## How to Exit Unity

Exit Unity Mode

- Click on the VMware Workstation Task Bar icon.
- Click on the "Exit Unity" button.

Reference

- Use Unity Mode
  - https://docs.vmware.com/en/VMware-Workstation-Player-for-Windows/16.0/com.vmware.player.win.using.doc/GUID-8C477788-7700-4030-8C4A-039C02AABB74.html

## ?

Reference

- Errors when booting Ubuntu: SMBus Host Controller not enabled! - Failed to connect to lvmetad - Falling back to internal scanning
  - https://communities.vmware.com/t5/VMware-Fusion-Discussions/Errors-when-booting-Ubuntu-SMBus-Host-Controller-not-enabled/td-p/450289
  
## How to Convert Version

To do.

## How to.. Screenshot

To do.

## How to Boot into BIOS

Add the following to the ".vmx" file.

```
bios.forceSetupOnce = "TRUE"
```

The folowing does not seem to work because the system goes straight to the GRUB menu.

```
bios.bootDelay = "15000"
```

The following keys do not seem to work because the system goes straight to the GRUB menu.

- F2 to enter SETUP
- F12 for Network Boot
- ESC for Boot Menu

Source

- Accessing the BIOS when the POST screen clears too quickly (1004129)
  - https://kb.vmware.com/s/article/1004129
- How to Increase the VMWare Boot Screen Delay
  - https://www.howtogeek.com/howto/16876/how-to-increase-the-vmware-boot-screen-delay/
- vmware workstation - How can you boot from CD?
  - https://superuser.com/questions/940427/vmware-workstation-how-can-you-boot-from-cd

## Mobile Phone Hotspot

- Virtual machine bridged mode.
- Or attach a USB network adapter and connect it to the virtual machine.

Source

- VM use phone hotspot
  - https://communities.vmware.com/t5/VMware-Workstation-Pro/VM-use-phone-hotspot/td-p/964677

## ... Shared Folders...

No solution... yet.

Source

- Shared folders not available on Linux guests after upgrading to VMWare Workstation 15
  - https://communities.vmware.com/t5/VMware-Workstation-Pro/Shared-folders-not-available-on-Linux-guests-after-upgrading-to/td-p/1404693

## How to Change the Boot Order

Sometimes you can't change boot order through the BIOS becuase it is says it is under supervisor control. Even when you set the supervisor password, you can't change the boot order.

```
bios.bootOrder = "cdrom,hdd"
```

Source

- Changing the boot order of a virtual machine using vmx options (2011654)
  - https://kb.vmware.com/s/article/2011654

## How to Set the Number of Processor Cores

- (CPU sockets) x (CPU cores) x (threads)
- If you have Hyper-Threading, then you have two threads.
- If you have twice the number of logical processors as cores, then you have Hyper-Threading.

Source

- Setting the Number of Cores per CPU in a Virtual Machine
  - https://www.nakivo.com/blog/the-number-of-cores-per-cpu-in-a-virtual-machine/
- How to Check if your CPU supports or is using Hyper-threading?
  - https://www.thepcinsider.com/how-to-check-cpu-supports-using-hyper-threading/

## How to Fix Fuzzy Chrome Extension Menus and Tab Previews on a Second Screen

Increase memory?

## Snapshots

- How to take a snapshot in VMware Player
   - https://communities.vmware.com/t5/VMware-Workstation-Player/How-to-take-a-snapshot-in-VMware-Player/td-p/2828612
   - You can't in Player. Only in Pro. 

## ...

> A full clone is an independent copy of a virtual machine that shares nothing with the parent virtual machine after the cloning operation. Ongoing operation of a full clone is separate from the parent virtual machine.
> ...
> A linked clone is a copy of a virtual machine that shares virtual disks with the parent virtual machine in an ongoing manner.
> ...
> All files available on the source machine at the moment of the snapshot continue to remain available to the linked clone. Ongoing changes to the virtual disk of the parent do not affect the linked clone, and changes to the disk of the linked clone do not affect the source machine.

- Full and Linked Clones
  - https://docs.vmware.com/en/vCenter-Converter-Standalone/6.2/com.vmware.convsa.guide/GUID-93894315-EFCA-4DD8-B583-FA24272DA180.html 

## Host Only Network... With Internet Access

- VMWare - How do i configure Host Only Network with a custom Gateway?
  - https://stackoverflow.com/questions/68625447/vmware-how-do-i-configure-host-only-network-with-a-custom-gateway

## VMware Files

I don't think that you need to backup VMEM files.

> Log files – Log files are just that- a log of virtual server activity for a single virtual server. ... Log files should be used only when you are having trouble with a virtual machine.
>
> VMDK files – VMDK files are the actual virtual hard drive for the virtual guest operation system (virtual machine / VM). You can create either dynamic or fixed virtual disks. With dynamic disks, the disks start small and grow as the disk inside the guest OS grows. With fixed disks, the virtual disk and guest OS disk start out at the same (large) disk. For more information on monolithic vs. split disks see this comparison from sanbarrow.com.
>
> VMEM – A VMEM file is a backup of the virtual machine’s paging file. It will only appear if the virtual machine is running, or if it has crashed.
>
> VMSN & VMSD files – these files are used for VMware snapshots. A VMSN file is used to store the exact state of the virtual machine when the snapshot was taken. Using this snapshot, you can then restore your machine to the same state as when the snapshot was taken. A VMSD file stores information about snapshots (metadata). You’ll notice that the names of these files match the names of the snapshots.
>
> NVRAM files – these files are the BIOS for the virtual machine. The VM must know how many hard drives it has and other common BIOS settings. The NVRAM file is where that BIOS information is stored.
>
> VMX files – a VMX file is the primary configuration file for a virtual machine. When you create a new virtual machine and answer questions about the operating system, disk sizes, and networking, those answers are stored in this file. As you can see from the screenshot below, a VMX file is actually a simple text file that can be edited with Notepad.

Source

- VMware File Types Explained: VMDK, VMEM, VMSN, VMSD, VMX & More
  - https://petri.com/virtual_vmware_files_explained/
