---
title: |
  Search for all possible paths to escalate privileges on Windows hosts (WindowsEnum)
description: |
  A Powershell Privilege Escalation Enumeration Script.

  Command Reference:

  	extended: Extended checks will search for config files, various interesting files, and passwords in files and the registry, etc. It will take some time so be patient.

command: |
  powershell -nologo -executionpolicy bypass -file WindowsEnum.ps1 extended
items:
  - Shell
OS:
  - Windows
attack_types:
  - PrivEsc
references:
  - https://github.com/absolomb/WindowsEnum
  - https://book.hacktricks.xyz/windows/windows-local-privilege-escalation
---
