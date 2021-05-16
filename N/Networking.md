# Networking

## ...

PowerShell, TCP

```
Get-Process -Id (Get-NetTCPConnection -LocalPort YourPortNumberHere).OwningProcess
```

PowerShell, UDP

```
Get-Process -Id (Get-NetUDPEndpoint -LocalPort YourPortNumberHere).OwningProcess
```

Command Prompt

```
C:\> netstat -a -b
```

Resource Monitor

* Network > Listening Ports

Source

* How can you find out which process is listening on a TCP or UDP port on Windows?
  * https://stackoverflow.com/questions/48198/how-can-you-find-out-which-process-is-listening-on-a-tcp-or-udp-port-on-windows
