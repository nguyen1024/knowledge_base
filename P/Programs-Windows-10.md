# Programs - Windows 10

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
