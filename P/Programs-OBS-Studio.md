# Programs - OBS Studio

## How to Fix Black Screen

You need to tell OBS Studio to use the integrated graphics card.

- Go to Settings > Display > Graphics
- Go to Custom options for apps
- Browse to add OBS Studio executable.
- Click on OBS Studio from the list.
- Click on Options.
- Select Power saving

Source

- OBS Black Screen Display Capture Solved (Still Works)
  - https://www.youtube.com/watch?v=awXP6_kDii4&ab_channel=NobleArcade

## ...

```
$ sudo add-apt-repository ppa:obsproject/obs-studio

[sudo] password for iba: 
 Latest stable release of OBS Studio
 More info: https://launchpad.net/~obsproject/+archive/ubuntu/obs-studio
Press [ENTER] to continue or ctrl-c to cancel adding it

gpg: keyring `/tmp/tmpyaf4hqpz/secring.gpg' created
gpg: keyring `/tmp/tmpyaf4hqpz/pubring.gpg' created
gpg: requesting key F425E228 from hkp server keyserver.ubuntu.com
gpg: /tmp/tmpyaf4hqpz/trustdb.gpg: trustdb created
gpg: key F425E228: public key "Launchpad PPA for obsproject" imported
gpg: Total number processed: 1
gpg:               imported: 1  (RSA: 1)
OK

iba@ubuntu:~/git/iba/data$ sudo apt update

Hit:1 http://security.ubuntu.com/ubuntu xenial-security InRelease
Ign:2 https://download.sublimetext.com apt/stable/ InRelease
Err:3 https://download.sublimetext.com apt/stable/ Release
  server certificate verification failed. CAfile: /etc/ssl/certs/ca-certificates.crt CRLfile: none
Get:4 http://ppa.launchpad.net/obsproject/obs-studio/ubuntu xenial InRelease [18.0 kB]
Hit:5 http://us.archive.ubuntu.com/ubuntu xenial InRelease
Get:6 http://ppa.launchpad.net/obsproject/obs-studio/ubuntu xenial/main amd64 Packages [908 B]
Hit:7 http://us.archive.ubuntu.com/ubuntu xenial-updates InRelease                                
Get:8 http://ppa.launchpad.net/obsproject/obs-studio/ubuntu xenial/main i386 Packages [904 B]
Hit:9 http://us.archive.ubuntu.com/ubuntu xenial-backports InRelease                              
Get:10 http://ppa.launchpad.net/obsproject/obs-studio/ubuntu xenial/main Translation-en [160 B]
Reading package lists... Done          
E: The repository 'https://download.sublimetext.com apt/stable/ Release' does not have a Release file.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.

iba@ubuntu:~/git/iba/data$sudo apt install obs-studio
```

Source

- Install Instructions
  - https://obsproject.com/wiki/install-instructions
