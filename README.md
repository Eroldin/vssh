# VSSH
##  A simple plugin for SSH to connect to a NAT VirtualBox machine 

SSH makes it easy to connect to a VirtualBox machine behind a NAT interface.
This however polutes your "known_host" file with (temperory?) keys which most likely won't be used again.
VSSH aims to solve this problem by connecting you to a password protected machine, without leaving anything behind on your system after a successfull logout.

It asks you for the ip/hostname:portnumber, user and password and immeditaly connects you to your system, without further questions. This means tha it can be used to connect to any external system with a ssh server installed.
It can be used for any (virtual) machine. Just keep security policies in mind.

## Features in a nutshell

- No more long terminal commands, just run "vssh" and answer the questions.
- No more manually removing keys from your "known_hosts". VSSH places a temperory file in your /tmp folder
- It does not leave anything on your system. The temparory file is deleted upon a logout, as long as you don't close the window.
- It is distro agnostic. Just make sure sshpass is installed.
