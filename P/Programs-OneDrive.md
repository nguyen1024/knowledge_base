# Programs - OneDrive

## How to Clear Up Space

- Open Command Prompt, not PowerShell.
- Go to the to your OneDrive folder.
- Enter the following command.

```
attrib -p +u * /s
```

| Switch | Description                              |
| ------ | ---------------------------------------- |
| -p     | Clears the Pinned attribute.             |
| +u     | Sets the Unpinned attribute.             |
| /s     | Process the files in subfolders as well. |

Source

- Use “attrib” to pin and unpin files and folders for OneDrive On-demand sync in Windows 10
  - https://www.theexperienceblog.com/2017/09/26/use-attrib-to-pin-and-unpin-files-and-folders-for-onedrive-on-demand-sync-in-windows-10/
- Is there a way to observe a file's 'availability status' via Windows command?
  - https://stackoverflow.com/questions/58184531/is-there-a-way-to-observe-a-files-availability-status-via-windows-command

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

## ... Startup...

If OneDrive does not start automatically, check Settings > Startup.

Source

- OneDrive doesn't start automatically with Windows 10 Pro
  - https://answers.microsoft.com/en-us/msoffice/forum/all/onedrive-doesnt-start-automatically-with-windows/3571a76f-f396-47b9-b35c-3ee8fd2a7b70
