# Programs - OneDrive

## ... Context Menu...

The Reason

The issue surfaced because I was logged into the PC with the default admin account – the one created when Windows was configured. In my case, this was a virtual machine in Azure, so it was the admin account I configured on the setup screen before provisioning. This means that Explorer was in elevated mode and OneDrive was running in per-user mode.

The Solution

- Open a Windows command prompt (run as Administrator) on the affected computer, and change directory to %localappdata%\Microsoft\OneDrive
- %localappdata% usually means “C:\users\[your username]\AppData\Local\ . It may be helpful to open this folder in Windows Explorer just to find the sub directory you will need.
- What you are looking for is the OneDriveSetup.exe application. In my case, it was in the folder:  %localappdata%\Microsoft\OneDrive\21.150.0725.0001.
- From the Windows command prompt, go into the folder where OneDriveSetup.exe is located.
- Then run this command: OneDriveSetup.exe /allusers

Source

- How to Add OneDrive to the Windows Context Menu
  - https://danielglenn.com/how-to-add-onedrive-to-the-windows-context-menu/ 

## ... Video Formats...

- MKV!

Source

- Video formats you can play on the OneDrive website
  - https://support.microsoft.com/en-us/office/video-formats-you-can-play-on-the-onedrive-website-07c008b2-70e4-4ced-8a9b-f25bed77196a 
