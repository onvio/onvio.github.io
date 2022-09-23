---
title: |
  Dump NTLM hashes locally after dumping the NTDS and SYSTEM
description: |
  Impacket's secretsdump.py will perform various techniques to dump secrets from the remote machine without executing any agent. Techniques include reading SAM and LSA secrets from registries, dumping NTLM hashes, plaintext credentials, and kerberos keys, and dumping NTDS.dit. The following command will attempt to use the specified machines NTDS.dit and system to extract the user account hashes associated with that machine.

  Or Windows Command:

  	NTDSDumpEx.exe -d ntds.dit -s SYSTEM

command: |
  python3 secretsdump.py -ntds ntds.dit -system SYS LOCAL
items:
  - Password
  - Username
services:
  - Kerberos
  - NTLM
OS:
  - Linux
  - Windows
attack_types:
  - Exploitation
references:
  - https://github.com/SecureAuthCorp/impacket/blob/master/examples/secretsdump.py
  - https://riccardoancarani.github.io/2020-05-10-hunting-for-impacket/#secretsdumppy
---
