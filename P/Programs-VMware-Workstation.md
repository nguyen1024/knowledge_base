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
  
## Convert Version

## Screenshot

## How to Boot into BIOS

Add the following to the ".vmx" file.

```
bios.forceSetupOnce = "TRUE"
```

Source

- Accessing the BIOS when the POST screen clears too quickly (1004129)
  - https://kb.vmware.com/s/article/1004129
- How to Increase the VMWare Boot Screen Delay
  - https://www.howtogeek.com/howto/16876/how-to-increase-the-vmware-boot-screen-delay/
