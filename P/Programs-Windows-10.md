# Programs - Windows 10

## How to Adjust Images for the Lock Screen

- Use Irfan to resise the image to be within 1920 x 1080.
- Use Irfan to increase the canvas to 1920 x 1080.

## How to Turn Off the Clock

Taskbar settings > Turn system icons on or off > Clock

Source

* How can I hide the clock from Windows 10 taskbar
  * https://superuser.com/questions/1417624/how-can-i-hide-the-clock-from-windows-10-taskbar

## apphostregistrationverifier.exe

* Microsoft Wallet app.
* Groove Music app

Source

* Windows 10 connects to these websites after a clean install
  * https://www.thewindowsclub.com/windows-10-connects-to-these-websites-after-a-clean-install

## Extract WiFi Password

Right Click > Status > Wireless Properties Button > Security Tab > Network security key Field

Source

* How to View Saved Wi-Fi Passwords
  * https://www.pcmag.com/how-to/how-to-view-saved-wi-fi-passwords#:~:text=Right%2Dclick%20on%20your%20computer's,password%20appear%20in%20plain%20text.
* Find your Wi-Fi network password in Windows
  * https://support.microsoft.com/en-us/windows/find-your-wi-fi-network-password-in-windows-2ec74b2e-d9ec-ade1-cc9b-bef1429cb678

## How to Fix Windows 10 Sign-in Options Not Loading

Run "SFC /SCANNOW" in a command prompt.

Source

* Windows 10 Sign-in Options Not Showing/Loading/Working
  * https://www.passmoz.com/windows-10-sign-in-options-not-loading.html

## How to Change Passwords

Settings > Sign-in Options >

Source

* How to Change Your Password in Windows 10
  * https://www.laptopmag.com/au/articles/change-password-windows-10

## How to Prevent F1 Opening Microsoft Edge Web Browser

Off

```
C:\WINDOWS\system32>taskkill /f /im HelpPane.exe
SUCCESS: The process "HelpPane.exe" with PID 13828 has been terminated.

C:\WINDOWS\system32>takeown /f %WinDir%\HelpPane.exe

SUCCESS: The file (or folder): "C:\WINDOWS\HelpPane.exe" now owned by user "GRAYMALKIN-2\Admin".

C:\WINDOWS\system32>icacls %WinDir%\HelpPane.exe /deny Everyone:(X)
processed file: C:\WINDOWS\HelpPane.exe
Successfully processed 1 files; Failed processing 0 files
```

On

```
icacls %WinDir%\HelpPane.exe /remove:d Everyone
icacls %WinDir%\HelpPane.exe /setowner "NT Service\TrustedInstaller"
```

If the 2nd command fails to execute and throws the error:

```
C:\WINDOWS\HelpPane.exe: Access is denied.
Successfully processed 0 files; Failed processing 1 files
```

Then, use the Permissions GUI to change ownership to NT Service\TrustedInstaller.

How to Stop F1 Key from Opening Help (Bing) in Windows 10
- https://www.winhelponline.com/blog/disable-f1-key-help-windows-10/

## ... Lock Screen

- Settings > Lock Screen
- Background > Slideshow > Advanced slideshow settings > When my PC is inactive, show lock screen instead of turning off the screen > Off

Source

- Prevent Windows 10 from Locking When Monitor Turns Off
  - https://superuser.com/questions/1214447/prevent-windows-10-from-locking-when-monitor-turns-off

## ... recent...

- File Explorer > View > Options > Privacy
- Untick "Show recently used files in Quick access".
- Untick "Show recentyl used folders in Quick access".
- Press "Clear".
- Restart the computer.

Source

- Windows 10: How to Find and Clear the All Recent Files List
  - https://winbuzzer.com/2020/04/29/windows-10-how-to-find-and-clear-the-all-recent-files-list-xcxwbt/

## How to Turn of the Windows Timeline

1. Open Settings.
1. Click on Privacy.
1. Click on Activity history.
1. Clear the Store my activity history on this device option.
1. Clear the Send my activity history to Microsoft option.
1. Activity history settings to disable TImeline on Windows 10
1. Activity history settings to disable TImeline on Windows 10
1. Under “Show activities from accounts,” turn off the toggle switch for all your accounts.
1. Jump to another settings page, and then come back to the “Activity history” page to refresh the page and make the option to delete your history available.
1. Under “Clear activity history,” click the Clear button.
1. Click the OK button to confirm.

Source

- How to disable Timeline on Windows 10
  - https://pureinfotech.com/disable-timeline-windows-10/

## Guest Accounts

- Create an account.
- Assign it to the guest group.

Source

- How to Create a Guest Account in Windows 10
  - https://www.laptopmag.com/articles/create-guest-account-windows-10

## ...

- Printers & Scanners > Open Queue > Properties > Advanced > Keep printed documents
- You can also enable in the Event Viewer for all printers.

Source

- How to Check Your Printed Document History in Windows 10
  - https://www.howtogeek.com/445760/how-to-check-your-printed-document-history-in-windows-10/

## Timezone

- Settings > Privacy > Location > Allow access to location on this device
- Settings > Privacy > Location > Allow apps to access your location
- Settings > Privacy > Location > Allow desktop apps to access your location
- Settings > Date & time > Set the time zone automatically

Source

- How to Fix Windows 10/11 Time Zone Keeps Changing to Pacific
  - https://bestwindowssoftware.net/windows-time-zone-keeps-changing/ 

## How to Sleep from the Command Line

If you do not have hibernate enabled.

```
rundll32.exe powrprof.dll,SetSuspendState 0,1,0
```

If you do have hibernate enabled.

```
powercfg -h off
rundll32.exe powrprof.dll,SetSuspendState 0,1,0
powercfg -h on
```

Else download [PsShutdown](http://technet.microsoft.com/en-us/sysinternals/bb897541.aspx)

```
psshutdown.exe -d -t 0 -accepteula
```

How to hibernate.

```
shutdown /h
```

Source

- How to hibernate Windows from command line
  - https://www.windows-commandline.com/hibernate-windows/
- How to sleep Windows 10 from the command line
  - https://winaero.com/how-to-sleep-windows-10-from-the-command-line/
