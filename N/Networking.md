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

## ...

* 2.4 GHz goes further.
* 5 GHz goes faster.

Source

* What is the difference between 2.4 GHz and 5 GHz wireless frequencies?
  * https://kb.netgear.com/29396/What-is-the-difference-between-2-4-GHz-and-5-GHz-wireless-frequencies
