---
title: |
  File Transfers - Windows to Linux - SCP
description: |
  Copy a file:

  	scp /path/to/source/file.txt username@ip:/path/to/destination/file.txt

  Download a file:

  	scp alfred@10.11.1.101:/tmp/output.txt .

  Copy a directory:

  	scp -r /path/to/source/dir username@ip:/path/to/destination

command: |
  See commands.
items:
  - Username
  - Password
OS:
  - Linux
attack_types:
  - Enumeration
  - PrivEsc
references:
  - https://book.hacktricks.xyz/generic-methodologies-and-resources/exfiltration
  - https://isroot.nl/2018/07/09/post-exploitation-file-transfers-on-windows-the-manual-way/
---
