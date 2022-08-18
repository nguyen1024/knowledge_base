# Programs - Windows Shared Folders

## How to Share Folders

- You might need to set a password on the computer sharing the folder.
- Go to "Control Panel > Network and Internet > Network and Sharing Centre > Advanced sharing settings".
  - Go to "Private".
    - Turn on network discovery
    - Turn on file and printer sharing
- Go to "Turn Windows features on or off.
  - Turn on "SMB 1.0/CIFS File Sharing Support".
  - Turn on "SMB Direct".
  - Restart the computer.

Resources

- How to share files between a Linux and Windows computer
 - https://www.computerhope.com/issues/ch001636.htm#:~:text=Right%2Dclick%20the%20folder%20and,and%20click%20the%20Share%20button.

## How to Delete Mapped Shared Folders

- Select and delete in File Explorer.

Source

- How to delete a mapped network drive from Windows (5 ways)
  - https://www.digitalcitizen.life/how-delete-mapped-drives-windows-7/

## How to Find Out What Folders Are Shared

1. File Explorer
2. Computer Management
3. Command Line

Source

- 3 ways to view your shared folders in Windows (all versions)
  - https://www.digitalcitizen.life/how-view-list-all-shared-network-folders/

## ...

- VMWare VM does not see a Shared Folder
  - https://superuser.com/questions/1714957/vmware-vm-does-not-see-a-shared-folder
  - Some notes on Windows and Linux.
  - There are also some notes on SMB and SAMBA.

```
In Linux terminal write the following command:

1- vmware-hgfsclient *

You should see your shared folder name then write:

2- sudo /usr/bin/vmhgfs-fuse .host:/ /mnt/hgfs -o subtype=vmhgfs-fuse,allow_other

Now you will find your shared folder mounted at /mnt/hgfs
```

- How to Share a Local Folder with a Remote Host Running on VMWare
  - https://www.tecmint.com/enable-share-folder-in-vmware-workstation/amp/
  - Some notes on where the shared folder is in Linux.

```
/mnt/hgfs
```

- 3 Types of Virtual Switches | VMnet0, VMnet8, VMnet1 in VMware 
  - https://www.ubackup.com/enterprise-backup/vmnet-vmware-jkzbj.amp.html 
  - VMnet0 - Bridged
  - VMnet8 - NAT
  - VMnet1 – Host-only

- What is the difference between NAT / Bridged / Host-Only networking?
  - https://superuser.com/questions/227505/what-is-the-difference-between-nat-bridged-host-only-networking
  - Has a nice image of a table of who can talk to who.
  - Notes that virtual machines on the same host only network can talk to each other.
