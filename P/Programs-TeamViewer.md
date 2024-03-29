# Programs - TeamViewer

## How to Turn Off Ads

Extras > Options > Advanced > Show advanced options > In-product marketing messages

Options > Account > Show in-product marketing messages (version 15.31.5)

If the option is greyed out, then sign out and sign back in.

Source

* Why am I getting ads in paid teamviewer?
  * https://community.teamviewer.com/English/discussion/comment/98469#Comment_98469
* In-Product marketing Messages greyed out
  * https://community.teamviewer.com/English/discussion/114981/in-product-marketing-messages-greyed-out

## ...

There is no keyboard shortcut to go back to the host.

Source

- Alt-tab back to the host while using TeamViewer?
  - https://superuser.com/questions/1078295/alt-tab-back-to-the-host-while-using-teamviewer

## “This screen cannot be captured at the moment. This is probably due to to fast user switching or a disconnected/minimized Remote Desktop session.”

Enable the following setting.

- Advanced
  - Advanced settings for connections to this computer
    - Full access control when a partner is connecting to the Windows logon screen

The following did not seem to work. The "User ID" and "Server ID" were the same.

- Use the "Server ID" instead of the "User ID".
- Right click on the TeamViewer Tray Icon > About Teamviewer
- The "Server ID" and the "User ID" can sometimes be the same.

Source

- REMOTE SUPPORT VIA TEAMVIEWER WITHOUT ACTIVE WINDOWS LOGIN ENDS IN “THIS SCREEN CANNOT BE CAPTURED AT THE MOMENT THIS IS DUE TO TO FAST USER SWITCHING OR A DISCONNECTED/MINIMIZED REMOTE DESKTOP SESSION”
  - https://pixelfriedhof.com/en/remote-support-via-teamviewer-without-active-windows-login-ends-in-this-screen-cannot-be-captured-at-the-moment-this-is-due-to-to-fast-user-switching-or-a-disconnected-minimized-remote-desktop-session/#:~:text=at%20the%20moment.-,This%20is%20due%20to%20to%20fast%20user%20switching%20or%20a,ID%20of%20the%20running%20TeamViewer.
- TV ID for User Session - not Device ID
  - https://community.teamviewer.com/English/discussion/2365/tv-id-for-user-session-not-device-id#:~:text=Best%20Answer&text=To%20get%20the%20ID%20of,Hope%20this%20helps!
- ServerID
  - https://community.teamviewer.com/English/discussion/59652/serverid  

## "Options > Advanced > Close to tray menu" Grayed Out

Because you have "Options > General > Start TeamViewer with Windows" activated.

Source

- Version 9.0.32494 won't let me close main window and keep connections active
  - https://teamviewerforums.com/index.php?topic=2462.0
