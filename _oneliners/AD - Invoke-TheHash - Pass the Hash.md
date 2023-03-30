---
title: |
  Pass the hash 
description: |
  Invoke-TheHash contains PowerShell functions for performing pass the hash WMI and SMB tasks. WMI and SMB connections are accessed through the .NET TCPClient. Authentication is performed by passing an NTLM hash into the NTLMv2 authentication protocol. Local administrator privilege is not required client-side.

  Command Reference:

  	-Type: WMIExec, SMBExec

command: |
  Invoke-TheHash -Type WMIExec -Target 192.168.100.0/24 -TargetExclude 192.168.100.50 -Username Administrator -Hash F6F38B793DB6A94BA04A52F1D3EE92F0
items:
  - Hash
services:
  - SMB
  - WMI
OS:
  - Windows
attack_types:
  - Lateral Movement
references:
  - https://github.com/Kevin-Robertson/Invoke-TheHash
---
