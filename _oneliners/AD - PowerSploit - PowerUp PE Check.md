---
title: |
  Privilege Escalation check (PowerUp.ps1)
description: |
  PowerSploit is a collection of Microsoft PowerShell modules that can be used to aid penetration testers during all phases of an assessment. PowerSploit is comprised of the following modules and scripts:

command: |
  powershell -exec bypass -Command "&{Import-Module .\PowerUp.ps1; Invoke-AllChecks}"
items:
  - Shell
OS:
  - Windows
attack_types:
  - PrivEsc
references:
  - https://github.com/PowerShellMafia/PowerSploit/blob/master/Privesc/PowerUp.ps1
---
