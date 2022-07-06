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

## Why 192.168... ?

> Per RFC 1918, the following three ranges are reserved for use on private networks:
> 10.0.0.0        -   10.255.255.255  (10/8 prefix)
> 172.16.0.0      -   172.31.255.255  (172.16/12 prefix)
> 192.168.0.0     -   192.168.255.255 (192.168/16 prefix)

Source

- Why 192.168.*.* for local addresses?
  - https://networkengineering.stackexchange.com/questions/5825/why-192-168-for-local-addresses

## ... Autoconfiguration IPV4

When a device can't get an IP number from the DHCP server... it generates a number.

Source

- What is IPv4 Autoconfiguration and why it overwrites static IP
  - https://superuser.com/questions/1243175/what-is-ipv4-autoconfiguration-and-why-it-overwrites-static-ip
