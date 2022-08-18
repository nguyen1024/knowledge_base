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
