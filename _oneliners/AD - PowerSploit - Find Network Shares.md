---
title: |
  Find Network Shares
description: |
  PowerSploit is a collection of Microsoft PowerShell modules that can be used to aid penetration testers during all phases of an assessment. PowerSploit is comprised of the following modules and scripts:

  Commands:

  	runas /netonly /userAD\User "Powershell.exe -exec bypass"

    PS >. .\c:\Recon\PowerView.ps1

    Import-Module (Resolve-Path('Powersploit'))

    Import-Module (Resolve-Path('Recon'))
    
    $ Invoke-ShareFinder -ComputerFile hosts.txt -NoPing -CheckShareAccess

command: |
  See commands
items:
  - Shell
OS:
  - Windows
attack_types:
  - Enumeration
references:
  - https://github.com/PowerShellMafia/PowerSploit/tree/master/Recon
  - https://github.com/PowerShellMafia/PowerSploit/
---
