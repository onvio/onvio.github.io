---
title: |
  Mount cifs share on a windows server
description: |
  On Linux and UNIX operating systems, you can use the mount command to attach (mount) file systems and removable devices such as USB flash drives at a particular mount point in the directory tree.

  Command Reference:

  	-t cifs: mount the cifs share on a windows server

command: |
  mount -t cifs //192.168.101.100/sales /mnt/cifs -o
items:
  - No-Creds
services:
  - SMB
attack_types:
  - Enumeration
OS:
  - Linux
references:
  - https://github.com/cddmp/enum4linux-ng
---
