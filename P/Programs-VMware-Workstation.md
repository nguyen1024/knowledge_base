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

Increase memory.
