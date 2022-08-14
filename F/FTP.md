# FTP

## ...

> Explicit security requires that the FTP client issues a specific command to the FTP server after establishing a connection to establish the SSL link. In explicit TLS the FTP client needs to send an explicit command (i.e. "AUTH TLS") to the FTP server to initiate a secure control connection.

> In Implicit FTP over TLS, there is no need for the FTP Client to send any command to turn on TLS security. In implicit FTP over TLS, TLS handshake must be negotiated before any FTP commands can be sent by the FTP client to the FTP Server.

Source

- SmartFTP - What is the difference between Implicit TLS and Explicit TLS_
  - https://www.smartftp.com/en-us/support/kb/189#:~:text=FTP%20over%20TLS%20(Explicit),initiate%20a%20secure%20control%20connection.
- Difference between explicit FTP over TLS and implicit FTP over TLS.mhtml
  - https://www.omnisecu.com/tcpip/difference-between-explicit-ftp-over-tls-and-implicit-ftp-over-tls.php#:~:text=In%20Implicit%20FTP%20over%20TLS,client%20to%20the%20FTP%20Server.

## ...

> Both SFTP and FTP over TLS securely transfer data—usernames, passwords, and file contents. However, SFTP enables bi-directional secure data transfer using one port. FTP over TLS requires multiple ports to be opened on a firewall—one for command data (to establish an encrypted connection) and at least one for file data.

Source

- SFTP for Secure Data Transfer-Secure FTP over SSL
  - https://www.vandyke.com/products/securefx/sftp.html#:~:text=Both%20SFTP%20and%20FTP%20over%20TLS%20securely%20transfer%20data%E2%80%94usernames,least%20one%20for%20file%20data.
