---
title: |
  Find user logged on machines with Invoke-UserHunter
description: |
  PowerView is a module within PowerSploit written in PowerShell to gain network situational awareness on Windows domains. The below command will query the Domain Controller for a list of available shares that the current user has access to.

  Invoke-UserHunter finds machines on the local domain where specified users are logged into, and can optionally check if the current user has local admin access to found machines.

  Other command:

  	powershell -exec bypass -Command "&{Import-Module .\powerview.ps1; Invoke-UserHunter -CheckAccess}"

command: |
  powershell -exec bypass -Command "&{Import-Module .\powerview.ps1; Invoke-UserHunter}"
items:
  - Shell
OS:
  - Windows
attack_types:
  - Enumeration
references:
  - https://github.com/PowerShellMafia/PowerSploit/tree/master/Recon
  - https://www.attackdebris.com/?p=470
  - https://github.com/PowerShellMafia/PowerSploit/
---
